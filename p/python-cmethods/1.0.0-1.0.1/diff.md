# Comparing `tmp/python_cmethods-1.0.0-py3-none-any.whl.zip` & `tmp/python_cmethods-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 37860 bytes, number of entries: 7
--rw-r--r--  2.0 unx    49343 b- defN 23-Apr-10 19:10 cmethods/__init__.py
--rw-r--r--  2.0 unx      160 b- defN 23-Apr-10 19:10 cmethods/_version.py
--rw-r--r--  2.0 unx    32891 b- defN 23-Apr-10 19:10 python_cmethods-1.0.0.dist-info/LICENSE
--rw-r--r--  2.0 unx    50169 b- defN 23-Apr-10 19:10 python_cmethods-1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-10 19:10 python_cmethods-1.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Apr-10 19:10 python_cmethods-1.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      581 b- defN 23-Apr-10 19:10 python_cmethods-1.0.0.dist-info/RECORD
-7 files, 133245 bytes uncompressed, 36828 bytes compressed:  72.4%
+Zip file size: 39021 bytes, number of entries: 7
+-rw-r--r--  2.0 unx    56727 b- defN 23-Apr-17 17:43 cmethods/__init__.py
+-rw-r--r--  2.0 unx      160 b- defN 23-Apr-17 17:43 cmethods/_version.py
+-rw-r--r--  2.0 unx    32891 b- defN 23-Apr-17 17:43 python_cmethods-1.0.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx    50808 b- defN 23-Apr-17 17:43 python_cmethods-1.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-17 17:43 python_cmethods-1.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Apr-17 17:43 python_cmethods-1.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      581 b- defN 23-Apr-17 17:43 python_cmethods-1.0.1.dist-info/RECORD
+7 files, 141268 bytes uncompressed, 37989 bytes compressed:  73.1%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: cmethods/__init__.py
 Comment: 
 
 Filename: cmethods/_version.py
 Comment: 
 
-Filename: python_cmethods-1.0.0.dist-info/LICENSE
+Filename: python_cmethods-1.0.1.dist-info/LICENSE
 Comment: 
 
-Filename: python_cmethods-1.0.0.dist-info/METADATA
+Filename: python_cmethods-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: python_cmethods-1.0.0.dist-info/WHEEL
+Filename: python_cmethods-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: python_cmethods-1.0.0.dist-info/top_level.txt
+Filename: python_cmethods-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: python_cmethods-1.0.0.dist-info/RECORD
+Filename: python_cmethods-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cmethods/__init__.py

```diff
@@ -54,22 +54,35 @@
         Scaling-based techniques:
             * Linear Scaling :func:`cmethods.CMethods.linear_scaling`
             * Variance Scaling :func:`cmethods.CMethods.variance_scaling`
             * Delta (change) Method :func:`cmethods.CMethods.delta_method`
 
         Distribution-based techniques:
             * Quantile Mapping :func:`cmethods.CMethods.quantile_mapping`
+            * Detrended Quantile Mapping :func:`cmethods.CMethods.detrended_quantile_mapping`
             * Quantile Delta Mapping :func:`cmethods.CMethods.quantile_delta_mapping`
 
-    Except for the Variance Scaling all methods can be applied on both, interval- and ratio- based
-    variables. The Variance Scaling can only be applied on interval-based variables.
+    Except for the Variance Scaling all methods can be applied on both, stochastic and non-stochastic
+    variables. The Variance Scaling can only be applied on stochastic climate variables.
+
+    Stochastic climate variables are those that are subject to random fluctuations
+    and are not predictable. They have no predictable trend or pattern. Examples of
+    stochastic climate variables include precipitation, air temperature, and humidity.
+
+    Non-stochastic climate variables, on the other hand, have clear trend and pattern histories
+    and can be readily predicted. They are often referred to as climate elements and include
+    variables such as water temperature and air pressure.
     """
 
     SCALING_METHODS = ["linear_scaling", "variance_scaling", "delta_method"]
-    DISTRIBUTION_METHODS = ["quantile_mapping", "quantile_delta_mapping"]
+    DISTRIBUTION_METHODS = [
+        "quantile_mapping",
+        "detrended_quantile_mapping",
+        "quantile_delta_mapping",
+    ]
 
     CUSTOM_METHODS = SCALING_METHODS + DISTRIBUTION_METHODS
     METHODS = CUSTOM_METHODS
 
     ADDITIVE = ["+", "add"]
     MULTIPLICATIVE = ["*", "mult"]
 
@@ -115,14 +128,16 @@
             return cls.linear_scaling
         if method == "variance_scaling":
             return cls.variance_scaling
         if method == "delta_method":
             return cls.delta_method
         if method == "quantile_mapping":
             return cls.quantile_mapping
+        if method == "detrended_quantile_mapping":
+            return cls.detrended_quantile_mapping
         if method == "empirical_quantile_mapping":
             return cls.empirical_quantile_mapping
         if method == "quantile_delta_mapping":
             return cls.quantile_delta_mapping
         raise UnknownMethodError(method, cls.METHODS)
 
     @classmethod
@@ -358,16 +373,16 @@
         simh: xr.core.dataarray.DataArray,
         simp: xr.core.dataarray.DataArray,
         group: Union[str, None] = "time.month",
         kind: str = "+",
         **kwargs,
     ) -> np.array:
         r"""
-        The Linear Scaling bias correction technique can be applied on interval- and
-        ratio-based climate variables to minimize deviations in the mean values
+        The Linear Scaling bias correction technique can be applied on stochastic and
+        non-stochastic climate variables to minimize deviations in the mean values
         between predicted and observed time-series of past and future time periods.
 
         Since the multiplicative scaling can result in very high scaling factors,
         a maximum scaling factor of 10 is set. This can be changed by passing
         another value to the optional `max_scaling_factor` argument.
 
         This method must be applied on a 1-dimensional data set i.e., there is only one
@@ -408,16 +423,16 @@
         :param simh: The modeled data of the control period
         :type simh: xr.core.dataarray.DataArray
         :param simp: The modeled data of the scenario period (this is the data set
             on which the bias correction takes action)
         :type simp: xr.core.dataarray.DataArray
         :param group: The grouping defines the basis of the mean, defaults to ``time.month``
         :type group: Union[str, None], optional
-        :param kind: The kind of the correction, additive for interval- and multiplicative
-            for ratio-based variables, defaults to ``+``
+        :param kind: The kind of the correction, additive for non-stochastic and multiplicative
+            for stochastic climate variables, defaults to ``+``
         :type kind: str, optional
         :raises NotImplementedError: If the kind is not in (``+``, ``*``, ``add``, ``mult``)
         :return: The bias-corrected time series
         :rtype: np.array
 
         .. code-block:: python
             :linenos:
@@ -450,15 +465,15 @@
                 kind=kind,
                 **kwargs,
             )
         if kind in cls.ADDITIVE:
             return np.array(simp) + (np.nanmean(obs) - np.nanmean(simh))  # Eq. 1
         if kind in cls.MULTIPLICATIVE:
             adj_scaling_factor = cls.get_adjusted_scaling_factor(
-                np.nanmean(obs) / np.nanmean(simh),
+                cls.ensure_devidable(np.nanmean(obs), np.nanmean(simh)),
                 kwargs.get("max_scaling_factor", cls.MAX_SCALING_FACTOR),
             )
             return np.array(simp) * adj_scaling_factor  # Eq. 2
         raise NotImplementedError(
             f"{kind} not available for linear_scaling. Use '+' or '*' instead."
         )
 
@@ -470,15 +485,15 @@
         simh: xr.core.dataarray.DataArray,
         simp: xr.core.dataarray.DataArray,
         group: Union[str, None] = "time.month",
         kind: str = "+",
         **kwargs,
     ) -> np.array:
         r"""
-        The Variance Scaling bias correction technique can be applied on interval-based
+        The Variance Scaling bias correction technique can be applied only on non-stochastic
         climate variables to minimize deviations in the mean and variance
         between predicted and observed time-series of past and future time periods.
 
         This method must be applied on a 1-dimensional data set i.e., there is only one
         time-series passed for each of ``obs``, ``simh``, and ``simp``.
 
         The Variance Scaling bias correction technique implemented here is based on the
@@ -528,15 +543,15 @@
         :param simh: The modeled data of the control period
         :type simh: xr.core.dataarray.DataArray
         :param simp: The modeled data of the scenario period (this is the data set
             on which the bias correction takes action)
         :type simp: xr.core.dataarray.DataArray
         :param group: The grouping defines the basis of the mean, defaults to ``time.month``
         :type group: Union[str, None], optional
-        :param kind: The kind of the correction, additive for interval-based variables,
+        :param kind: The kind of the correction, additive for non-stochastic climate variables
             no other kind is available so far, defaults to ``+``
         :type kind: str, optional
         :raises NotImplementedError: If the kind is not in (``+``, ``add``)
         :return: The bias-corrected time series
         :rtype: np.array
 
         .. code-block:: python
@@ -573,15 +588,15 @@
             LS_simh = cls.linear_scaling(obs, simh, simh, group=None)  # Eq. 1
             LS_simp = cls.linear_scaling(obs, simh, simp, group=None)  # Eq. 2
 
             VS_1_simh = LS_simh - np.nanmean(LS_simh)  # Eq. 3
             VS_1_simp = LS_simp - np.nanmean(LS_simp)  # Eq. 4
 
             adj_scaling_factor = cls.get_adjusted_scaling_factor(
-                np.std(np.array(obs)) / np.std(VS_1_simh),
+                cls.ensure_devidable(np.std(np.array(obs)), np.std(VS_1_simh)),
                 kwargs.get("max_scaling_factor", cls.MAX_SCALING_FACTOR),
             )
 
             VS_2_simp = VS_1_simp * adj_scaling_factor  # Eq. 5
             return VS_2_simp + np.nanmean(LS_simp)  # Eq. 6
 
         raise NotImplementedError(
@@ -596,16 +611,16 @@
         simh: xr.core.dataarray.DataArray,
         simp: xr.core.dataarray.DataArray,
         group: Union[str, None] = "time.month",
         kind: str = "+",
         **kwargs,
     ) -> np.array:
         r"""
-        The Delta Method bias correction technique can be applied on interval- and
-        ratio-based climate variables to minimize deviations in the mean values
+        The Delta Method bias correction technique can be applied on stochastic and
+        non-stochastic climate variables to minimize deviations in the mean values
         between predicted and observed time-series of past and future time periods.
 
         Since the multiplicative scaling can result in very high scaling factors,
         a maximum scaling factor of 10 is set. This can be changed by passing
         another value to the optional `max_scaling_factor` argument.
 
         This method must be applied on a 1-dimensional data set i.e., there is only one
@@ -647,16 +662,16 @@
         :param simh: The modeled data of the control period
         :type simh: xr.core.dataarray.DataArray
         :param simp: The modeled data of the scenario period (this is the data set
             on which the bias correction takes action)
         :type simp: xr.core.dataarray.DataArray
         :param group: The grouping defines the basis of the mean, defaults to ``time.month``
         :type group: Union[str, None], optional
-        :param kind: The kind of the correction, additive for interval- and multiplicative
-            for ratio-based variables, defaults to ``+``
+        :param kind: The kind of the correction, additive for non-stochastic and multiplicative
+            for stochastic climate variables, defaults to ``+``
         :type kind: str, optional
         :raises NotImplementedError: If the kind is not in (``+``, ``*``, ``add``, ``mult``)
         :return: The bias-corrected time series
         :rtype: np.array
 
         .. code-block:: python
             :linenos:
@@ -688,15 +703,15 @@
                 kind=kind,
                 **kwargs,
             )
         if kind in cls.ADDITIVE:
             return np.array(obs) + (np.nanmean(simp) - np.nanmean(simh))  # Eq. 1
         if kind in cls.MULTIPLICATIVE:
             adj_scaling_factor = cls.get_adjusted_scaling_factor(
-                np.nanmean(simp) / np.nanmean(simh),
+                cls.ensure_devidable(np.nanmean(simp), np.nanmean(simh)),
                 kwargs.get("max_scaling_factor", cls.MAX_SCALING_FACTOR),
             )
             return np.array(obs) * adj_scaling_factor  # Eq. 2
         raise NotImplementedError(
             f"{kind} not available for delta_method. Use '+' or '*' instead."
         )
 
@@ -705,15 +720,14 @@
     def quantile_mapping(
         cls,
         obs: xr.core.dataarray.DataArray,
         simh: xr.core.dataarray.DataArray,
         simp: xr.core.dataarray.DataArray,
         n_quantiles: int,
         kind: str = "+",
-        detrended: bool = False,
         **kwargs,
     ) -> np.array:
         r"""
         The Quantile Mapping bias correction technique can be used to minimize distributional
         biases between modeled and observed time-series climate data. Its interval-independant
         behaviour ensures that the whole time series is taken into account to redistribute
         its values, based on the distributions of the modeled and observed/reference data of the
@@ -723,29 +737,50 @@
         time-series passed for each of ``obs``, ``simh``, and ``simp``.
 
         The Quantile Mapping technique implemented here is based on the equations of
         Alex J. Cannon and Stephen R. Sobie and Trevor Q. Murdock (2015) *"Bias Correction of GCM
         Precipitation by Quantile Mapping: How Well Do Methods Preserve Changes in Quantiles
         and Extremes?"* (https://doi.org/10.1175/JCLI-D-14-00754.1).
 
-        Since the regular Quantile Mapping is bounded to the value range of the modeled data of
-        the control period, the *Detrended* Quantile Mapping approach can be used by setting the
-        ``detrended`` argument to ``True``. Detrending means, that the values of :math:`X_{sim,p}`
-        are shifted to the value range of :math:`X_{sim,h}` before the Quantile Mapping is applied.
-        After the Quantile Mapping was applied, the mean is shifted back. Since it does not make sens
-        to take the whole mean to rescale the data, the month-dependent long-term mean is used.
+        The regular Quantile Mapping is bounded to the value range of the modeled data
+        of the control period. To avoid this, the Detrended Quantile Mapping can be used.
 
-        In the following the equations of Alex J. Cannon (2015) are shown (without detrending):
+        In the following the equations of Alex J. Cannon (2015) are shown and explained:
 
         **Additive**:
 
             .. math::
 
                 X^{*QM}_{sim,p}(i) = F^{-1}_{obs,h} \left\{F_{sim,h}\left[X_{sim,p}(i)\right]\right\}
 
+
+            The additive quantile mapping procedure consists of inserting the value to be
+            adjusted (:math:`X_{sim,p}(i)`) into the cumulative distribution function
+            of the modeled data of the control period (:math:`F_{sim,h}`). This determines,
+            in which quantile the value to be adjusted can be found in the modeled data of the control period
+            The following images show this by using :math:`T` for temperatures.
+
+            .. figure:: ../_static/images/qm-cdf-plot-1.png
+                :width: 600
+                :align: center
+                :alt: Determination of the quantile value
+
+                Fig 1: Inserting :math:`X_{sim,p}(i)` into :math:`F_{sim,h}` to determine the quantile value
+
+            This value, which of course lies between 0 and 1, is subsequently inserted
+            into the inverse cumulative distribution function of the reference data of the control period to
+            determine the bias-corrected value at time step :math:`i`.
+
+            .. figure:: ../_static/images/qm-cdf-plot-2.png
+                :width: 600
+                :align: center
+                :alt: Determination of the QM bias-corrected value
+
+                Fig 1: Inserting the quantile value into :math:`F^{-1}_{obs,h}` to determine the bias-corrected value for time step :math:`i`
+
         **Multiplicative**:
 
             .. math::
 
                 X^{*QM}_{sim,p}(i) = F^{-1}_{obs,h}\Biggl\{F_{sim,h}\left[\frac{\mu{X_{sim,h}} \cdot \mu{X_{sim,p}(i)}}{\mu{X_{sim,p}(i)}}\right]\Biggr\}\frac{\mu{X_{sim,p}(i)}}{\mu{X_{sim,h}}}
 
 
@@ -755,20 +790,21 @@
         :param simh: The modeled data of the control period
         :type simh: xr.core.dataarray.DataArray
         :param simp: The modeled data of the scenario period (this is the data set
             on which the bias correction takes action)
         :type simp: xr.core.dataarray.DataArray
         :param n_quantiles: Number of quantiles to respect/use
         :type n_quantiles: int
-        :param kind: The kind of the correction, additive for interval- and multiplicative
-            for ratio-based variables, defaults to ``+``
+        :param kind: The kind of the correction, additive for non-stochastic and multiplicative
+            for stochastic climate variables, defaults to ``+``
         :type kind: str, optional
-        :param detrended: If the extremes should be respected by applying month-dependent
-            detrending before and after applying the Quantile Mapping
-        :type detrended: bool, optional
+        :param val_min: Lower boundary for interpolation (only if ``kind="*"``, default: ``0.0``)
+        :type val_min: float, optional
+        :param val_max: Upper boundary for interpolation (only if ``kind="*"``, default: ``None``)
+        :type val_max: float, optional
         :raises NotImplementedError: If the kind is not in (``+``, ``*``, ``add``, ``mult``)
         :return: The bias-corrected time series
         :rtype: np.array
 
         .. code-block:: python
             :linenos:
             :caption: Example: Quantile Mapping
@@ -786,82 +822,182 @@
             >>> qm_adjusted = cm.quantile_mapping(
             ...     obs=obs[variable],
             ...     simh=simh[variable],
             ...     simp=simp[variable],
             ...     n_quantiles=250
             ... )
         """
-        obs, simh, simp_ = np.array(obs), np.array(simh), np.array(simp)
+        obs, simh, simp = np.array(obs), np.array(simh), np.array(simp)
 
         global_max = max(np.amax(obs), np.amax(simh))
         global_min = min(np.amin(obs), np.amin(simh))
         wide = abs(global_max - global_min) / n_quantiles
         xbins = np.arange(global_min, global_max + wide, wide)
 
         cdf_obs = cls.get_cdf(obs, xbins)
         cdf_simh = cls.get_cdf(simh, xbins)
 
-        if detrended:
-            # detrended => shift mean of $X_{sim,p}$ to range of $X_{sim,h}$ to adjust extremes
-            res = np.zeros(len(simp.values))
-            for _, idxs in simp.groupby("time.month").groups.items():
-                # detrended by long-term month
-                m_simh, m_simp = [], []
-                for idx in idxs:
-                    m_simh.append(simh[idx])
-                    m_simp.append(simp[idx])
-
-                m_simh = np.array(m_simh)
-                m_simp = np.array(m_simp)
-                m_simh_mean = np.nanmean(m_simh)
-                m_simp_mean = np.nanmean(m_simp)
-
-                if kind in cls.ADDITIVE:
-                    epsilon = np.interp(
-                        m_simp - m_simp_mean + m_simh_mean, xbins, cdf_simh
-                    )  # Eq. 1
-                    X = (
-                        cls.get_inverse_of_cdf(cdf_obs, epsilon, xbins)
-                        + m_simp_mean
-                        - m_simh_mean
-                    )  # Eq. 1
-
-                elif kind in cls.MULTIPLICATIVE:
-                    epsilon = np.interp(  # Eq. 2
-                        (m_simh_mean * m_simp) / m_simp_mean,
-                        xbins,
-                        cdf_simh,
-                        left=kwargs.get("val_min", 0.0),
-                        right=kwargs.get("val_max", None),
-                    )
-                    X = np.interp(epsilon, cdf_obs, xbins) * (
-                        m_simp_mean / m_simh_mean
-                    )  # Eq. 2
-                for i, idx in enumerate(idxs):
-                    res[idx] = X[i]
-            return res
-
         if kind in cls.ADDITIVE:
-            epsilon = np.interp(simp_, xbins, cdf_simh)  # Eq. 1
+            epsilon = np.interp(simp, xbins, cdf_simh)  # Eq. 1
             return cls.get_inverse_of_cdf(cdf_obs, epsilon, xbins)  # Eq. 1
 
         if kind in cls.MULTIPLICATIVE:
             epsilon = np.interp(  # Eq. 2
-                simp_,
+                simp,
                 xbins,
                 cdf_simh,
                 left=kwargs.get("val_min", 0.0),
                 right=kwargs.get("val_max", None),
             )
             return cls.get_inverse_of_cdf(cdf_obs, epsilon, xbins)  # Eq. 2
 
         raise NotImplementedError(
             f"{kind} for quantile_mapping is not available. Use '+' or '*' instead."
         )
 
+    @classmethod
+    def detrended_quantile_mapping(
+        cls,
+        obs: xr.core.dataarray.DataArray,
+        simh: xr.core.dataarray.DataArray,
+        simp: xr.core.dataarray.DataArray,
+        n_quantiles: int,
+        kind: str = "+",
+        **kwargs,
+    ) -> np.array:
+        r"""
+        The Detrended Quantile Mapping bias correction technique can be used to minimize distributional
+        biases between modeled and observed time-series climate data like the regular Quantile Mapping.
+        Detrending means, that the values of :math:`X_{sim,p}` are shifted to the value range of
+        :math:`X_{sim,h}` before the regular Quantile Mapping is applied.
+        After the Quantile Mapping was applied, the mean is shifted back. Since it does not make sens
+        to take the whole mean to rescale the data, the month-dependent long-term mean is used.
+
+        This method must be applied on a 1-dimensional data set i.e., there is only one
+        time-series passed for each of ``obs``, ``simh``, and ``simp``. Also this method requires
+        that the time series are groupable by ``time.month``.
+
+        The Detrended Quantile Mapping technique implemented here is based on the equations of
+        Alex J. Cannon and Stephen R. Sobie and Trevor Q. Murdock (2015) *"Bias Correction of GCM
+        Precipitation by Quantile Mapping: How Well Do Methods Preserve Changes in Quantiles
+        and Extremes?"* (https://doi.org/10.1175/JCLI-D-14-00754.1).
+
+        In the following the equations of Alex J. Cannon (2015) are shown (without detrending; see QM
+        for explainations):
+
+        **Additive**:
+
+            .. math::
+
+                X^{*QM}_{sim,p}(i) = F^{-1}_{obs,h} \left\{F_{sim,h}\left[X_{sim,p}(i)\right]\right\}
+
+
+        **Multiplicative**:
+
+            .. math::
+
+                X^{*QM}_{sim,p}(i) = F^{-1}_{obs,h}\Biggl\{F_{sim,h}\left[\frac{\mu{X_{sim,h}} \cdot \mu{X_{sim,p}(i)}}{\mu{X_{sim,p}(i)}}\right]\Biggr\}\frac{\mu{X_{sim,p}(i)}}{\mu{X_{sim,h}}}
+
+
+        :param obs: The reference data set of the control period
+            (in most cases the observational data)
+        :type obs: xr.core.dataarray.DataArray
+        :param simh: The modeled data of the control period
+        :type simh: xr.core.dataarray.DataArray
+        :param simp: The modeled data of the scenario period (this is the data set
+            on which the bias correction takes action)
+        :type simp: xr.core.dataarray.DataArray
+        :param n_quantiles: Number of quantiles to respect/use
+        :type n_quantiles: int
+        :param kind: The kind of the correction, additive for non-stochastic and multiplicative
+            for stochastic climate variables, defaults to ``+``
+        :type kind: str, optional
+        :param val_min: Lower boundary for interpolation (only if ``kind="*"``, default: ``0.0``)
+        :type val_min: float, optional
+        :param val_max: Upper boundary for interpolation (only if ``kind="*"``, default: ``None``)
+        :type val_max: float, optional
+        :raises NotImplementedError: If the kind is not in (``+``, ``*``, ``add``, ``mult``)
+        :return: The bias-corrected time series
+        :rtype: np.array
+
+        .. code-block:: python
+            :linenos:
+            :caption: Example: Quantile Mapping
+
+            >>> import xarray as xr
+            >>> from cmethods import CMethods as cm
+
+            >>> # Note: The data sets must contain the dimension "time"
+            >>> #       for the respective variable.
+            >>> obsh = xr.open_dataset("path/to/reference_data-control_period.nc")
+            >>> simh = xr.open_dataset("path/to/modeled_data-control_period.nc")
+            >>> simp = xr.open_dataset("path/to/the_dataset_to_adjust-scenario_period.nc")
+            >>> variable = "tas" # temperatures
+
+            >>> qm_adjusted = cm.detrended_quantile_mapping(
+            ...     obs=obs[variable],
+            ...     simh=simh[variable],
+            ...     simp=simp[variable],
+            ...     n_quantiles=250
+            ... )
+        """
+        if kind not in cls.MULTIPLICATIVE and kind not in cls.ADDITIVE:
+            raise NotImplementedError(
+                f"{kind} for detrended_quantile_mapping is not available. Use '+' or '*' instead."
+            )
+
+        obs, simh = np.array(obs), np.array(simh)
+
+        global_max = max(np.amax(obs), np.amax(simh))
+        global_min = min(np.amin(obs), np.amin(simh))
+        wide = abs(global_max - global_min) / n_quantiles
+        xbins = np.arange(global_min, global_max + wide, wide)
+
+        cdf_obs = cls.get_cdf(obs, xbins)
+        cdf_simh = cls.get_cdf(simh, xbins)
+
+        # detrended => shift mean of $X_{sim,p}$ to range of $X_{sim,h}$ to adjust extremes
+        res = np.zeros(len(simp.values))
+        for _, idxs in simp.groupby("time.month").groups.items():
+            # detrended by long-term month
+            m_simh, m_simp = [], []
+            for idx in idxs:
+                m_simh.append(simh[idx])
+                m_simp.append(simp[idx])
+
+            m_simh = np.array(m_simh)
+            m_simp = np.array(m_simp)
+            m_simh_mean = np.nanmean(m_simh)
+            m_simp_mean = np.nanmean(m_simp)
+
+            if kind in cls.ADDITIVE:
+                epsilon = np.interp(
+                    m_simp - m_simp_mean + m_simh_mean, xbins, cdf_simh
+                )  # Eq. 1
+                X = (
+                    cls.get_inverse_of_cdf(cdf_obs, epsilon, xbins)
+                    + m_simp_mean
+                    - m_simh_mean
+                )  # Eq. 1
+
+            elif kind in cls.MULTIPLICATIVE:
+                epsilon = np.interp(  # Eq. 2
+                    cls.ensure_devidable((m_simh_mean * m_simp), m_simp_mean),
+                    xbins,
+                    cdf_simh,
+                    left=kwargs.get("val_min", 0.0),
+                    right=kwargs.get("val_max", None),
+                )
+                X = np.interp(epsilon, cdf_obs, xbins) * cls.ensure_devidable(
+                    m_simp_mean, m_simh_mean
+                )  # Eq. 2
+            for i, idx in enumerate(idxs):
+                res[idx] = X[i]
+        return res
+
     # ? -----========= E M P I R I C A L - Q U A N T I L E - M A P P I N G =========------
     @classmethod
     def empirical_quantile_mapping(
         cls,
         obs: xr.core.dataarray.DataArray,
         simh: xr.core.dataarray.DataArray,
         simp: xr.core.dataarray.DataArray,
@@ -965,15 +1101,15 @@
 
             **(2.3)** The :math:`\Delta(i)` in the multiplicative Quantile Delta Mapping is calulated like the
             additive variant, but using the relative than the absolute change.
 
                 .. math::
 
                     \Delta(i) & = \frac{ F^{-1}_{sim,p}\left[\varepsilon(i)\right] }{ F^{-1}_{sim,h}\left[\varepsilon(i)\right] } \\[1pt]
-                              & = \frac{ X_{sim,p}(i) }{ F^{-1}_{sim,h}\left\{F^{}_{sim,p}\left[X_{sim,p}(i)\right]\right\} }
+                              & = \frac{ X_{sim,p}(i) }{ F^{-1}_{sim,h}\left\{F_{sim,p}\left[X_{sim,p}(i)\right]\right\} }
 
 
             **(2.4)** The relative change between the modeled data of the control and scenario period is than
             multiplicated with the bias-corrected value (see **1.2**).
 
                 .. math::
 
@@ -986,16 +1122,16 @@
         :param simh: The modeled data of the control period
         :type simh: xr.core.dataarray.DataArray
         :param simp: The modeled data of the scenario period (this is the data set
             on which the bias correction takes action)
         :type simp: xr.core.dataarray.DataArray
         :param n_quantiles: Number of quantiles to respect/use
         :type n_quantiles: int
-        :param kind: The kind of the correction, additive for interval- and multiplicative
-            for ratio-based variables, defaults to ``+``
+        :param kind: The kind of the correction, additive for non-stochastic and multiplicative
+            for non-stochastic climate variables, defaults to ``+``
         :type kind: str, optional
         :raises NotImplementedError: If the kind is not in (``+``, ``*``, ``add``, ``mult``)
         :return: The bias-corrected time series
         :rtype: np.array
 
         .. code-block:: python
             :linenos:
@@ -1048,25 +1184,54 @@
             cdf_obs = cls.get_cdf(obs, xbins)
             cdf_simh = cls.get_cdf(simh, xbins)
             cdf_simp = cls.get_cdf(simp, xbins)
 
             epsilon = np.interp(simp, xbins, cdf_simp)  # Eq. 1.1
             QDM1 = cls.get_inverse_of_cdf(cdf_obs, epsilon, xbins)  # Eq. 1.2
 
-            with np.errstate(divide="ignore", invalid="ignore"):
-                delta = simp / cls.get_inverse_of_cdf(
-                    cdf_simh, epsilon, xbins
-                )  # Eq. 2.3
-            delta[np.isnan(delta)] = 0
-
+            delta = cls.ensure_devidable(
+                simp, cls.get_inverse_of_cdf(cdf_simh, epsilon, xbins)
+            )  # Eq. 2.3
             return QDM1 * delta  # Eq. 2.4
         raise NotImplementedError(
             f"{kind} not available for quantile_delta_mapping. Use '+' or '*' instead."
         )
 
+    @classmethod
+    def ensure_devidable(
+        cls, numerator: Union[float, np.array], denominator: Union[float, np.array]
+    ) -> np.array:
+        """
+        Ensures that the arrays can be devided. The numerator will be multiplied by
+        the maximum scaling factor of the CMethods class if division by zero.
+
+        :param numerator: Numerator to use
+        :type numerator: np.array
+        :param denominator: Denominator that can be zero
+        :type denominator: np.array
+        :return: Zero-ensured devision
+        :rtype: np.array
+        """
+        with np.errstate(divide="ignore", invalid="ignore"):
+            result = numerator / denominator
+
+        if isinstance(numerator, np.ndarray):
+            mask_inf = np.isinf(result)
+            result[mask_inf] = numerator[mask_inf] * cls.MAX_SCALING_FACTOR
+
+            mask_nan = np.isnan(result)
+            result[mask_nan] = 0
+        else:
+            if np.isinf(result):
+                result = numerator * cls.MAX_SCALING_FACTOR
+            elif np.isnan(result):
+                result = 0
+
+        return result
+
     @staticmethod
     def get_pdf(x: Union[list, np.array], xbins: Union[list, np.array]) -> np.array:
         r"""
         Compuites and returns the the probability density function :math:`P(x)`
         of ``x`` based on ``xbins``.
 
         :param x: The vector to get :math:`P(x)` from
@@ -1121,15 +1286,15 @@
     @staticmethod
     def get_inverse_of_cdf(
         base_cdf: Union[list, np.array],
         insert_cdf: Union[list, np.array],
         xbins: Union[list, np.array],
     ) -> np.array:
         r"""
-        Returns the inverse cumulative distribution function of with the following
+        Returns the inverse cumulative distribution function as:
         :math:`F^{-1}_{x}\left[y\right]` where :math:`x` represents ``base_cdf`` and
         ``insert_cdf`` is represented by :math:`y`.
 
         :param base_cdf: The basis
         :type base_cdf: Union[list, np.array]
         :param insert_cdf: The CDF that gets inserted
         :type insert_cdf: Union[list, np.array]
@@ -1148,15 +1313,15 @@
         Returns:
             - :math:`x` if :math:`-|y| \le x \le |y|`,
             - :math:`|y|` if :math:`x > |y|`, or
             - :math:`-|y|` if :math:`x < -|y|`
 
             where:
                 - :math:`x` is ``factor``
-                - :math:`y` is ``max_scaling_factor``.
+                - :math:`y` is ``max_scaling_factor``
 
         :param factor: The value to check for
         :type factor: Union[int, float]
         :param max_scaling_factor: The maximum/minimum allowed value
         :type max_scaling_factor: Union[int, float]
         :return: The correct value
         :rtype: float
```

## cmethods/_version.py

```diff
@@ -1,4 +1,4 @@
 # file generated by setuptools_scm
 # don't change, don't track in version control
-__version__ = version = '1.0.0'
-__version_tuple__ = version_tuple = (1, 0, 0)
+__version__ = version = '1.0.1'
+__version_tuple__ = version_tuple = (1, 0, 1)
```

## Comparing `python_cmethods-1.0.0.dist-info/LICENSE` & `python_cmethods-1.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `python_cmethods-1.0.0.dist-info/METADATA` & `python_cmethods-1.0.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-cmethods
-Version: 1.0.0
+Version: 1.0.1
 Summary: Collection of bias correction procedures for 1- and 3-dimensional climate data
 Author-email: Benjamin Thomas Schwertfeger <development@b-schwertfeger.de>
 License: GNU GENERAL PUBLIC LICENSE
         Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
         Everyone is permitted to copy and distribute verbatim copies
@@ -689,15 +689,15 @@
 [![DOI](https://zenodo.org/badge/496160109.svg)](https://zenodo.org/badge/latestdoi/496160109)
 [![Documentation Status](https://readthedocs.org/projects/python-cmethods/badge/?version=stable)](https://python-cmethods.readthedocs.io/en/latest/?badge=stable)
 
 </div>
 
 This Python module serves as a collection of different scale- and distribution-based bias correction techniques for climatic research
 
-The documentation is available at: [https://python-kraken-sdk.readthedocs.io/en/stable/](https://python-kraken-sdk.readthedocs.io/en/stable/)
+The documentation is available at: [https://python-cmethods.readthedocs.io/en/stable/](https://python-cmethods.readthedocs.io/en/stable/)
 
 > ⚠️ For the application of bias corrections on _lage data sets_ it is recomanded to use the command-line tool [BiasAdjustCXX](https://github.com/btschwertfeger/BiasAdjustCXX) since bias corrections are complex statistical transformation which are very slow in Python compared to the C++ implementation.
 
 ---
 
 ## Table of Contents
 
@@ -710,29 +710,29 @@
 
 ---
 
 <a name="about"></a>
 
 ## 1. About
 
-These programs and data structures are designed to help minimize discrepancies between modeled and observed climate data. Data from past periods are used to adjust variables from current and future time series so that their distributional properties approximate possible actual values.
+These programs and data structures are developed with the aim of reducing discrepancies between modeled and observed climate data. Historical data is utilized to calibrate variables from current and future time series to achieve distributional properties that closely resemble the possible actual values.
 
 <figure>
   <img
-  src="docs/images/biasCdiagram.png?raw=true"
+  src="docs/_static/images/biasCdiagram.png?raw=true"
   alt="Schematic representation of a bias adjustment procedure"
   style="background-color: white; border-radius: 7px">
   <figcaption>Figure 1: Schematic representation of a bias adjustment procedure</figcaption>
 </figure>
 
-In this way, for example, modeled data, which on average represent values that are too cold, can be adjusted by applying an adjustment procedure. The following figure shows the observed, the modeled, and the adjusted values. It is directly visible that the delta adjusted time series ($T^{\*DM}_{sim,p}$) are much more similar to the observed data ($T_{obs,p}$) than the raw modeled data ($T_{sim,p}$).
+For instance, modeled data typically indicate values that are colder than the actual values. To address this issue, an adjustment procedure is employed. The figure below illustrates the observed, modeled, and adjusted values, revealing that the delta adjusted time series ($T^{*DM}_{sim,p}$) are significantly more similar to the observed data ($T{obs,p}$) than the raw modeled data ($T_{sim,p}$).
 
 <figure>
   <img
-  src="docs/images/dm-doy-plot.png?raw=true"
+  src="docs/_static/images/dm-doy-plot.png?raw=true"
   alt="Temperature per day of year in modeled, observed and bias-adjusted climate data"
   style="background-color: white; border-radius: 7px">
   <figcaption>Figure 2: Temperature per day of year in observed, modeled, and bias-adjusted climate data</figcaption>
 </figure>
 
 ---
 
@@ -747,14 +747,25 @@
 | `linear_scaling`         | Linear Scaling (additive and multiplicative)                                                                                                                 |
 | `variance_scaling`       | Variance Scaling (additive)                                                                                                                                  |
 | `delta_method`           | Delta (Change) Method (additive and multiplicative)                                                                                                          |
 | `quantile_mapping`       | Quantile Mapping (additive and multiplicative) and Detrended Quantile Mapping (additive and multiplicative; to use DQM, set parameter `detrended` to `True`) |
 | `quantile_delta_mapping` | Quantile Delta Mapping (additive and multiplicative)                                                                                                         |
 | `adjust_3d`              | requires a method name and the respective parameters to adjust all time series of a 3-dimensional data set                                                   |
 
+Except for the variance scaling, all methods can be applied on stochastic and non-stochastic
+climate variables. Variance scaling can only be applied on non-stochastic climate variables.
+
+- Stochastic climate variables are those that are subject to random fluctuations
+  and are not predictable. They have no predictable trend or pattern. Examples of
+  stochastic climate variables include precipitation, air temperature, and humidity.
+
+- Non-stochastic climate variables, on the other hand, have clear trend and pattern histories
+  and can be readily predicted. They are often referred to as climate elements and include
+  variables such as water temperature and air pressure.
+
 ---
 
 <a name="installation"></a>
 
 ## 3. Installation
 
 ```bash
@@ -788,21 +799,21 @@
     simh = simh['tas'],
     simp = simp['tas'],
     n_quaniles = 1000,
     kind = '+'
 )
 # to calculate the relative rather than the absolute change,
 # '*' can be used instead of '+' (this is prefered when adjusting
-# ratio based variables like precipitation)
+# stochastic variables like precipitation)
 ```
 
 Notes:
 
 - When using the `adjust_3d` method you have to specify the method by name.
-- For the multiplicative linear scaling and the delta method as well as the variance scaling method a maximum scaling factor of 10 is defined. This can be changed by the parameter `max_scaling_factor`.
+- For the multiplicative techniques a maximum scaling factor of 10 is defined. This can be changed by the attribute `max_scaling_factor`.
 
 ## Examples (see repository on [GitHub](https://github.com/btschwertfeger/python-cmethods))
 
 Notebook with different methods and plots: `/examples/examples.ipynb`
 
 There is also an exmple script (`/examples/biasadjust.py`) that can be used to apply the available bias correction methods
 on 1- and 3-dimensional data sets (see `/examples/input_data/*.nc`).
```

