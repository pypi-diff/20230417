# Comparing `tmp/jupyterlab_blockly-0.3.0a0.tar.gz` & `tmp/jupyterlab_blockly-0.3.0a1.tar.gz`

## Comparing `jupyterlab_blockly-0.3.0a0.tar` & `jupyterlab_blockly-0.3.0a1.tar`

### file list

```diff
@@ -1,695 +1,695 @@
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/.eslintignore
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/.eslintrc.js
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/.prettierignore
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/.prettierrc
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/.readthedocs.yml
--rw-r--r--   0        0        0    24473 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/CHANGELOG.md
--rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/RELEASE.md
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/install.json
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/lerna.json
--rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/package.json
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/setup.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/tsconfig.eslint.json
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/tsconfig.json
--rw-r--r--   0        0        0   342722 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/yarn.lock
--rw-r--r--   0        0        0    68615 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/assets/info_full_release.png
--rw-r--r--   0        0        0   175573 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/assets/merge_changelog.png
--rw-r--r--   0        0        0   165057 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/assets/run_draft_changelog.png
--rw-r--r--   0        0        0   174150 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/assets/run_full_release.png
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/docs/Makefile
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/docs/blockly_editor.md
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/docs/blockly_files.md
--rw-r--r--   0        0        0     2803 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/docs/conf.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/docs/environment.yml
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/docs/example.jpblockly
--rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/docs/examples.md
--rw-r--r--   0        0        0     3400 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/docs/functions.jpblockly
--rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/docs/index.rst
--rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/docs/installation.md
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/docs/jupyter-lite.json
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/docs/jupyterlab_integration.md
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/docs/jupyterlite_config.json
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/docs/kernels.md
--rw-r--r--   0        0        0     4077 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/docs/logic.jpblockly
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/docs/loops.jpblockly
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/docs/make.bat
--rw-r--r--   0        0        0     7151 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/docs/other_extensions.md
--rw-r--r--   0        0        0     4127 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/docs/text_and_lists.jpblockly
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/docs/toolbox.md
--rw-r--r--   0        0        0    75296 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/docs/_static/BlocklyOverview.png
--rw-r--r--   0        0        0   176466 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/docs/_static/OverviewBlockly.gif
--rw-r--r--   0        0        0    60807 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/docs/_static/changeKernel.png
--rw-r--r--   0        0        0    28267 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/docs/_static/commentBlock.png
--rw-r--r--   0        0        0   104770 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/docs/_static/creatingVariable.gif
--rw-r--r--   0        0        0    71339 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/docs/_static/darkBlockly.png
--rw-r--r--   0        0        0   101648 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/docs/_static/ifBlock.gif
--rw-r--r--   0        0        0    27639 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/docs/_static/openBlocklyEditor.png
--rw-r--r--   0        0        0    88956 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/docs/_static/openFromLauncher.png
--rw-r--r--   0        0        0    10678 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/docs/_static/selectKernel.png
--rw-r--r--   0        0        0  1007479 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/docs/_static/shortBlocklyDemo.gif
--rw-r--r--   0        0        0    29212 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/docs/_static/toolboxSwitch.png
--rw-r--r--   0        0        0   193519 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/docs/_static/toolboxView.gif
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/examples/example.jpblockly
--rw-r--r--   0        0        0     3293 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/examples/functions.jpblockly
--rw-r--r--   0        0        0     3971 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/examples/logic.jpblockly
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/examples/loops.jpblockly
--rw-r--r--   0        0        0     4231 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/examples/text_and_lists.jpblockly
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/__init__.py
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/_version.py
--rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/package.json
--rw-r--r--   0        0        0    28584 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/109.624848fd57458c5dd4f0.js
--rw-r--r--   0        0        0    48490 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/109.624848fd57458c5dd4f0.js.map
--rw-r--r--   0        0        0    31279 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/157.921bbfb16083689ff62a.js
--rw-r--r--   0        0        0    50866 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/157.921bbfb16083689ff62a.js.map
--rw-r--r--   0        0        0    28431 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/168.8383bc2d0a83f2b959fd.js
--rw-r--r--   0        0        0    48064 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/168.8383bc2d0a83f2b959fd.js.map
--rw-r--r--   0        0        0    28488 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/173.df5a30c1440df850aa82.js
--rw-r--r--   0        0        0    48333 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/173.df5a30c1440df850aa82.js.map
--rw-r--r--   0        0        0    35787 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/210.35c06ed0583039490182.js
--rw-r--r--   0        0        0    55693 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/210.35c06ed0583039490182.js.map
--rw-r--r--   0        0        0   625206 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/215.82ec42ef5a24d2ff187f.js
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/215.82ec42ef5a24d2ff187f.js.LICENSE.txt
--rw-r--r--   0        0        0  1745486 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/215.82ec42ef5a24d2ff187f.js.map
--rw-r--r--   0        0        0     6026 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/216.011d737685936c4c8e1a.js
--rw-r--r--   0        0        0    16800 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/216.011d737685936c4c8e1a.js.map
--rw-r--r--   0        0        0    28813 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/232.d5cb8a2dcc0d34fabd8a.js
--rw-r--r--   0        0        0    48644 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/232.d5cb8a2dcc0d34fabd8a.js.map
--rw-r--r--   0        0        0    28219 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/268.4eaefedf266ea50fd6df.js
--rw-r--r--   0        0        0    48105 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/268.4eaefedf266ea50fd6df.js.map
--rw-r--r--   0        0        0    28387 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/31.418331b4a22dffe518b4.js
--rw-r--r--   0        0        0    48065 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/31.418331b4a22dffe518b4.js.map
--rw-r--r--   0        0        0    30585 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/326.f8d1ef211f999b0b3dca.js
--rw-r--r--   0        0        0    50268 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/326.f8d1ef211f999b0b3dca.js.map
--rw-r--r--   0        0        0    31628 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/382.0016faf875cb665ac9b2.js
--rw-r--r--   0        0        0    51447 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/382.0016faf875cb665ac9b2.js.map
--rw-r--r--   0        0        0    28777 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/410.941cb48faa5e2d568b13.js
--rw-r--r--   0        0        0    48689 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/410.941cb48faa5e2d568b13.js.map
--rw-r--r--   0        0        0    28161 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/428.cb1cafd5e6ba8a81b05a.js
--rw-r--r--   0        0        0    48219 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/428.cb1cafd5e6ba8a81b05a.js.map
--rw-r--r--   0        0        0    31528 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/513.5646d474a0e4d9613886.js
--rw-r--r--   0        0        0    51567 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/513.5646d474a0e4d9613886.js.map
--rw-r--r--   0        0        0    32792 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/533.606434cc067b99350123.js
--rw-r--r--   0        0        0    52613 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/533.606434cc067b99350123.js.map
--rw-r--r--   0        0        0    39949 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/549.dbfa5147d8fec7e5a76f.js
--rw-r--r--   0        0        0    59869 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/549.dbfa5147d8fec7e5a76f.js.map
--rw-r--r--   0        0        0    36365 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/588.3e52218ff8bfd1512578.js
--rw-r--r--   0        0        0    56138 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/588.3e52218ff8bfd1512578.js.map
--rw-r--r--   0        0        0    78268 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/593.526fcc348e87fac11681.js
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/593.526fcc348e87fac11681.js.LICENSE.txt
--rw-r--r--   0        0        0   178349 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/593.526fcc348e87fac11681.js.map
--rw-r--r--   0        0        0    36509 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/617.c198d75d062c9be68fef.js
--rw-r--r--   0        0        0    56465 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/617.c198d75d062c9be68fef.js.map
--rw-r--r--   0        0        0    28137 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/619.84aef6ceee0a82ac27ee.js
--rw-r--r--   0        0        0    48131 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/619.84aef6ceee0a82ac27ee.js.map
--rw-r--r--   0        0        0    28292 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/627.5da93440391d7167f88d.js
--rw-r--r--   0        0        0    48933 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/627.5da93440391d7167f88d.js.map
--rw-r--r--   0        0        0     4881 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/643.34f4f43b70e246a962a8.js
--rw-r--r--   0        0        0    20194 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/643.34f4f43b70e246a962a8.js.map
--rw-r--r--   0        0        0    30103 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/647.d729bd3d64d38278f913.js
--rw-r--r--   0        0        0    49677 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/647.d729bd3d64d38278f913.js.map
--rw-r--r--   0        0        0    28152 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/655.13bd86e04776bccddcee.js
--rw-r--r--   0        0        0    48041 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/655.13bd86e04776bccddcee.js.map
--rw-r--r--   0        0        0    27281 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/671.5cc50d235d821a731440.js
--rw-r--r--   0        0        0    52560 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/671.5cc50d235d821a731440.js.map
--rw-r--r--   0        0        0    28971 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/693.91ee036f7a5bf0e5a1b0.js
--rw-r--r--   0        0        0    48999 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/693.91ee036f7a5bf0e5a1b0.js.map
--rw-r--r--   0        0        0    27162 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/698.48373f0b62bef71acebe.js
--rw-r--r--   0        0        0    46766 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/698.48373f0b62bef71acebe.js.map
--rw-r--r--   0        0        0    28108 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/704.cf482c52df64c1afcb10.js
--rw-r--r--   0        0        0    48203 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/704.cf482c52df64c1afcb10.js.map
--rw-r--r--   0        0        0    21496 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/835.cbd12870eccd44d69cf0.js
--rw-r--r--   0        0        0    57250 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/835.cbd12870eccd44d69cf0.js.map
--rw-r--r--   0        0        0    76408 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/839.c46366b4bade6ade8403.js
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/839.c46366b4bade6ade8403.js.LICENSE.txt
--rw-r--r--   0        0        0   172185 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/839.c46366b4bade6ade8403.js.map
--rw-r--r--   0        0        0    28765 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/929.d864f042fdaf411ba52b.js
--rw-r--r--   0        0        0    48784 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/929.d864f042fdaf411ba52b.js.map
--rw-r--r--   0        0        0    27934 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/939.973bc21fa6263dbabd09.js
--rw-r--r--   0        0        0    48001 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/939.973bc21fa6263dbabd09.js.map
--rw-r--r--   0        0        0    27211 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/974.5f4a862a240a7368a2b5.js
--rw-r--r--   0        0        0    46914 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/974.5f4a862a240a7368a2b5.js.map
--rw-r--r--   0        0        0    10830 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/remoteEntry.64321718d51bd0ccabe6.js
--rw-r--r--   0        0        0    45150 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/remoteEntry.64321718d51bd0ccabe6.js.map
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/style.js
--rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/patches/@jupyterlab+codeeditor+3.6.1.patch
--rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/scripts/bump-version.py
--rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/package.json
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/tsconfig.json
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/.bin/rimraf -> ../rimraf/dist/cjs/src/bin.js
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/.bin/tsc -> ../../../../node_modules/typescript/bin/tsc
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/.bin/tsserver -> ../../../../node_modules/typescript/bin/tsserver
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/brace-expansion/LICENSE
--rw-r--r--   0        0        0     4252 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/brace-expansion/README.md
--rw-r--r--   0        0        0     4992 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/brace-expansion/index.js
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/brace-expansion/package.json
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/brace-expansion/.github/FUNDING.yml
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/LICENSE
--rw-r--r--   0        0        0    39545 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/README.md
--rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/package.json
--rw-r--r--   0        0        0    12284 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/cjs/glob.d.ts
--rw-r--r--   0        0        0     3763 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/cjs/glob.d.ts.map
--rw-r--r--   0        0        0     7550 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/cjs/glob.js
--rw-r--r--   0        0        0     6560 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/cjs/glob.js.map
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/cjs/has-magic.d.ts
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/cjs/has-magic.d.ts.map
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/cjs/has-magic.js
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/cjs/has-magic.js.map
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/cjs/ignore.d.ts
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/cjs/ignore.d.ts.map
--rw-r--r--   0        0        0     3791 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/cjs/ignore.js
--rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/cjs/ignore.js.map
--rw-r--r--   0        0        0     4357 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/cjs/index-cjs.d.ts
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/cjs/index-cjs.d.ts.map
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/cjs/index-cjs.js
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/cjs/index-cjs.js.map
--rw-r--r--   0        0        0     6045 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/cjs/index.d.ts
--rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/cjs/index.d.ts.map
--rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/cjs/index.js
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/cjs/index.js.map
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/cjs/package.json
--rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/cjs/pattern.d.ts
--rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/cjs/pattern.d.ts.map
--rw-r--r--   0        0        0     7298 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/cjs/pattern.js
--rw-r--r--   0        0        0     5949 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/cjs/pattern.js.map
--rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/cjs/processor.d.ts
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/cjs/processor.d.ts.map
--rw-r--r--   0        0        0    10937 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/cjs/processor.js
--rw-r--r--   0        0        0     8994 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/cjs/processor.js.map
--rw-r--r--   0        0        0     4190 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/cjs/walker.d.ts
--rw-r--r--   0        0        0     4571 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/cjs/walker.d.ts.map
--rw-r--r--   0        0        0    11900 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/cjs/walker.js
--rw-r--r--   0        0        0    12084 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/cjs/walker.js.map
--rw-r--r--   0        0        0    12284 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/mjs/glob.d.ts
--rw-r--r--   0        0        0     3763 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/mjs/glob.d.ts.map
--rw-r--r--   0        0        0     7353 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/mjs/glob.js
--rw-r--r--   0        0        0     6719 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/mjs/glob.js.map
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/mjs/has-magic.d.ts
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/mjs/has-magic.d.ts.map
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/mjs/has-magic.js
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/mjs/has-magic.js.map
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/mjs/ignore.d.ts
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/mjs/ignore.d.ts.map
--rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/mjs/ignore.js
--rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/mjs/ignore.js.map
--rw-r--r--   0        0        0     6045 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/mjs/index.d.ts
--rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/mjs/index.d.ts.map
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/mjs/index.js
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/mjs/index.js.map
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/mjs/package.json
--rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/mjs/pattern.d.ts
--rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/mjs/pattern.d.ts.map
--rw-r--r--   0        0        0     7159 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/mjs/pattern.js
--rw-r--r--   0        0        0     5965 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/mjs/pattern.js.map
--rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/mjs/processor.d.ts
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/mjs/processor.d.ts.map
--rw-r--r--   0        0        0    10630 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/mjs/processor.js
--rw-r--r--   0        0        0     8987 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/mjs/processor.js.map
--rw-r--r--   0        0        0     4190 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/mjs/walker.d.ts
--rw-r--r--   0        0        0     4571 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/mjs/walker.d.ts.map
--rw-r--r--   0        0        0    11441 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/mjs/walker.js
--rw-r--r--   0        0        0    12125 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/mjs/walker.js.map
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minimatch/LICENSE
--rw-r--r--   0        0        0    17061 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minimatch/README.md
--rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minimatch/package.json
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minimatch/dist/cjs/brace-expressions.d.ts
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minimatch/dist/cjs/brace-expressions.d.ts.map
--rw-r--r--   0        0        0     5763 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minimatch/dist/cjs/brace-expressions.js
--rw-r--r--   0        0        0     4882 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minimatch/dist/cjs/brace-expressions.js.map
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minimatch/dist/cjs/escape.d.ts
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minimatch/dist/cjs/escape.d.ts.map
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minimatch/dist/cjs/escape.js
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minimatch/dist/cjs/escape.js.map
--rw-r--r--   0        0        0     3176 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minimatch/dist/cjs/index-cjs.d.ts
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minimatch/dist/cjs/index-cjs.d.ts.map
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minimatch/dist/cjs/index-cjs.js
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minimatch/dist/cjs/index-cjs.js.map
--rw-r--r--   0        0        0     3784 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minimatch/dist/cjs/index.d.ts
--rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minimatch/dist/cjs/index.d.ts.map
--rw-r--r--   0        0        0    52207 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minimatch/dist/cjs/index.js
--rw-r--r--   0        0        0    42018 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minimatch/dist/cjs/index.js.map
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minimatch/dist/cjs/package.json
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minimatch/dist/cjs/unescape.d.ts
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minimatch/dist/cjs/unescape.d.ts.map
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minimatch/dist/cjs/unescape.js
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minimatch/dist/cjs/unescape.js.map
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minimatch/dist/mjs/brace-expressions.d.ts
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minimatch/dist/mjs/brace-expressions.d.ts.map
--rw-r--r--   0        0        0     5631 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minimatch/dist/mjs/brace-expressions.js
--rw-r--r--   0        0        0     4866 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minimatch/dist/mjs/brace-expressions.js.map
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minimatch/dist/mjs/escape.d.ts
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minimatch/dist/mjs/escape.d.ts.map
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minimatch/dist/mjs/escape.js
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minimatch/dist/mjs/escape.js.map
--rw-r--r--   0        0        0     3784 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minimatch/dist/mjs/index.d.ts
--rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minimatch/dist/mjs/index.d.ts.map
--rw-r--r--   0        0        0    50982 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minimatch/dist/mjs/index.js
--rw-r--r--   0        0        0    42020 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minimatch/dist/mjs/index.js.map
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minimatch/dist/mjs/package.json
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minimatch/dist/mjs/unescape.d.ts
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minimatch/dist/mjs/unescape.d.ts.map
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minimatch/dist/mjs/unescape.js
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minimatch/dist/mjs/unescape.js.map
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minipass/LICENSE
--rw-r--r--   0        0        0    25522 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minipass/README.md
--rw-r--r--   0        0        0     4245 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minipass/index.d.ts
--rw-r--r--   0        0        0    18549 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minipass/index.js
--rw-r--r--   0        0        0    18532 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minipass/index.mjs
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minipass/package.json
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/LICENSE
--rw-r--r--   0        0        0     8564 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/README.md
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/package.json
--rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/package.json
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/bin.d.ts
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/bin.d.ts.map
--rwxr-xr-x   0        0        0     8928 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/bin.js
--rw-r--r--   0        0        0     6527 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/bin.js.map
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/default-tmp.d.ts
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/default-tmp.d.ts.map
--rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/default-tmp.js
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/default-tmp.js.map
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/fix-eperm.d.ts
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/fix-eperm.d.ts.map
--rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/fix-eperm.js
--rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/fix-eperm.js.map
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/fs.d.ts
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/fs.d.ts.map
--rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/fs.js
--rw-r--r--   0        0        0     3180 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/fs.js.map
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/ignore-enoent.d.ts
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/ignore-enoent.d.ts.map
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/ignore-enoent.js
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/ignore-enoent.js.map
--rw-r--r--   0        0        0     4885 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/index-cjs.d.ts
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/index-cjs.d.ts.map
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/index-cjs.js
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/index-cjs.js.map
--rw-r--r--   0        0        0     4150 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/index.d.ts
--rw-r--r--   0        0        0     3313 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/index.d.ts.map
--rw-r--r--   0        0        0     4605 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/index.js
--rw-r--r--   0        0        0     3938 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/index.js.map
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/opt-arg.d.ts
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/opt-arg.d.ts.map
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/opt-arg.js
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/opt-arg.js.map
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/path-arg.d.ts
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/path-arg.d.ts.map
--rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/path-arg.js
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/path-arg.js.map
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/platform.d.ts
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/platform.d.ts.map
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/platform.js
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/platform.js.map
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/readdir-or-error.d.ts
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/readdir-or-error.d.ts.map
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/readdir-or-error.js
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/readdir-or-error.js.map
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/retry-busy.d.ts
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/retry-busy.d.ts.map
--rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/retry-busy.js
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/retry-busy.js.map
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/rimraf-manual.d.ts
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/rimraf-manual.d.ts.map
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/rimraf-manual.js
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/rimraf-manual.js.map
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/rimraf-move-remove.d.ts
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/rimraf-move-remove.d.ts.map
--rw-r--r--   0        0        0     6655 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/rimraf-move-remove.js
--rw-r--r--   0        0        0     6167 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/rimraf-move-remove.js.map
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/rimraf-native.d.ts
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/rimraf-native.d.ts.map
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/rimraf-native.js
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/rimraf-native.js.map
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/rimraf-posix.d.ts
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/rimraf-posix.d.ts.map
--rw-r--r--   0        0        0     4310 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/rimraf-posix.js
--rw-r--r--   0        0        0     3803 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/rimraf-posix.js.map
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/rimraf-windows.d.ts
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/rimraf-windows.d.ts.map
--rw-r--r--   0        0        0     6622 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/rimraf-windows.js
--rw-r--r--   0        0        0     5752 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/rimraf-windows.js.map
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/use-native.d.ts
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/use-native.d.ts.map
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/use-native.js
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/use-native.js.map
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/default-tmp.d.ts
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/default-tmp.d.ts.map
--rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/default-tmp.js
--rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/default-tmp.js.map
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/fix-eperm.d.ts
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/fix-eperm.d.ts.map
--rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/fix-eperm.js
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/fix-eperm.js.map
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/fs.d.ts
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/fs.d.ts.map
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/fs.js
--rw-r--r--   0        0        0     3151 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/fs.js.map
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/ignore-enoent.d.ts
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/ignore-enoent.d.ts.map
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/ignore-enoent.js
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/ignore-enoent.js.map
--rw-r--r--   0        0        0     4150 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/index.d.ts
--rw-r--r--   0        0        0     3310 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/index.d.ts.map
--rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/index.js
--rw-r--r--   0        0        0     4171 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/index.js.map
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/opt-arg.d.ts
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/opt-arg.d.ts.map
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/opt-arg.js
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/opt-arg.js.map
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/package.json
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/path-arg.d.ts
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/path-arg.d.ts.map
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/path-arg.js
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/path-arg.js.map
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/platform.d.ts
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/platform.d.ts.map
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/platform.js
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/platform.js.map
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/readdir-or-error.d.ts
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/readdir-or-error.d.ts.map
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/readdir-or-error.js
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/readdir-or-error.js.map
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/retry-busy.d.ts
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/retry-busy.d.ts.map
--rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/retry-busy.js
--rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/retry-busy.js.map
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/rimraf-manual.d.ts
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/rimraf-manual.d.ts.map
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/rimraf-manual.js
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/rimraf-manual.js.map
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/rimraf-move-remove.d.ts
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/rimraf-move-remove.d.ts.map
--rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/rimraf-move-remove.js
--rw-r--r--   0        0        0     6278 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/rimraf-move-remove.js.map
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/rimraf-native.d.ts
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/rimraf-native.d.ts.map
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/rimraf-native.js
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/rimraf-native.js.map
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/rimraf-posix.d.ts
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/rimraf-posix.d.ts.map
--rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/rimraf-posix.js
--rw-r--r--   0        0        0     3882 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/rimraf-posix.js.map
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/rimraf-windows.d.ts
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/rimraf-windows.d.ts.map
--rw-r--r--   0        0        0     6049 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/rimraf-windows.js
--rw-r--r--   0        0        0     5904 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/rimraf-windows.js.map
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/use-native.d.ts
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/use-native.d.ts.map
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/use-native.js
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/use-native.js.map
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/src/factory.ts
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/src/index.ts
--rw-r--r--   0        0        0     7343 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/src/layout.ts
--rw-r--r--   0        0        0     4896 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/src/manager.ts
--rw-r--r--   0        0        0     5627 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/src/registry.ts
--rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/src/token.ts
--rw-r--r--   0        0        0    16084 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/src/utils.ts
--rw-r--r--   0        0        0     3380 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/src/widget.ts
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/src/toolbar/generator.tsx
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/src/toolbar/index.ts
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/src/toolbar/toolbox.tsx
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/src/toolbar/utils.ts
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly/style/index.js
--rw-r--r--   0        0        0     2642 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/package.json
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/tsconfig.json
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/webpack.config.js
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/.bin/build-labextension -> ../../../../node_modules/@jupyterlab/builder/lib/build-labextension.js
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/.bin/npm-run-all -> ../../../../node_modules/npm-run-all/bin/npm-run-all/index.js
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/.bin/rimraf -> ../rimraf/dist/cjs/src/bin.js
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/.bin/run-p -> ../../../../node_modules/npm-run-all/bin/run-p/index.js
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/.bin/run-s -> ../../../../node_modules/npm-run-all/bin/run-s/index.js
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/.bin/tsc -> ../../../../node_modules/typescript/bin/tsc
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/.bin/tsserver -> ../../../../node_modules/typescript/bin/tsserver
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/brace-expansion/LICENSE
--rw-r--r--   0        0        0     4252 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/brace-expansion/README.md
--rw-r--r--   0        0        0     4992 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/brace-expansion/index.js
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/brace-expansion/package.json
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/brace-expansion/.github/FUNDING.yml
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/LICENSE
--rw-r--r--   0        0        0    39545 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/README.md
--rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/package.json
--rw-r--r--   0        0        0    12284 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/cjs/glob.d.ts
--rw-r--r--   0        0        0     3763 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/cjs/glob.d.ts.map
--rw-r--r--   0        0        0     7550 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/cjs/glob.js
--rw-r--r--   0        0        0     6560 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/cjs/glob.js.map
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/cjs/has-magic.d.ts
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/cjs/has-magic.d.ts.map
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/cjs/has-magic.js
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/cjs/has-magic.js.map
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/cjs/ignore.d.ts
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/cjs/ignore.d.ts.map
--rw-r--r--   0        0        0     3791 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/cjs/ignore.js
--rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/cjs/ignore.js.map
--rw-r--r--   0        0        0     4357 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/cjs/index-cjs.d.ts
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/cjs/index-cjs.d.ts.map
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/cjs/index-cjs.js
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/cjs/index-cjs.js.map
--rw-r--r--   0        0        0     6045 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/cjs/index.d.ts
--rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/cjs/index.d.ts.map
--rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/cjs/index.js
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/cjs/index.js.map
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/cjs/package.json
--rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/cjs/pattern.d.ts
--rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/cjs/pattern.d.ts.map
--rw-r--r--   0        0        0     7298 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/cjs/pattern.js
--rw-r--r--   0        0        0     5949 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/cjs/pattern.js.map
--rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/cjs/processor.d.ts
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/cjs/processor.d.ts.map
--rw-r--r--   0        0        0    10937 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/cjs/processor.js
--rw-r--r--   0        0        0     8994 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/cjs/processor.js.map
--rw-r--r--   0        0        0     4190 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/cjs/walker.d.ts
--rw-r--r--   0        0        0     4571 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/cjs/walker.d.ts.map
--rw-r--r--   0        0        0    11900 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/cjs/walker.js
--rw-r--r--   0        0        0    12084 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/cjs/walker.js.map
--rw-r--r--   0        0        0    12284 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/mjs/glob.d.ts
--rw-r--r--   0        0        0     3763 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/mjs/glob.d.ts.map
--rw-r--r--   0        0        0     7353 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/mjs/glob.js
--rw-r--r--   0        0        0     6719 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/mjs/glob.js.map
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/mjs/has-magic.d.ts
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/mjs/has-magic.d.ts.map
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/mjs/has-magic.js
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/mjs/has-magic.js.map
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/mjs/ignore.d.ts
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/mjs/ignore.d.ts.map
--rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/mjs/ignore.js
--rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/mjs/ignore.js.map
--rw-r--r--   0        0        0     6045 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/mjs/index.d.ts
--rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/mjs/index.d.ts.map
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/mjs/index.js
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/mjs/index.js.map
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/mjs/package.json
--rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/mjs/pattern.d.ts
--rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/mjs/pattern.d.ts.map
--rw-r--r--   0        0        0     7159 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/mjs/pattern.js
--rw-r--r--   0        0        0     5965 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/mjs/pattern.js.map
--rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/mjs/processor.d.ts
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/mjs/processor.d.ts.map
--rw-r--r--   0        0        0    10630 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/mjs/processor.js
--rw-r--r--   0        0        0     8987 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/mjs/processor.js.map
--rw-r--r--   0        0        0     4190 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/mjs/walker.d.ts
--rw-r--r--   0        0        0     4571 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/mjs/walker.d.ts.map
--rw-r--r--   0        0        0    11441 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/mjs/walker.js
--rw-r--r--   0        0        0    12125 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/mjs/walker.js.map
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minimatch/LICENSE
--rw-r--r--   0        0        0    17061 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minimatch/README.md
--rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minimatch/package.json
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minimatch/dist/cjs/brace-expressions.d.ts
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minimatch/dist/cjs/brace-expressions.d.ts.map
--rw-r--r--   0        0        0     5763 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minimatch/dist/cjs/brace-expressions.js
--rw-r--r--   0        0        0     4882 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minimatch/dist/cjs/brace-expressions.js.map
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minimatch/dist/cjs/escape.d.ts
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minimatch/dist/cjs/escape.d.ts.map
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minimatch/dist/cjs/escape.js
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minimatch/dist/cjs/escape.js.map
--rw-r--r--   0        0        0     3176 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minimatch/dist/cjs/index-cjs.d.ts
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minimatch/dist/cjs/index-cjs.d.ts.map
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minimatch/dist/cjs/index-cjs.js
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minimatch/dist/cjs/index-cjs.js.map
--rw-r--r--   0        0        0     3784 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minimatch/dist/cjs/index.d.ts
--rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minimatch/dist/cjs/index.d.ts.map
--rw-r--r--   0        0        0    52207 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minimatch/dist/cjs/index.js
--rw-r--r--   0        0        0    42018 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minimatch/dist/cjs/index.js.map
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minimatch/dist/cjs/package.json
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minimatch/dist/cjs/unescape.d.ts
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minimatch/dist/cjs/unescape.d.ts.map
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minimatch/dist/cjs/unescape.js
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minimatch/dist/cjs/unescape.js.map
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minimatch/dist/mjs/brace-expressions.d.ts
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minimatch/dist/mjs/brace-expressions.d.ts.map
--rw-r--r--   0        0        0     5631 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minimatch/dist/mjs/brace-expressions.js
--rw-r--r--   0        0        0     4866 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minimatch/dist/mjs/brace-expressions.js.map
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minimatch/dist/mjs/escape.d.ts
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minimatch/dist/mjs/escape.d.ts.map
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minimatch/dist/mjs/escape.js
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minimatch/dist/mjs/escape.js.map
--rw-r--r--   0        0        0     3784 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minimatch/dist/mjs/index.d.ts
--rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minimatch/dist/mjs/index.d.ts.map
--rw-r--r--   0        0        0    50982 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minimatch/dist/mjs/index.js
--rw-r--r--   0        0        0    42020 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minimatch/dist/mjs/index.js.map
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minimatch/dist/mjs/package.json
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minimatch/dist/mjs/unescape.d.ts
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minimatch/dist/mjs/unescape.d.ts.map
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minimatch/dist/mjs/unescape.js
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minimatch/dist/mjs/unescape.js.map
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minipass/LICENSE
--rw-r--r--   0        0        0    25522 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minipass/README.md
--rw-r--r--   0        0        0     4245 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minipass/index.d.ts
--rw-r--r--   0        0        0    18549 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minipass/index.js
--rw-r--r--   0        0        0    18532 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minipass/index.mjs
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minipass/package.json
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/LICENSE
--rw-r--r--   0        0        0     8564 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/README.md
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/package.json
--rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/package.json
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/bin.d.ts
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/bin.d.ts.map
--rwxr-xr-x   0        0        0     8928 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/bin.js
--rw-r--r--   0        0        0     6527 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/bin.js.map
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/default-tmp.d.ts
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/default-tmp.d.ts.map
--rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/default-tmp.js
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/default-tmp.js.map
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/fix-eperm.d.ts
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/fix-eperm.d.ts.map
--rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/fix-eperm.js
--rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/fix-eperm.js.map
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/fs.d.ts
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/fs.d.ts.map
--rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/fs.js
--rw-r--r--   0        0        0     3180 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/fs.js.map
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/ignore-enoent.d.ts
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/ignore-enoent.d.ts.map
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/ignore-enoent.js
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/ignore-enoent.js.map
--rw-r--r--   0        0        0     4885 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/index-cjs.d.ts
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/index-cjs.d.ts.map
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/index-cjs.js
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/index-cjs.js.map
--rw-r--r--   0        0        0     4150 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/index.d.ts
--rw-r--r--   0        0        0     3313 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/index.d.ts.map
--rw-r--r--   0        0        0     4605 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/index.js
--rw-r--r--   0        0        0     3938 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/index.js.map
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/opt-arg.d.ts
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/opt-arg.d.ts.map
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/opt-arg.js
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/opt-arg.js.map
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/path-arg.d.ts
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/path-arg.d.ts.map
--rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/path-arg.js
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/path-arg.js.map
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/platform.d.ts
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/platform.d.ts.map
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/platform.js
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/platform.js.map
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/readdir-or-error.d.ts
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/readdir-or-error.d.ts.map
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/readdir-or-error.js
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/readdir-or-error.js.map
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/retry-busy.d.ts
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/retry-busy.d.ts.map
--rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/retry-busy.js
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/retry-busy.js.map
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/rimraf-manual.d.ts
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/rimraf-manual.d.ts.map
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/rimraf-manual.js
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/rimraf-manual.js.map
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/rimraf-move-remove.d.ts
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/rimraf-move-remove.d.ts.map
--rw-r--r--   0        0        0     6655 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/rimraf-move-remove.js
--rw-r--r--   0        0        0     6167 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/rimraf-move-remove.js.map
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/rimraf-native.d.ts
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/rimraf-native.d.ts.map
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/rimraf-native.js
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/rimraf-native.js.map
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/rimraf-posix.d.ts
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/rimraf-posix.d.ts.map
--rw-r--r--   0        0        0     4310 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/rimraf-posix.js
--rw-r--r--   0        0        0     3803 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/rimraf-posix.js.map
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/rimraf-windows.d.ts
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/rimraf-windows.d.ts.map
--rw-r--r--   0        0        0     6622 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/rimraf-windows.js
--rw-r--r--   0        0        0     5752 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/rimraf-windows.js.map
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/use-native.d.ts
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/use-native.d.ts.map
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/use-native.js
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/use-native.js.map
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/default-tmp.d.ts
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/default-tmp.d.ts.map
--rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/default-tmp.js
--rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/default-tmp.js.map
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/fix-eperm.d.ts
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/fix-eperm.d.ts.map
--rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/fix-eperm.js
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/fix-eperm.js.map
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/fs.d.ts
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/fs.d.ts.map
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/fs.js
--rw-r--r--   0        0        0     3151 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/fs.js.map
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/ignore-enoent.d.ts
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/ignore-enoent.d.ts.map
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/ignore-enoent.js
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/ignore-enoent.js.map
--rw-r--r--   0        0        0     4150 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/index.d.ts
--rw-r--r--   0        0        0     3310 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/index.d.ts.map
--rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/index.js
--rw-r--r--   0        0        0     4171 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/index.js.map
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/opt-arg.d.ts
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/opt-arg.d.ts.map
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/opt-arg.js
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/opt-arg.js.map
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/package.json
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/path-arg.d.ts
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/path-arg.d.ts.map
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/path-arg.js
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/path-arg.js.map
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/platform.d.ts
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/platform.d.ts.map
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/platform.js
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/platform.js.map
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/readdir-or-error.d.ts
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/readdir-or-error.d.ts.map
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/readdir-or-error.js
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/readdir-or-error.js.map
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/retry-busy.d.ts
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/retry-busy.d.ts.map
--rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/retry-busy.js
--rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/retry-busy.js.map
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/rimraf-manual.d.ts
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/rimraf-manual.d.ts.map
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/rimraf-manual.js
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/rimraf-manual.js.map
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/rimraf-move-remove.d.ts
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/rimraf-move-remove.d.ts.map
--rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/rimraf-move-remove.js
--rw-r--r--   0        0        0     6278 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/rimraf-move-remove.js.map
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/rimraf-native.d.ts
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/rimraf-native.d.ts.map
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/rimraf-native.js
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/rimraf-native.js.map
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/rimraf-posix.d.ts
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/rimraf-posix.d.ts.map
--rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/rimraf-posix.js
--rw-r--r--   0        0        0     3882 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/rimraf-posix.js.map
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/rimraf-windows.d.ts
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/rimraf-windows.d.ts.map
--rw-r--r--   0        0        0     6049 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/rimraf-windows.js
--rw-r--r--   0        0        0     5904 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/rimraf-windows.js.map
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/use-native.d.ts
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/use-native.d.ts.map
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/use-native.js
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/use-native.js.map
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/src/icons.ts
--rw-r--r--   0        0        0     7916 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/src/index.ts
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/src/svg.d.ts
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/style/index.js
--rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/packages/blockly-extension/style/icons/blockly_logo.svg
--rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/.gitignore
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/LICENSE
--rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/README.md
--rw-r--r--   0        0        0     2541 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/pyproject.toml
--rw-r--r--   0        0        0     6404 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a0/PKG-INFO
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/.eslintignore
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/.eslintrc.js
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/.prettierignore
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/.prettierrc
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/.readthedocs.yml
+-rw-r--r--   0        0        0    25303 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/CHANGELOG.md
+-rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/RELEASE.md
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/install.json
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/lerna.json
+-rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/package.json
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/setup.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/tsconfig.eslint.json
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/tsconfig.json
+-rw-r--r--   0        0        0   352745 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/yarn.lock
+-rw-r--r--   0        0        0    68615 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/assets/info_full_release.png
+-rw-r--r--   0        0        0   175573 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/assets/merge_changelog.png
+-rw-r--r--   0        0        0   165057 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/assets/run_draft_changelog.png
+-rw-r--r--   0        0        0   174150 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/assets/run_full_release.png
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/docs/Makefile
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/docs/blockly_editor.md
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/docs/blockly_files.md
+-rw-r--r--   0        0        0     2803 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/docs/conf.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/docs/environment.yml
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/docs/example.jpblockly
+-rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/docs/examples.md
+-rw-r--r--   0        0        0     3400 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/docs/functions.jpblockly
+-rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/docs/index.rst
+-rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/docs/installation.md
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/docs/jupyter-lite.json
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/docs/jupyterlab_integration.md
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/docs/jupyterlite_config.json
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/docs/kernels.md
+-rw-r--r--   0        0        0     4077 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/docs/logic.jpblockly
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/docs/loops.jpblockly
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/docs/make.bat
+-rw-r--r--   0        0        0     7151 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/docs/other_extensions.md
+-rw-r--r--   0        0        0     4127 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/docs/text_and_lists.jpblockly
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/docs/toolbox.md
+-rw-r--r--   0        0        0    75296 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/docs/_static/BlocklyOverview.png
+-rw-r--r--   0        0        0   176466 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/docs/_static/OverviewBlockly.gif
+-rw-r--r--   0        0        0    60807 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/docs/_static/changeKernel.png
+-rw-r--r--   0        0        0    28267 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/docs/_static/commentBlock.png
+-rw-r--r--   0        0        0   104770 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/docs/_static/creatingVariable.gif
+-rw-r--r--   0        0        0    71339 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/docs/_static/darkBlockly.png
+-rw-r--r--   0        0        0   101648 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/docs/_static/ifBlock.gif
+-rw-r--r--   0        0        0    27639 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/docs/_static/openBlocklyEditor.png
+-rw-r--r--   0        0        0    88956 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/docs/_static/openFromLauncher.png
+-rw-r--r--   0        0        0    10678 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/docs/_static/selectKernel.png
+-rw-r--r--   0        0        0  1007479 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/docs/_static/shortBlocklyDemo.gif
+-rw-r--r--   0        0        0    29212 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/docs/_static/toolboxSwitch.png
+-rw-r--r--   0        0        0   193519 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/docs/_static/toolboxView.gif
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/examples/example.jpblockly
+-rw-r--r--   0        0        0     3293 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/examples/functions.jpblockly
+-rw-r--r--   0        0        0     3971 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/examples/logic.jpblockly
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/examples/loops.jpblockly
+-rw-r--r--   0        0        0     4231 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/examples/text_and_lists.jpblockly
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/__init__.py
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/_version.py
+-rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/package.json
+-rw-r--r--   0        0        0    28584 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/109.624848fd57458c5dd4f0.js
+-rw-r--r--   0        0        0    48490 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/109.624848fd57458c5dd4f0.js.map
+-rw-r--r--   0        0        0    31279 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/157.921bbfb16083689ff62a.js
+-rw-r--r--   0        0        0    50866 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/157.921bbfb16083689ff62a.js.map
+-rw-r--r--   0        0        0    28431 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/168.8383bc2d0a83f2b959fd.js
+-rw-r--r--   0        0        0    48064 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/168.8383bc2d0a83f2b959fd.js.map
+-rw-r--r--   0        0        0    28488 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/173.df5a30c1440df850aa82.js
+-rw-r--r--   0        0        0    48333 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/173.df5a30c1440df850aa82.js.map
+-rw-r--r--   0        0        0    35787 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/210.35c06ed0583039490182.js
+-rw-r--r--   0        0        0    55693 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/210.35c06ed0583039490182.js.map
+-rw-r--r--   0        0        0   625206 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/215.82ec42ef5a24d2ff187f.js
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/215.82ec42ef5a24d2ff187f.js.LICENSE.txt
+-rw-r--r--   0        0        0  1745486 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/215.82ec42ef5a24d2ff187f.js.map
+-rw-r--r--   0        0        0     6363 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/216.751d5114e75a3795211f.js
+-rw-r--r--   0        0        0    18052 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/216.751d5114e75a3795211f.js.map
+-rw-r--r--   0        0        0    28813 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/232.d5cb8a2dcc0d34fabd8a.js
+-rw-r--r--   0        0        0    48644 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/232.d5cb8a2dcc0d34fabd8a.js.map
+-rw-r--r--   0        0        0    28219 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/268.4eaefedf266ea50fd6df.js
+-rw-r--r--   0        0        0    48105 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/268.4eaefedf266ea50fd6df.js.map
+-rw-r--r--   0        0        0    28387 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/31.418331b4a22dffe518b4.js
+-rw-r--r--   0        0        0    48065 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/31.418331b4a22dffe518b4.js.map
+-rw-r--r--   0        0        0    30585 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/326.f8d1ef211f999b0b3dca.js
+-rw-r--r--   0        0        0    50268 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/326.f8d1ef211f999b0b3dca.js.map
+-rw-r--r--   0        0        0    31628 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/382.0016faf875cb665ac9b2.js
+-rw-r--r--   0        0        0    51447 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/382.0016faf875cb665ac9b2.js.map
+-rw-r--r--   0        0        0    28777 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/410.941cb48faa5e2d568b13.js
+-rw-r--r--   0        0        0    48689 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/410.941cb48faa5e2d568b13.js.map
+-rw-r--r--   0        0        0    28161 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/428.cb1cafd5e6ba8a81b05a.js
+-rw-r--r--   0        0        0    48219 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/428.cb1cafd5e6ba8a81b05a.js.map
+-rw-r--r--   0        0        0    31528 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/513.5646d474a0e4d9613886.js
+-rw-r--r--   0        0        0    51567 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/513.5646d474a0e4d9613886.js.map
+-rw-r--r--   0        0        0    32792 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/533.606434cc067b99350123.js
+-rw-r--r--   0        0        0    52613 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/533.606434cc067b99350123.js.map
+-rw-r--r--   0        0        0    39949 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/549.dbfa5147d8fec7e5a76f.js
+-rw-r--r--   0        0        0    59869 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/549.dbfa5147d8fec7e5a76f.js.map
+-rw-r--r--   0        0        0    36365 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/588.3e52218ff8bfd1512578.js
+-rw-r--r--   0        0        0    56138 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/588.3e52218ff8bfd1512578.js.map
+-rw-r--r--   0        0        0    78268 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/593.526fcc348e87fac11681.js
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/593.526fcc348e87fac11681.js.LICENSE.txt
+-rw-r--r--   0        0        0   178349 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/593.526fcc348e87fac11681.js.map
+-rw-r--r--   0        0        0    36509 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/617.c198d75d062c9be68fef.js
+-rw-r--r--   0        0        0    56465 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/617.c198d75d062c9be68fef.js.map
+-rw-r--r--   0        0        0    28137 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/619.84aef6ceee0a82ac27ee.js
+-rw-r--r--   0        0        0    48131 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/619.84aef6ceee0a82ac27ee.js.map
+-rw-r--r--   0        0        0    28292 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/627.5da93440391d7167f88d.js
+-rw-r--r--   0        0        0    48933 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/627.5da93440391d7167f88d.js.map
+-rw-r--r--   0        0        0     4881 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/643.34f4f43b70e246a962a8.js
+-rw-r--r--   0        0        0    20194 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/643.34f4f43b70e246a962a8.js.map
+-rw-r--r--   0        0        0    30103 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/647.d729bd3d64d38278f913.js
+-rw-r--r--   0        0        0    49677 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/647.d729bd3d64d38278f913.js.map
+-rw-r--r--   0        0        0    28152 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/655.13bd86e04776bccddcee.js
+-rw-r--r--   0        0        0    48041 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/655.13bd86e04776bccddcee.js.map
+-rw-r--r--   0        0        0    27281 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/671.5cc50d235d821a731440.js
+-rw-r--r--   0        0        0    52560 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/671.5cc50d235d821a731440.js.map
+-rw-r--r--   0        0        0    28971 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/693.91ee036f7a5bf0e5a1b0.js
+-rw-r--r--   0        0        0    48999 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/693.91ee036f7a5bf0e5a1b0.js.map
+-rw-r--r--   0        0        0    27162 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/698.48373f0b62bef71acebe.js
+-rw-r--r--   0        0        0    46766 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/698.48373f0b62bef71acebe.js.map
+-rw-r--r--   0        0        0    28108 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/704.cf482c52df64c1afcb10.js
+-rw-r--r--   0        0        0    48203 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/704.cf482c52df64c1afcb10.js.map
+-rw-r--r--   0        0        0    21644 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/835.6f7e7b701fee67a1ec53.js
+-rw-r--r--   0        0        0    58232 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/835.6f7e7b701fee67a1ec53.js.map
+-rw-r--r--   0        0        0    76408 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/839.c46366b4bade6ade8403.js
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/839.c46366b4bade6ade8403.js.LICENSE.txt
+-rw-r--r--   0        0        0   172185 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/839.c46366b4bade6ade8403.js.map
+-rw-r--r--   0        0        0    28765 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/929.d864f042fdaf411ba52b.js
+-rw-r--r--   0        0        0    48784 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/929.d864f042fdaf411ba52b.js.map
+-rw-r--r--   0        0        0    27934 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/939.973bc21fa6263dbabd09.js
+-rw-r--r--   0        0        0    48001 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/939.973bc21fa6263dbabd09.js.map
+-rw-r--r--   0        0        0    27211 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/974.5f4a862a240a7368a2b5.js
+-rw-r--r--   0        0        0    46914 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/974.5f4a862a240a7368a2b5.js.map
+-rw-r--r--   0        0        0    10966 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/remoteEntry.fd0c0fecc472143c1077.js
+-rw-r--r--   0        0        0    45496 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/remoteEntry.fd0c0fecc472143c1077.js.map
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/style.js
+-rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/patches/@jupyterlab+codeeditor+3.6.3.patch
+-rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/scripts/bump-version.py
+-rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/package.json
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/tsconfig.json
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/.bin/rimraf -> ../rimraf/dist/cjs/src/bin.js
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/.bin/tsc -> ../../../../node_modules/typescript/bin/tsc
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/.bin/tsserver -> ../../../../node_modules/typescript/bin/tsserver
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/brace-expansion/LICENSE
+-rw-r--r--   0        0        0     4252 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/brace-expansion/README.md
+-rw-r--r--   0        0        0     4992 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/brace-expansion/index.js
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/brace-expansion/package.json
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/brace-expansion/.github/FUNDING.yml
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/LICENSE
+-rw-r--r--   0        0        0    39545 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/README.md
+-rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/package.json
+-rw-r--r--   0        0        0    12284 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/cjs/glob.d.ts
+-rw-r--r--   0        0        0     3763 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/cjs/glob.d.ts.map
+-rw-r--r--   0        0        0     7550 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/cjs/glob.js
+-rw-r--r--   0        0        0     6560 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/cjs/glob.js.map
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/cjs/has-magic.d.ts
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/cjs/has-magic.d.ts.map
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/cjs/has-magic.js
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/cjs/has-magic.js.map
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/cjs/ignore.d.ts
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/cjs/ignore.d.ts.map
+-rw-r--r--   0        0        0     3791 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/cjs/ignore.js
+-rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/cjs/ignore.js.map
+-rw-r--r--   0        0        0     4357 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/cjs/index-cjs.d.ts
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/cjs/index-cjs.d.ts.map
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/cjs/index-cjs.js
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/cjs/index-cjs.js.map
+-rw-r--r--   0        0        0     6045 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/cjs/index.d.ts
+-rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/cjs/index.d.ts.map
+-rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/cjs/index.js
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/cjs/index.js.map
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/cjs/package.json
+-rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/cjs/pattern.d.ts
+-rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/cjs/pattern.d.ts.map
+-rw-r--r--   0        0        0     7298 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/cjs/pattern.js
+-rw-r--r--   0        0        0     5949 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/cjs/pattern.js.map
+-rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/cjs/processor.d.ts
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/cjs/processor.d.ts.map
+-rw-r--r--   0        0        0    10937 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/cjs/processor.js
+-rw-r--r--   0        0        0     8994 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/cjs/processor.js.map
+-rw-r--r--   0        0        0     4190 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/cjs/walker.d.ts
+-rw-r--r--   0        0        0     4571 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/cjs/walker.d.ts.map
+-rw-r--r--   0        0        0    11900 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/cjs/walker.js
+-rw-r--r--   0        0        0    12084 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/cjs/walker.js.map
+-rw-r--r--   0        0        0    12284 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/mjs/glob.d.ts
+-rw-r--r--   0        0        0     3763 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/mjs/glob.d.ts.map
+-rw-r--r--   0        0        0     7353 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/mjs/glob.js
+-rw-r--r--   0        0        0     6719 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/mjs/glob.js.map
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/mjs/has-magic.d.ts
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/mjs/has-magic.d.ts.map
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/mjs/has-magic.js
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/mjs/has-magic.js.map
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/mjs/ignore.d.ts
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/mjs/ignore.d.ts.map
+-rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/mjs/ignore.js
+-rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/mjs/ignore.js.map
+-rw-r--r--   0        0        0     6045 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/mjs/index.d.ts
+-rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/mjs/index.d.ts.map
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/mjs/index.js
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/mjs/index.js.map
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/mjs/package.json
+-rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/mjs/pattern.d.ts
+-rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/mjs/pattern.d.ts.map
+-rw-r--r--   0        0        0     7159 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/mjs/pattern.js
+-rw-r--r--   0        0        0     5965 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/mjs/pattern.js.map
+-rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/mjs/processor.d.ts
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/mjs/processor.d.ts.map
+-rw-r--r--   0        0        0    10630 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/mjs/processor.js
+-rw-r--r--   0        0        0     8987 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/mjs/processor.js.map
+-rw-r--r--   0        0        0     4190 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/mjs/walker.d.ts
+-rw-r--r--   0        0        0     4571 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/mjs/walker.d.ts.map
+-rw-r--r--   0        0        0    11441 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/mjs/walker.js
+-rw-r--r--   0        0        0    12125 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/mjs/walker.js.map
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minimatch/LICENSE
+-rw-r--r--   0        0        0    17061 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minimatch/README.md
+-rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minimatch/package.json
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minimatch/dist/cjs/brace-expressions.d.ts
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minimatch/dist/cjs/brace-expressions.d.ts.map
+-rw-r--r--   0        0        0     5763 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minimatch/dist/cjs/brace-expressions.js
+-rw-r--r--   0        0        0     4882 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minimatch/dist/cjs/brace-expressions.js.map
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minimatch/dist/cjs/escape.d.ts
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minimatch/dist/cjs/escape.d.ts.map
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minimatch/dist/cjs/escape.js
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minimatch/dist/cjs/escape.js.map
+-rw-r--r--   0        0        0     3176 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minimatch/dist/cjs/index-cjs.d.ts
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minimatch/dist/cjs/index-cjs.d.ts.map
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minimatch/dist/cjs/index-cjs.js
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minimatch/dist/cjs/index-cjs.js.map
+-rw-r--r--   0        0        0     3784 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minimatch/dist/cjs/index.d.ts
+-rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minimatch/dist/cjs/index.d.ts.map
+-rw-r--r--   0        0        0    52207 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minimatch/dist/cjs/index.js
+-rw-r--r--   0        0        0    42018 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minimatch/dist/cjs/index.js.map
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minimatch/dist/cjs/package.json
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minimatch/dist/cjs/unescape.d.ts
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minimatch/dist/cjs/unescape.d.ts.map
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minimatch/dist/cjs/unescape.js
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minimatch/dist/cjs/unescape.js.map
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minimatch/dist/mjs/brace-expressions.d.ts
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minimatch/dist/mjs/brace-expressions.d.ts.map
+-rw-r--r--   0        0        0     5631 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minimatch/dist/mjs/brace-expressions.js
+-rw-r--r--   0        0        0     4866 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minimatch/dist/mjs/brace-expressions.js.map
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minimatch/dist/mjs/escape.d.ts
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minimatch/dist/mjs/escape.d.ts.map
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minimatch/dist/mjs/escape.js
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minimatch/dist/mjs/escape.js.map
+-rw-r--r--   0        0        0     3784 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minimatch/dist/mjs/index.d.ts
+-rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minimatch/dist/mjs/index.d.ts.map
+-rw-r--r--   0        0        0    50982 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minimatch/dist/mjs/index.js
+-rw-r--r--   0        0        0    42020 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minimatch/dist/mjs/index.js.map
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minimatch/dist/mjs/package.json
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minimatch/dist/mjs/unescape.d.ts
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minimatch/dist/mjs/unescape.d.ts.map
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minimatch/dist/mjs/unescape.js
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minimatch/dist/mjs/unescape.js.map
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minipass/LICENSE
+-rw-r--r--   0        0        0    25522 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minipass/README.md
+-rw-r--r--   0        0        0     4245 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minipass/index.d.ts
+-rw-r--r--   0        0        0    18549 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minipass/index.js
+-rw-r--r--   0        0        0    18532 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minipass/index.mjs
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minipass/package.json
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/LICENSE
+-rw-r--r--   0        0        0     8564 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/README.md
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/package.json
+-rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/package.json
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/bin.d.ts
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/bin.d.ts.map
+-rwxr-xr-x   0        0        0     8928 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/bin.js
+-rw-r--r--   0        0        0     6527 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/bin.js.map
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/default-tmp.d.ts
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/default-tmp.d.ts.map
+-rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/default-tmp.js
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/default-tmp.js.map
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/fix-eperm.d.ts
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/fix-eperm.d.ts.map
+-rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/fix-eperm.js
+-rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/fix-eperm.js.map
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/fs.d.ts
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/fs.d.ts.map
+-rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/fs.js
+-rw-r--r--   0        0        0     3180 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/fs.js.map
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/ignore-enoent.d.ts
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/ignore-enoent.d.ts.map
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/ignore-enoent.js
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/ignore-enoent.js.map
+-rw-r--r--   0        0        0     4885 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/index-cjs.d.ts
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/index-cjs.d.ts.map
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/index-cjs.js
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/index-cjs.js.map
+-rw-r--r--   0        0        0     4150 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/index.d.ts
+-rw-r--r--   0        0        0     3313 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/index.d.ts.map
+-rw-r--r--   0        0        0     4605 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/index.js
+-rw-r--r--   0        0        0     3938 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/index.js.map
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/opt-arg.d.ts
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/opt-arg.d.ts.map
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/opt-arg.js
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/opt-arg.js.map
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/path-arg.d.ts
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/path-arg.d.ts.map
+-rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/path-arg.js
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/path-arg.js.map
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/platform.d.ts
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/platform.d.ts.map
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/platform.js
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/platform.js.map
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/readdir-or-error.d.ts
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/readdir-or-error.d.ts.map
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/readdir-or-error.js
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/readdir-or-error.js.map
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/retry-busy.d.ts
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/retry-busy.d.ts.map
+-rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/retry-busy.js
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/retry-busy.js.map
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/rimraf-manual.d.ts
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/rimraf-manual.d.ts.map
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/rimraf-manual.js
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/rimraf-manual.js.map
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/rimraf-move-remove.d.ts
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/rimraf-move-remove.d.ts.map
+-rw-r--r--   0        0        0     6655 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/rimraf-move-remove.js
+-rw-r--r--   0        0        0     6167 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/rimraf-move-remove.js.map
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/rimraf-native.d.ts
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/rimraf-native.d.ts.map
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/rimraf-native.js
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/rimraf-native.js.map
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/rimraf-posix.d.ts
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/rimraf-posix.d.ts.map
+-rw-r--r--   0        0        0     4310 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/rimraf-posix.js
+-rw-r--r--   0        0        0     3803 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/rimraf-posix.js.map
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/rimraf-windows.d.ts
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/rimraf-windows.d.ts.map
+-rw-r--r--   0        0        0     6622 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/rimraf-windows.js
+-rw-r--r--   0        0        0     5752 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/rimraf-windows.js.map
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/use-native.d.ts
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/use-native.d.ts.map
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/use-native.js
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/use-native.js.map
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/default-tmp.d.ts
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/default-tmp.d.ts.map
+-rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/default-tmp.js
+-rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/default-tmp.js.map
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/fix-eperm.d.ts
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/fix-eperm.d.ts.map
+-rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/fix-eperm.js
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/fix-eperm.js.map
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/fs.d.ts
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/fs.d.ts.map
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/fs.js
+-rw-r--r--   0        0        0     3151 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/fs.js.map
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/ignore-enoent.d.ts
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/ignore-enoent.d.ts.map
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/ignore-enoent.js
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/ignore-enoent.js.map
+-rw-r--r--   0        0        0     4150 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/index.d.ts
+-rw-r--r--   0        0        0     3310 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/index.d.ts.map
+-rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/index.js
+-rw-r--r--   0        0        0     4171 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/index.js.map
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/opt-arg.d.ts
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/opt-arg.d.ts.map
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/opt-arg.js
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/opt-arg.js.map
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/package.json
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/path-arg.d.ts
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/path-arg.d.ts.map
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/path-arg.js
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/path-arg.js.map
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/platform.d.ts
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/platform.d.ts.map
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/platform.js
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/platform.js.map
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/readdir-or-error.d.ts
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/readdir-or-error.d.ts.map
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/readdir-or-error.js
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/readdir-or-error.js.map
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/retry-busy.d.ts
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/retry-busy.d.ts.map
+-rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/retry-busy.js
+-rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/retry-busy.js.map
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/rimraf-manual.d.ts
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/rimraf-manual.d.ts.map
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/rimraf-manual.js
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/rimraf-manual.js.map
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/rimraf-move-remove.d.ts
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/rimraf-move-remove.d.ts.map
+-rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/rimraf-move-remove.js
+-rw-r--r--   0        0        0     6278 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/rimraf-move-remove.js.map
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/rimraf-native.d.ts
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/rimraf-native.d.ts.map
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/rimraf-native.js
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/rimraf-native.js.map
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/rimraf-posix.d.ts
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/rimraf-posix.d.ts.map
+-rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/rimraf-posix.js
+-rw-r--r--   0        0        0     3882 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/rimraf-posix.js.map
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/rimraf-windows.d.ts
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/rimraf-windows.d.ts.map
+-rw-r--r--   0        0        0     6049 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/rimraf-windows.js
+-rw-r--r--   0        0        0     5904 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/rimraf-windows.js.map
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/use-native.d.ts
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/use-native.d.ts.map
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/use-native.js
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/use-native.js.map
+-rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/src/factory.ts
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/src/index.ts
+-rw-r--r--   0        0        0     7647 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/src/layout.ts
+-rw-r--r--   0        0        0     4896 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/src/manager.ts
+-rw-r--r--   0        0        0     5627 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/src/registry.ts
+-rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/src/token.ts
+-rw-r--r--   0        0        0    16084 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/src/utils.ts
+-rw-r--r--   0        0        0     3753 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/src/widget.ts
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/src/toolbar/generator.tsx
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/src/toolbar/index.ts
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/src/toolbar/toolbox.tsx
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/src/toolbar/utils.ts
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly/style/index.js
+-rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/package.json
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/tsconfig.json
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/webpack.config.js
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/.bin/build-labextension -> ../../../../node_modules/@jupyterlab/builder/lib/build-labextension.js
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/.bin/npm-run-all -> ../../../../node_modules/npm-run-all/bin/npm-run-all/index.js
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/.bin/rimraf -> ../rimraf/dist/cjs/src/bin.js
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/.bin/run-p -> ../../../../node_modules/npm-run-all/bin/run-p/index.js
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/.bin/run-s -> ../../../../node_modules/npm-run-all/bin/run-s/index.js
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/.bin/tsc -> ../../../../node_modules/typescript/bin/tsc
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/.bin/tsserver -> ../../../../node_modules/typescript/bin/tsserver
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/brace-expansion/LICENSE
+-rw-r--r--   0        0        0     4252 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/brace-expansion/README.md
+-rw-r--r--   0        0        0     4992 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/brace-expansion/index.js
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/brace-expansion/package.json
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/brace-expansion/.github/FUNDING.yml
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/LICENSE
+-rw-r--r--   0        0        0    39545 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/README.md
+-rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/package.json
+-rw-r--r--   0        0        0    12284 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/cjs/glob.d.ts
+-rw-r--r--   0        0        0     3763 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/cjs/glob.d.ts.map
+-rw-r--r--   0        0        0     7550 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/cjs/glob.js
+-rw-r--r--   0        0        0     6560 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/cjs/glob.js.map
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/cjs/has-magic.d.ts
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/cjs/has-magic.d.ts.map
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/cjs/has-magic.js
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/cjs/has-magic.js.map
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/cjs/ignore.d.ts
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/cjs/ignore.d.ts.map
+-rw-r--r--   0        0        0     3791 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/cjs/ignore.js
+-rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/cjs/ignore.js.map
+-rw-r--r--   0        0        0     4357 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/cjs/index-cjs.d.ts
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/cjs/index-cjs.d.ts.map
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/cjs/index-cjs.js
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/cjs/index-cjs.js.map
+-rw-r--r--   0        0        0     6045 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/cjs/index.d.ts
+-rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/cjs/index.d.ts.map
+-rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/cjs/index.js
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/cjs/index.js.map
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/cjs/package.json
+-rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/cjs/pattern.d.ts
+-rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/cjs/pattern.d.ts.map
+-rw-r--r--   0        0        0     7298 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/cjs/pattern.js
+-rw-r--r--   0        0        0     5949 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/cjs/pattern.js.map
+-rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/cjs/processor.d.ts
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/cjs/processor.d.ts.map
+-rw-r--r--   0        0        0    10937 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/cjs/processor.js
+-rw-r--r--   0        0        0     8994 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/cjs/processor.js.map
+-rw-r--r--   0        0        0     4190 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/cjs/walker.d.ts
+-rw-r--r--   0        0        0     4571 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/cjs/walker.d.ts.map
+-rw-r--r--   0        0        0    11900 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/cjs/walker.js
+-rw-r--r--   0        0        0    12084 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/cjs/walker.js.map
+-rw-r--r--   0        0        0    12284 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/mjs/glob.d.ts
+-rw-r--r--   0        0        0     3763 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/mjs/glob.d.ts.map
+-rw-r--r--   0        0        0     7353 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/mjs/glob.js
+-rw-r--r--   0        0        0     6719 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/mjs/glob.js.map
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/mjs/has-magic.d.ts
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/mjs/has-magic.d.ts.map
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/mjs/has-magic.js
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/mjs/has-magic.js.map
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/mjs/ignore.d.ts
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/mjs/ignore.d.ts.map
+-rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/mjs/ignore.js
+-rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/mjs/ignore.js.map
+-rw-r--r--   0        0        0     6045 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/mjs/index.d.ts
+-rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/mjs/index.d.ts.map
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/mjs/index.js
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/mjs/index.js.map
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/mjs/package.json
+-rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/mjs/pattern.d.ts
+-rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/mjs/pattern.d.ts.map
+-rw-r--r--   0        0        0     7159 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/mjs/pattern.js
+-rw-r--r--   0        0        0     5965 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/mjs/pattern.js.map
+-rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/mjs/processor.d.ts
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/mjs/processor.d.ts.map
+-rw-r--r--   0        0        0    10630 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/mjs/processor.js
+-rw-r--r--   0        0        0     8987 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/mjs/processor.js.map
+-rw-r--r--   0        0        0     4190 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/mjs/walker.d.ts
+-rw-r--r--   0        0        0     4571 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/mjs/walker.d.ts.map
+-rw-r--r--   0        0        0    11441 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/mjs/walker.js
+-rw-r--r--   0        0        0    12125 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/mjs/walker.js.map
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minimatch/LICENSE
+-rw-r--r--   0        0        0    17061 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minimatch/README.md
+-rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minimatch/package.json
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minimatch/dist/cjs/brace-expressions.d.ts
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minimatch/dist/cjs/brace-expressions.d.ts.map
+-rw-r--r--   0        0        0     5763 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minimatch/dist/cjs/brace-expressions.js
+-rw-r--r--   0        0        0     4882 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minimatch/dist/cjs/brace-expressions.js.map
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minimatch/dist/cjs/escape.d.ts
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minimatch/dist/cjs/escape.d.ts.map
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minimatch/dist/cjs/escape.js
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minimatch/dist/cjs/escape.js.map
+-rw-r--r--   0        0        0     3176 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minimatch/dist/cjs/index-cjs.d.ts
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minimatch/dist/cjs/index-cjs.d.ts.map
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minimatch/dist/cjs/index-cjs.js
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minimatch/dist/cjs/index-cjs.js.map
+-rw-r--r--   0        0        0     3784 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minimatch/dist/cjs/index.d.ts
+-rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minimatch/dist/cjs/index.d.ts.map
+-rw-r--r--   0        0        0    52207 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minimatch/dist/cjs/index.js
+-rw-r--r--   0        0        0    42018 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minimatch/dist/cjs/index.js.map
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minimatch/dist/cjs/package.json
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minimatch/dist/cjs/unescape.d.ts
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minimatch/dist/cjs/unescape.d.ts.map
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minimatch/dist/cjs/unescape.js
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minimatch/dist/cjs/unescape.js.map
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minimatch/dist/mjs/brace-expressions.d.ts
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minimatch/dist/mjs/brace-expressions.d.ts.map
+-rw-r--r--   0        0        0     5631 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minimatch/dist/mjs/brace-expressions.js
+-rw-r--r--   0        0        0     4866 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minimatch/dist/mjs/brace-expressions.js.map
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minimatch/dist/mjs/escape.d.ts
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minimatch/dist/mjs/escape.d.ts.map
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minimatch/dist/mjs/escape.js
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minimatch/dist/mjs/escape.js.map
+-rw-r--r--   0        0        0     3784 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minimatch/dist/mjs/index.d.ts
+-rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minimatch/dist/mjs/index.d.ts.map
+-rw-r--r--   0        0        0    50982 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minimatch/dist/mjs/index.js
+-rw-r--r--   0        0        0    42020 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minimatch/dist/mjs/index.js.map
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minimatch/dist/mjs/package.json
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minimatch/dist/mjs/unescape.d.ts
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minimatch/dist/mjs/unescape.d.ts.map
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minimatch/dist/mjs/unescape.js
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minimatch/dist/mjs/unescape.js.map
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minipass/LICENSE
+-rw-r--r--   0        0        0    25522 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minipass/README.md
+-rw-r--r--   0        0        0     4245 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minipass/index.d.ts
+-rw-r--r--   0        0        0    18549 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minipass/index.js
+-rw-r--r--   0        0        0    18532 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minipass/index.mjs
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minipass/package.json
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/LICENSE
+-rw-r--r--   0        0        0     8564 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/README.md
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/package.json
+-rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/package.json
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/bin.d.ts
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/bin.d.ts.map
+-rwxr-xr-x   0        0        0     8928 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/bin.js
+-rw-r--r--   0        0        0     6527 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/bin.js.map
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/default-tmp.d.ts
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/default-tmp.d.ts.map
+-rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/default-tmp.js
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/default-tmp.js.map
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/fix-eperm.d.ts
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/fix-eperm.d.ts.map
+-rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/fix-eperm.js
+-rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/fix-eperm.js.map
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/fs.d.ts
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/fs.d.ts.map
+-rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/fs.js
+-rw-r--r--   0        0        0     3180 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/fs.js.map
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/ignore-enoent.d.ts
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/ignore-enoent.d.ts.map
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/ignore-enoent.js
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/ignore-enoent.js.map
+-rw-r--r--   0        0        0     4885 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/index-cjs.d.ts
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/index-cjs.d.ts.map
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/index-cjs.js
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/index-cjs.js.map
+-rw-r--r--   0        0        0     4150 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/index.d.ts
+-rw-r--r--   0        0        0     3313 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/index.d.ts.map
+-rw-r--r--   0        0        0     4605 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/index.js
+-rw-r--r--   0        0        0     3938 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/index.js.map
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/opt-arg.d.ts
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/opt-arg.d.ts.map
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/opt-arg.js
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/opt-arg.js.map
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/path-arg.d.ts
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/path-arg.d.ts.map
+-rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/path-arg.js
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/path-arg.js.map
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/platform.d.ts
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/platform.d.ts.map
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/platform.js
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/platform.js.map
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/readdir-or-error.d.ts
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/readdir-or-error.d.ts.map
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/readdir-or-error.js
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/readdir-or-error.js.map
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/retry-busy.d.ts
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/retry-busy.d.ts.map
+-rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/retry-busy.js
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/retry-busy.js.map
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/rimraf-manual.d.ts
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/rimraf-manual.d.ts.map
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/rimraf-manual.js
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/rimraf-manual.js.map
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/rimraf-move-remove.d.ts
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/rimraf-move-remove.d.ts.map
+-rw-r--r--   0        0        0     6655 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/rimraf-move-remove.js
+-rw-r--r--   0        0        0     6167 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/rimraf-move-remove.js.map
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/rimraf-native.d.ts
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/rimraf-native.d.ts.map
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/rimraf-native.js
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/rimraf-native.js.map
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/rimraf-posix.d.ts
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/rimraf-posix.d.ts.map
+-rw-r--r--   0        0        0     4310 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/rimraf-posix.js
+-rw-r--r--   0        0        0     3803 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/rimraf-posix.js.map
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/rimraf-windows.d.ts
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/rimraf-windows.d.ts.map
+-rw-r--r--   0        0        0     6622 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/rimraf-windows.js
+-rw-r--r--   0        0        0     5752 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/rimraf-windows.js.map
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/use-native.d.ts
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/use-native.d.ts.map
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/use-native.js
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/use-native.js.map
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/default-tmp.d.ts
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/default-tmp.d.ts.map
+-rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/default-tmp.js
+-rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/default-tmp.js.map
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/fix-eperm.d.ts
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/fix-eperm.d.ts.map
+-rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/fix-eperm.js
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/fix-eperm.js.map
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/fs.d.ts
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/fs.d.ts.map
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/fs.js
+-rw-r--r--   0        0        0     3151 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/fs.js.map
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/ignore-enoent.d.ts
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/ignore-enoent.d.ts.map
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/ignore-enoent.js
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/ignore-enoent.js.map
+-rw-r--r--   0        0        0     4150 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/index.d.ts
+-rw-r--r--   0        0        0     3310 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/index.d.ts.map
+-rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/index.js
+-rw-r--r--   0        0        0     4171 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/index.js.map
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/opt-arg.d.ts
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/opt-arg.d.ts.map
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/opt-arg.js
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/opt-arg.js.map
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/package.json
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/path-arg.d.ts
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/path-arg.d.ts.map
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/path-arg.js
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/path-arg.js.map
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/platform.d.ts
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/platform.d.ts.map
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/platform.js
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/platform.js.map
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/readdir-or-error.d.ts
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/readdir-or-error.d.ts.map
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/readdir-or-error.js
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/readdir-or-error.js.map
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/retry-busy.d.ts
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/retry-busy.d.ts.map
+-rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/retry-busy.js
+-rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/retry-busy.js.map
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/rimraf-manual.d.ts
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/rimraf-manual.d.ts.map
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/rimraf-manual.js
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/rimraf-manual.js.map
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/rimraf-move-remove.d.ts
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/rimraf-move-remove.d.ts.map
+-rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/rimraf-move-remove.js
+-rw-r--r--   0        0        0     6278 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/rimraf-move-remove.js.map
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/rimraf-native.d.ts
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/rimraf-native.d.ts.map
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/rimraf-native.js
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/rimraf-native.js.map
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/rimraf-posix.d.ts
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/rimraf-posix.d.ts.map
+-rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/rimraf-posix.js
+-rw-r--r--   0        0        0     3882 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/rimraf-posix.js.map
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/rimraf-windows.d.ts
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/rimraf-windows.d.ts.map
+-rw-r--r--   0        0        0     6049 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/rimraf-windows.js
+-rw-r--r--   0        0        0     5904 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/rimraf-windows.js.map
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/use-native.d.ts
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/use-native.d.ts.map
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/use-native.js
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/use-native.js.map
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/src/icons.ts
+-rw-r--r--   0        0        0     8833 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/src/index.ts
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/src/svg.d.ts
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/style/index.js
+-rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/packages/blockly-extension/style/icons/blockly_logo.svg
+-rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/.gitignore
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/LICENSE
+-rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/README.md
+-rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/pyproject.toml
+-rw-r--r--   0        0        0     6443 2020-02-02 00:00:00.000000 jupyterlab_blockly-0.3.0a1/PKG-INFO
```

### Comparing `jupyterlab_blockly-0.3.0a0/.eslintrc.js` & `jupyterlab_blockly-0.3.0a1/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/CHANGELOG.md` & `jupyterlab_blockly-0.3.0a1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,27 @@
 # Changelog
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 0.3.0alpha1
+
+([Full Changelog](https://github.com/QuantStack/jupyterlab-blockly/compare/jupyterlab-blockly-extension@0.3.0-alpha.0...32b4140e5e6097dded2dca850eb22291ec87bdab))
+
+### Enhancements made
+
+- Add support for widgets [#73](https://github.com/QuantStack/jupyterlab-blockly/pull/73) ([@hbcarlos](https://github.com/hbcarlos))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/QuantStack/jupyterlab-blockly/graphs/contributors?from=2023-03-15&to=2023-04-17&type=c))
+
+[@github-actions](https://github.com/search?q=repo%3AQuantStack%2Fjupyterlab-blockly+involves%3Agithub-actions+updated%3A2023-03-15..2023-04-17&type=Issues) | [@hbcarlos](https://github.com/search?q=repo%3AQuantStack%2Fjupyterlab-blockly+involves%3Ahbcarlos+updated%3A2023-03-15..2023-04-17&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 0.3.0alpha0
 
 ([Full Changelog](https://github.com/QuantStack/jupyterlab-blockly/compare/jupyterlab-blockly-extension@0.2.1...2f7ca5003863f9b8688b5f3e744ce85d228e6f4c))
 
 ### Maintenance and upkeep improvements
 
 - Updates to JupyterLab 3.6 and fixes check release [#72](https://github.com/QuantStack/jupyterlab-blockly/pull/72) ([@hbcarlos](https://github.com/hbcarlos))
@@ -14,16 +30,14 @@
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/QuantStack/jupyterlab-blockly/graphs/contributors?from=2022-09-07&to=2023-03-15&type=c))
 
 [@bollwyvl](https://github.com/search?q=repo%3AQuantStack%2Fjupyterlab-blockly+involves%3Abollwyvl+updated%3A2022-09-07..2023-03-15&type=Issues) | [@github-actions](https://github.com/search?q=repo%3AQuantStack%2Fjupyterlab-blockly+involves%3Agithub-actions+updated%3A2022-09-07..2023-03-15&type=Issues) | [@hbcarlos](https://github.com/search?q=repo%3AQuantStack%2Fjupyterlab-blockly+involves%3Ahbcarlos+updated%3A2022-09-07..2023-03-15&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 0.2.1
 
 ([Full Changelog](https://github.com/QuantStack/jupyterlab-blockly/compare/jupyterlab-blockly-extension@0.2.0...bd41065fbfe8712ad75fad0b2df6be7c9e887c4f))
 
 ### Bugs fixed
 
 - Fixes the scroll behavior of the code cell [#68](https://github.com/QuantStack/jupyterlab-blockly/pull/68) ([@hbcarlos](https://github.com/hbcarlos))
```

### Comparing `jupyterlab_blockly-0.3.0a0/RELEASE.md` & `jupyterlab_blockly-0.3.0a1/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/package.json` & `jupyterlab_blockly-0.3.0a1/package.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9615384615384616%*

 * *Differences: {"'version'": "'0.3.0-alpha.1'"}*

```diff
@@ -46,14 +46,14 @@
         "lint:check": "jlpm prettier:check && jlpm eslint:check",
         "postinstall": "patch-package",
         "prettier": "jlpm prettier:base --write --list-different",
         "prettier:base": "prettier \"**/*{.ts,.tsx,.js,.jsx,.css}\"",
         "prettier:check": "jlpm prettier:base --check",
         "watch": "lerna run --stream watch"
     },
-    "version": "0.3.0-alpha.0",
+    "version": "0.3.0-alpha.1",
     "workspaces": {
         "packages": [
             "packages/*"
         ]
     }
 }
```

### Comparing `jupyterlab_blockly-0.3.0a0/yarn.lock` & `jupyterlab_blockly-0.3.0a1/yarn.lock`

 * *Files 4% similar despite different names*

```diff
@@ -195,110 +195,190 @@
     "@jridgewell/sourcemap-codec" "1.4.14"
 
 "@juggle/resize-observer@^3.3.1":
   version "3.4.0"
   resolved "https://registry.yarnpkg.com/@juggle/resize-observer/-/resize-observer-3.4.0.tgz#08d6c5e20cf7e4cc02fd181c4b0c225cd31dbb60"
   integrity sha512-dfLbk+PwWvFzSxwk3n5ySL0hfBog779o8h68wK/7/APo/7cgyWp5jcXockbxdk5kFRkbeXWm4Fbi9FrdN381sA==
 
-"@jupyter/ydoc@~0.2.0":
-  version "0.2.3"
-  resolved "https://registry.yarnpkg.com/@jupyter/ydoc/-/ydoc-0.2.3.tgz#468a88d0250c5d59800a5cc15a33df211b4b2141"
-  integrity sha512-mwmlzOYXr4StXL1ijrSkt6+Bu4cF5nZQAep2zULa5IDe/PVDBqDtMrLqZyKQOgB3IT/sLJidU1P3wTdb8bwmww==
+"@jupyter-widgets/base-manager@^1.0.5":
+  version "1.0.5"
+  resolved "https://registry.yarnpkg.com/@jupyter-widgets/base-manager/-/base-manager-1.0.5.tgz#c580806fbb83c4e9ad164948b8a58369a301ae6b"
+  integrity sha512-+pagXIXBbSq1NdqaJ8xJj52SF3t0zyUofDHVZ1bFrfWIhl5qZuLxtD16PvnqO+n1gIPLlW238Og6QuIGKOKkZQ==
+  dependencies:
+    "@jupyter-widgets/base" "^6.0.4"
+    "@jupyterlab/services" "^6.0.0"
+    "@lumino/coreutils" "^1.11.1"
+    base64-js "^1.2.1"
+    sanitize-html "^2.3"
+
+"@jupyter-widgets/base@^6.0.4":
+  version "6.0.4"
+  resolved "https://registry.yarnpkg.com/@jupyter-widgets/base/-/base-6.0.4.tgz#6348b29f3574df4f0a7df593b4088529f46be57a"
+  integrity sha512-w5KUL8q44Isp0N/ElOAJbPSgWBdeGZO5EYEcz50rfqYAUMSh2Qx0oQJYMddbRgi8b5CajGHFvcHTfvwaNDLSmA==
+  dependencies:
+    "@jupyterlab/services" "^6.0.0"
+    "@lumino/coreutils" "^1.11.1"
+    "@lumino/messaging" "^1.10.1"
+    "@lumino/widgets" "^1.30.0"
+    "@types/backbone" "1.4.14"
+    "@types/lodash" "^4.14.134"
+    backbone "1.4.0"
+    jquery "^3.1.1"
+    lodash "^4.17.4"
+
+"@jupyter-widgets/controls@^5.0.5":
+  version "5.0.5"
+  resolved "https://registry.yarnpkg.com/@jupyter-widgets/controls/-/controls-5.0.5.tgz#076b75a0c04a946a5bd8fd1d3401f428dbe673f3"
+  integrity sha512-Y6NvKdE1Pkp/3tS/gJUIv1fxmRkCrbWx8SLDxA29QJrEriC/Kpjoq4qMBtL6JwS+UNcouLuX+jfhBtaDw8d5Xw==
+  dependencies:
+    "@jupyter-widgets/base" "^6.0.4"
+    "@lumino/algorithm" "^1.9.1"
+    "@lumino/domutils" "^1.8.1"
+    "@lumino/messaging" "^1.10.1"
+    "@lumino/signaling" "^1.10.1"
+    "@lumino/widgets" "^1.30.0"
+    d3-color "^3.0.1"
+    d3-format "^3.0.1"
+    jquery "^3.1.1"
+    nouislider "15.4.0"
+
+"@jupyter-widgets/jupyterlab-manager@^5.0.7":
+  version "5.0.7"
+  resolved "https://registry.yarnpkg.com/@jupyter-widgets/jupyterlab-manager/-/jupyterlab-manager-5.0.7.tgz#5813fc5087823eae5af76a7af1fc6ba03092777e"
+  integrity sha512-+kCuf9IiTfFCY9iUrCoxKXID0eI45Ovom1gsgRbHlckInhhn4raB2YDEL0lgy/G9Bj+qXMZoih9VKds7KrWIrw==
+  dependencies:
+    "@jupyter-widgets/base" "^6.0.4"
+    "@jupyter-widgets/base-manager" "^1.0.5"
+    "@jupyter-widgets/controls" "^5.0.5"
+    "@jupyter-widgets/output" "^6.0.4"
+    "@jupyterlab/application" "^3.0.0"
+    "@jupyterlab/docregistry" "^3.0.0"
+    "@jupyterlab/logconsole" "^3.0.0"
+    "@jupyterlab/mainmenu" "^3.0.0"
+    "@jupyterlab/nbformat" "^3.0.0"
+    "@jupyterlab/notebook" "^3.0.0"
+    "@jupyterlab/outputarea" "^3.0.0"
+    "@jupyterlab/rendermime" "^3.0.0"
+    "@jupyterlab/rendermime-interfaces" "^3.0.0"
+    "@jupyterlab/services" "^6.0.0"
+    "@jupyterlab/settingregistry" "^3.0.0"
+    "@jupyterlab/translation" "^3.0.0"
+    "@lumino/algorithm" "^1.9.1"
+    "@lumino/coreutils" "^1.11.1"
+    "@lumino/disposable" "^1.10.1"
+    "@lumino/properties" "^1.8.1"
+    "@lumino/signaling" "^1.10.1"
+    "@lumino/widgets" "^1.30.0"
+    "@types/backbone" "1.4.14"
+    jquery "^3.1.1"
+    semver "^7.3.5"
+
+"@jupyter-widgets/output@^6.0.4":
+  version "6.0.4"
+  resolved "https://registry.yarnpkg.com/@jupyter-widgets/output/-/output-6.0.4.tgz#991d1a1b904a28daa3fd74f0d148455b9e475623"
+  integrity sha512-wwh/RjYNcP1dQsd4HcMYlRx+hlIAOJ2cnG/iQY+e34Fm90kzIElm9gNL8eRzHFmT3psg6c6zW9cIvg+q6Gd3ag==
+  dependencies:
+    "@jupyter-widgets/base" "^6.0.4"
+
+"@jupyter/ydoc@~0.2.3":
+  version "0.2.4"
+  resolved "https://registry.yarnpkg.com/@jupyter/ydoc/-/ydoc-0.2.4.tgz#bc312f171777b58e286aadca62dadeca3a894dd1"
+  integrity sha512-QACcB4bF+Ew4UJmJP+3OyiyQm3vwRYF6iZCQK9q0nE2U5uAosQkfLyT6Bx71jPUXe4G9lEF6m9fjpZvSUX7Lyw==
   dependencies:
     "@jupyterlab/nbformat" "^3.0.0 || ^4.0.0-alpha.15"
     "@lumino/coreutils" "^1.11.0 || ^2.0.0-alpha.6"
     "@lumino/disposable" "^1.10.0 || ^2.0.0-alpha.6"
     "@lumino/signaling" "^1.10.0 || ^2.0.0-alpha.6"
     y-protocols "^1.0.5"
     yjs "^13.5.40"
 
-"@jupyterlab/application@^3.6":
-  version "3.6.1"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/application/-/application-3.6.1.tgz#41b897a809847fcd9426fe12ab0415c4373d24ed"
-  integrity sha512-EpZ5pByXqiNwX9Kj6H5UepYJ9nNI3uU0ule7vCHhLmvJTM9+ARUKT9a52qp2uAyZSjdihl1cHfVKONEM9Xn8fA==
+"@jupyterlab/application@^3.0.0", "@jupyterlab/application@^3.6":
+  version "3.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/application/-/application-3.6.3.tgz#7e199f77a4536bc7429fbecf9ba1850f51d9de52"
+  integrity sha512-G0tR6sUSCuHB8vGQnaB5lfihKNJVHtqYNoMlsZYF9rYpZEhW1TRD4uE5rg4RfDDR+GghjckQlP3rRNB2Vn4tMA==
   dependencies:
     "@fortawesome/fontawesome-free" "^5.12.0"
-    "@jupyterlab/apputils" "^3.6.1"
-    "@jupyterlab/coreutils" "^5.6.1"
-    "@jupyterlab/docregistry" "^3.6.1"
-    "@jupyterlab/rendermime" "^3.6.1"
-    "@jupyterlab/rendermime-interfaces" "^3.6.1"
-    "@jupyterlab/services" "^6.6.1"
-    "@jupyterlab/statedb" "^3.6.1"
-    "@jupyterlab/translation" "^3.6.1"
-    "@jupyterlab/ui-components" "^3.6.1"
+    "@jupyterlab/apputils" "^3.6.3"
+    "@jupyterlab/coreutils" "^5.6.3"
+    "@jupyterlab/docregistry" "^3.6.3"
+    "@jupyterlab/rendermime" "^3.6.3"
+    "@jupyterlab/rendermime-interfaces" "^3.6.3"
+    "@jupyterlab/services" "^6.6.3"
+    "@jupyterlab/statedb" "^3.6.3"
+    "@jupyterlab/translation" "^3.6.3"
+    "@jupyterlab/ui-components" "^3.6.3"
     "@lumino/algorithm" "^1.9.0"
-    "@lumino/application" "^1.31.3"
+    "@lumino/application" "^1.31.4"
     "@lumino/commands" "^1.19.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/messaging" "^1.10.0"
     "@lumino/polling" "^1.9.0"
     "@lumino/properties" "^1.8.0"
     "@lumino/signaling" "^1.10.0"
-    "@lumino/widgets" "^1.37.1"
+    "@lumino/widgets" "^1.37.2"
 
-"@jupyterlab/apputils@^3.6", "@jupyterlab/apputils@^3.6.1":
-  version "3.6.1"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/apputils/-/apputils-3.6.1.tgz#c547886300e67c5eea0b9ee349e6e1acb0576e64"
-  integrity sha512-/kvncjPLuBnq8unPEVxI/iwUVCVPFw9bmpnYenOdoAlbdrDD8nJwsiFi4xpk1d4VittPZ6vJaAMvXA0X2QGYlQ==
-  dependencies:
-    "@jupyterlab/coreutils" "^5.6.1"
-    "@jupyterlab/observables" "^4.6.1"
-    "@jupyterlab/services" "^6.6.1"
-    "@jupyterlab/settingregistry" "^3.6.1"
-    "@jupyterlab/statedb" "^3.6.1"
-    "@jupyterlab/translation" "^3.6.1"
-    "@jupyterlab/ui-components" "^3.6.1"
+"@jupyterlab/apputils@^3.6", "@jupyterlab/apputils@^3.6.3":
+  version "3.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/apputils/-/apputils-3.6.3.tgz#bc37683142b281e21d22a2f4698634563658298e"
+  integrity sha512-um2Aaa5fOUwHFpAqKTDA+MFpnAldzOILIi5QsKOWRxiJA2W8x+hlg5HvHbq+eSWuWEU3ah15M7htzBcL3g9d4Q==
+  dependencies:
+    "@jupyterlab/coreutils" "^5.6.3"
+    "@jupyterlab/observables" "^4.6.3"
+    "@jupyterlab/services" "^6.6.3"
+    "@jupyterlab/settingregistry" "^3.6.3"
+    "@jupyterlab/statedb" "^3.6.3"
+    "@jupyterlab/translation" "^3.6.3"
+    "@jupyterlab/ui-components" "^3.6.3"
     "@lumino/algorithm" "^1.9.0"
     "@lumino/commands" "^1.19.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/domutils" "^1.8.0"
     "@lumino/messaging" "^1.10.0"
     "@lumino/polling" "^1.9.0"
     "@lumino/properties" "^1.8.0"
     "@lumino/signaling" "^1.10.0"
     "@lumino/virtualdom" "^1.14.0"
-    "@lumino/widgets" "^1.37.1"
+    "@lumino/widgets" "^1.37.2"
     "@types/react" "^17.0.0"
     react "^17.0.1"
     react-dom "^17.0.1"
     sanitize-html "~2.7.3"
     url "^0.11.0"
 
-"@jupyterlab/attachments@^3.6.1":
-  version "3.6.1"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/attachments/-/attachments-3.6.1.tgz#af3b3baa0f4150d412a874121b15029e9761c3a8"
-  integrity sha512-0RA8H0pR3apvqHmkzuFJcJrNXXVDa5GG2Y2Nb5QDtOj+IFRMxEa/8Q4rXtiC7p+fDIgKC/B8xa4CTQlfDCEjaw==
-  dependencies:
-    "@jupyterlab/nbformat" "^3.6.1"
-    "@jupyterlab/observables" "^4.6.1"
-    "@jupyterlab/rendermime" "^3.6.1"
-    "@jupyterlab/rendermime-interfaces" "^3.6.1"
+"@jupyterlab/attachments@^3.6.3":
+  version "3.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/attachments/-/attachments-3.6.3.tgz#f2e52c3518d3f84cb7a7cc7c8a113f49dfdde4f1"
+  integrity sha512-ZYDJjcoExmojsGkX5f1WVFfW39XJcb7CtfzFcNz3AbytebRK13S1xqCRlef/TFW+XT6BG7hjMSJlpW3GdkCV1Q==
+  dependencies:
+    "@jupyterlab/nbformat" "^3.6.3"
+    "@jupyterlab/observables" "^4.6.3"
+    "@jupyterlab/rendermime" "^3.6.3"
+    "@jupyterlab/rendermime-interfaces" "^3.6.3"
     "@lumino/disposable" "^1.10.0"
     "@lumino/signaling" "^1.10.0"
 
 "@jupyterlab/builder@^3.6":
-  version "3.6.1"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/builder/-/builder-3.6.1.tgz#a04bf0312e8679d1f452c27fee2554ba4a6af3f5"
-  integrity sha512-LvHQe6InEXJisEcvAdvSFbEEl8OhTjxBSNz7MrjRB+Ur+Qs898dg8QhDH9Ad5mgK3uh4nEN1BDq9W7C/NomqoA==
+  version "3.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/builder/-/builder-3.6.3.tgz#a4b22efe34e9598b84122ff10509d3d890017b6a"
+  integrity sha512-oY1a/r75RMoPzhSmuVu+DfjL0cKk1ceHTniZsM2wPuhjjyoF875u6CDzArJatpOOuTgLm7CY5OcU3LCIK1OAgg==
   dependencies:
     "@lumino/algorithm" "^1.9.0"
-    "@lumino/application" "^1.31.3"
+    "@lumino/application" "^1.31.4"
     "@lumino/commands" "^1.19.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/domutils" "^1.8.0"
     "@lumino/dragdrop" "^1.13.0"
     "@lumino/messaging" "^1.10.0"
     "@lumino/properties" "^1.8.0"
     "@lumino/signaling" "^1.10.0"
     "@lumino/virtualdom" "^1.14.0"
-    "@lumino/widgets" "^1.37.1"
+    "@lumino/widgets" "^1.37.2"
     ajv "^6.12.3"
     commander "~6.0.0"
     css-loader "^5.0.1"
     duplicate-package-checker-webpack-plugin "^3.0.0"
     file-loader "~6.0.0"
     fs-extra "^9.0.1"
     glob "~7.1.6"
@@ -315,371 +395,419 @@
     to-string-loader "^1.1.6"
     url-loader "~4.1.0"
     webpack "^5.41.1"
     webpack-cli "^4.1.0"
     webpack-merge "^5.1.2"
     worker-loader "^3.0.2"
 
-"@jupyterlab/cells@^3.6":
-  version "3.6.1"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/cells/-/cells-3.6.1.tgz#84c4a43cb66e94a934bcf25172b6ded64d87bba6"
-  integrity sha512-Ojep4Sw83c4uzYSDMQcECW7wuan/dkerimKkb/5cm277ryHL51IgjZTEpJKaW8AeEjNxtAwjlo4cl/5KIwKvQw==
-  dependencies:
-    "@jupyter/ydoc" "~0.2.0"
-    "@jupyterlab/apputils" "^3.6.1"
-    "@jupyterlab/attachments" "^3.6.1"
-    "@jupyterlab/codeeditor" "^3.6.1"
-    "@jupyterlab/codemirror" "^3.6.1"
-    "@jupyterlab/coreutils" "^5.6.1"
-    "@jupyterlab/filebrowser" "^3.6.1"
-    "@jupyterlab/nbformat" "^3.6.1"
-    "@jupyterlab/observables" "^4.6.1"
-    "@jupyterlab/outputarea" "^3.6.1"
-    "@jupyterlab/rendermime" "^3.6.1"
-    "@jupyterlab/services" "^6.6.1"
-    "@jupyterlab/ui-components" "^3.6.1"
+"@jupyterlab/cells@^3.6", "@jupyterlab/cells@^3.6.3":
+  version "3.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/cells/-/cells-3.6.3.tgz#ac8191f99923a004211725435d25280347794cff"
+  integrity sha512-o3Uydof6bZ6HGSRgSm6isuAhaqYVmv+ozsmADYNmIGbwwwC+eb391Cv+rC3kuPZX/+2UhhO6s7fqFxW8aHUDkg==
+  dependencies:
+    "@jupyter/ydoc" "~0.2.3"
+    "@jupyterlab/apputils" "^3.6.3"
+    "@jupyterlab/attachments" "^3.6.3"
+    "@jupyterlab/codeeditor" "^3.6.3"
+    "@jupyterlab/codemirror" "^3.6.3"
+    "@jupyterlab/coreutils" "^5.6.3"
+    "@jupyterlab/filebrowser" "^3.6.3"
+    "@jupyterlab/nbformat" "^3.6.3"
+    "@jupyterlab/observables" "^4.6.3"
+    "@jupyterlab/outputarea" "^3.6.3"
+    "@jupyterlab/rendermime" "^3.6.3"
+    "@jupyterlab/services" "^6.6.3"
+    "@jupyterlab/ui-components" "^3.6.3"
     "@lumino/algorithm" "^1.9.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/domutils" "^1.8.0"
     "@lumino/dragdrop" "^1.13.0"
     "@lumino/messaging" "^1.10.0"
     "@lumino/polling" "^1.9.0"
     "@lumino/signaling" "^1.10.0"
     "@lumino/virtualdom" "^1.14.0"
-    "@lumino/widgets" "^1.37.1"
+    "@lumino/widgets" "^1.37.2"
     marked "^4.0.17"
     react "^17.0.1"
 
-"@jupyterlab/codeeditor@^3.6", "@jupyterlab/codeeditor@^3.6.1":
-  version "3.6.1"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/codeeditor/-/codeeditor-3.6.1.tgz#9643e9f4f594f6cc3f02a2d5a192d8e2bc844284"
-  integrity sha512-KIALB/PHY9LheZ0zGYMHnDGVUO5xReiG+u0Gb+658xYET148a/pU4kp47GzTYB2bsQRrmOmtMqda1/Nhn/c0xw==
-  dependencies:
-    "@jupyter/ydoc" "~0.2.0"
-    "@jupyterlab/coreutils" "^5.6.1"
-    "@jupyterlab/nbformat" "^3.6.1"
-    "@jupyterlab/observables" "^4.6.1"
-    "@jupyterlab/translation" "^3.6.1"
-    "@jupyterlab/ui-components" "^3.6.1"
+"@jupyterlab/codeeditor@^3.6", "@jupyterlab/codeeditor@^3.6.3":
+  version "3.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/codeeditor/-/codeeditor-3.6.3.tgz#a889c1821001888af7b60f66b1ee91e15797c0bb"
+  integrity sha512-SnVo5KDhyRkK/o1SDRX9nehLEAMaOBFf+GUx2jeXBTfr6wTKcwDBnJAUwlOfncwRlMV79aUIqTIcS861FSXDyA==
+  dependencies:
+    "@jupyter/ydoc" "~0.2.3"
+    "@jupyterlab/coreutils" "^5.6.3"
+    "@jupyterlab/nbformat" "^3.6.3"
+    "@jupyterlab/observables" "^4.6.3"
+    "@jupyterlab/translation" "^3.6.3"
+    "@jupyterlab/ui-components" "^3.6.3"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/dragdrop" "^1.13.0"
     "@lumino/messaging" "^1.10.0"
     "@lumino/signaling" "^1.10.0"
-    "@lumino/widgets" "^1.37.1"
+    "@lumino/widgets" "^1.37.2"
 
-"@jupyterlab/codemirror@^3.6.1":
-  version "3.6.1"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/codemirror/-/codemirror-3.6.1.tgz#e21134b02d8ae5b6d971549a689b8462987d30c7"
-  integrity sha512-hEjdAm1bSsBNuzjhnCJrphVdl8HZSGh/+q2MioyF7zRK+VbFarx7DKoYdAtaunHu5MkYA9NGf7mjLVyg17dK9g==
-  dependencies:
-    "@jupyter/ydoc" "~0.2.0"
-    "@jupyterlab/apputils" "^3.6.1"
-    "@jupyterlab/codeeditor" "^3.6.1"
-    "@jupyterlab/coreutils" "^5.6.1"
-    "@jupyterlab/nbformat" "^3.6.1"
-    "@jupyterlab/observables" "^4.6.1"
-    "@jupyterlab/statusbar" "^3.6.1"
-    "@jupyterlab/translation" "^3.6.1"
+"@jupyterlab/codemirror@^3.6.3":
+  version "3.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/codemirror/-/codemirror-3.6.3.tgz#7cb19faae58d4fc26bc37064f029c4b17098c20a"
+  integrity sha512-VU5bInzSqsyPGZkEd/w6HtJ9PSw7U5twoyrQSpSM+E2SEYWskaBZOHJf8XNunVoRRKwSvDLyxSs07Ot6zUlA0w==
+  dependencies:
+    "@jupyter/ydoc" "~0.2.3"
+    "@jupyterlab/apputils" "^3.6.3"
+    "@jupyterlab/codeeditor" "^3.6.3"
+    "@jupyterlab/coreutils" "^5.6.3"
+    "@jupyterlab/nbformat" "^3.6.3"
+    "@jupyterlab/observables" "^4.6.3"
+    "@jupyterlab/statusbar" "^3.6.3"
+    "@jupyterlab/translation" "^3.6.3"
     "@lumino/algorithm" "^1.9.0"
     "@lumino/commands" "^1.19.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/polling" "^1.9.0"
     "@lumino/signaling" "^1.10.0"
-    "@lumino/widgets" "^1.37.1"
+    "@lumino/widgets" "^1.37.2"
     codemirror "~5.61.0"
     react "^17.0.1"
     y-codemirror "^3.0.1"
 
-"@jupyterlab/coreutils@^5.6", "@jupyterlab/coreutils@^5.6.1":
-  version "5.6.1"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/coreutils/-/coreutils-5.6.1.tgz#da6c2fe28298ffcad09f1ec5ad4202bdaf1c07c8"
-  integrity sha512-nS4ixC9H53lFzdszOfZfDhlM2hlXfOtQAn6TnA/0Ra/gTBQ+LEbFIWdAp588iKuv8eKX39O/Us53T4oq24A31g==
+"@jupyterlab/coreutils@^5.6", "@jupyterlab/coreutils@^5.6.3":
+  version "5.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/coreutils/-/coreutils-5.6.3.tgz#3b0b5d481b14596158b560336833c89be509e84e"
+  integrity sha512-jRVTpwGzP9wBNYuaZTip89FS1qbeSYrEO2qdNVdW2rs0mQHcIlu3Fkv5muMFmKYGi0XHhG3UhZiWQ7qiPw2svQ==
   dependencies:
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/signaling" "^1.10.0"
     minimist "~1.2.0"
     moment "^2.24.0"
     path-browserify "^1.0.0"
     url-parse "~1.5.1"
 
-"@jupyterlab/docmanager@^3.6.1":
-  version "3.6.1"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/docmanager/-/docmanager-3.6.1.tgz#2f62aabb9dc3f8007f5f54b61473274f784b1972"
-  integrity sha512-olDFoXq2H6TsnCk4OMJus4PcmXCtc2uewZy66XcLD7igDxKvQ50h9uF2wnrxohlgvXxZV9HTMyDyLD7layt82g==
-  dependencies:
-    "@jupyterlab/apputils" "^3.6.1"
-    "@jupyterlab/coreutils" "^5.6.1"
-    "@jupyterlab/docprovider" "^3.6.1"
-    "@jupyterlab/docregistry" "^3.6.1"
-    "@jupyterlab/services" "^6.6.1"
-    "@jupyterlab/statusbar" "^3.6.1"
-    "@jupyterlab/translation" "^3.6.1"
+"@jupyterlab/docmanager@^3.6.3":
+  version "3.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/docmanager/-/docmanager-3.6.3.tgz#df2c5b45c5e9b38e2a48eb703ff5e3a9b4b7860c"
+  integrity sha512-4d5zGE3SGbg58wsFJtyskUxK7dEvl8d5Wh90hTlmsFNmr+nh5duTWcqTQ/a+d76YxYbGhH5vqOsNm5ORZq4Umw==
+  dependencies:
+    "@jupyterlab/apputils" "^3.6.3"
+    "@jupyterlab/coreutils" "^5.6.3"
+    "@jupyterlab/docprovider" "^3.6.3"
+    "@jupyterlab/docregistry" "^3.6.3"
+    "@jupyterlab/services" "^6.6.3"
+    "@jupyterlab/statusbar" "^3.6.3"
+    "@jupyterlab/translation" "^3.6.3"
     "@lumino/algorithm" "^1.9.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/messaging" "^1.10.0"
     "@lumino/properties" "^1.8.0"
     "@lumino/signaling" "^1.10.0"
-    "@lumino/widgets" "^1.37.1"
+    "@lumino/widgets" "^1.37.2"
     react "^17.0.1"
 
-"@jupyterlab/docprovider@^3.6.1":
-  version "3.6.1"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/docprovider/-/docprovider-3.6.1.tgz#8be66a419d595b490d6ca3f79238fd160d1cd53e"
-  integrity sha512-YeqLMPlC2jEWBvxgIVfhxbeYXWKb5DGEkv+WJp11S6oFgSNqAHZ1zqH1BB/+UgYWwwkafADwAjepaGFhnr2pPw==
-  dependencies:
-    "@jupyter/ydoc" "~0.2.0"
-    "@jupyterlab/coreutils" "^5.6.1"
-    "@jupyterlab/services" "^6.6.1"
+"@jupyterlab/docprovider@^3.6.3":
+  version "3.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/docprovider/-/docprovider-3.6.3.tgz#90fbf07214b6c3e98055787fc351a68e9d83470c"
+  integrity sha512-M5IoyykDpWnUFNePHz3+fi/RNvV92UNbQGfAvsaCMSn+fl48rD4rHB9EZGceOisb3m1U+E4SntKYI3pl49yUEg==
+  dependencies:
+    "@jupyter/ydoc" "~0.2.3"
+    "@jupyterlab/apputils" "^3.6.3"
+    "@jupyterlab/coreutils" "^5.6.3"
+    "@jupyterlab/services" "^6.6.3"
+    "@jupyterlab/translation" "^3.6.3"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/signaling" "^1.10.0"
     y-protocols "^1.0.5"
-    y-websocket "^1.3.15"
-    yjs "^13.5.17"
+    y-websocket "^1.4.6"
 
-"@jupyterlab/docregistry@^3.6", "@jupyterlab/docregistry@^3.6.1":
-  version "3.6.1"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/docregistry/-/docregistry-3.6.1.tgz#942b76ea7c59ab9ee375dce4a7bb9377d28d7f61"
-  integrity sha512-uQsmw1LpvcRC8CZ/cjmFnQKB+E+kWqJQDGwtzBDjZm4UcADVs1mwvSwPpAZvTBb0gmYBcS09mTZt7WgVv1Nj8A==
-  dependencies:
-    "@jupyter/ydoc" "~0.2.0"
-    "@jupyterlab/apputils" "^3.6.1"
-    "@jupyterlab/codeeditor" "^3.6.1"
-    "@jupyterlab/codemirror" "^3.6.1"
-    "@jupyterlab/coreutils" "^5.6.1"
-    "@jupyterlab/docprovider" "^3.6.1"
-    "@jupyterlab/observables" "^4.6.1"
-    "@jupyterlab/rendermime" "^3.6.1"
-    "@jupyterlab/rendermime-interfaces" "^3.6.1"
-    "@jupyterlab/services" "^6.6.1"
-    "@jupyterlab/translation" "^3.6.1"
-    "@jupyterlab/ui-components" "^3.6.1"
+"@jupyterlab/docregistry@^3.0.0", "@jupyterlab/docregistry@^3.6", "@jupyterlab/docregistry@^3.6.3":
+  version "3.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/docregistry/-/docregistry-3.6.3.tgz#4a03fbb704449bda7a94df7a4bd63078c11aef58"
+  integrity sha512-unDMrtCSGKPqX9uvYCkI7zGTvskuC9odAPIHPsYSVMcHL/o5M7lQkHmRZCoSIezfe5OvPGXbYT2boQrBKXqCFw==
+  dependencies:
+    "@jupyter/ydoc" "~0.2.3"
+    "@jupyterlab/apputils" "^3.6.3"
+    "@jupyterlab/codeeditor" "^3.6.3"
+    "@jupyterlab/codemirror" "^3.6.3"
+    "@jupyterlab/coreutils" "^5.6.3"
+    "@jupyterlab/docprovider" "^3.6.3"
+    "@jupyterlab/observables" "^4.6.3"
+    "@jupyterlab/rendermime" "^3.6.3"
+    "@jupyterlab/rendermime-interfaces" "^3.6.3"
+    "@jupyterlab/services" "^6.6.3"
+    "@jupyterlab/translation" "^3.6.3"
+    "@jupyterlab/ui-components" "^3.6.3"
     "@lumino/algorithm" "^1.9.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/messaging" "^1.10.0"
     "@lumino/signaling" "^1.10.0"
-    "@lumino/widgets" "^1.37.1"
+    "@lumino/widgets" "^1.37.2"
 
-"@jupyterlab/filebrowser@^3.6", "@jupyterlab/filebrowser@^3.6.1":
-  version "3.6.1"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/filebrowser/-/filebrowser-3.6.1.tgz#8fe44d03545fd9318fe8014edd5c4ddbf705bcb5"
-  integrity sha512-brd5PQQ1m9HK+53opahoi6SaEO0oweRloE1GJEA9t9CHKklpiZ18/3QXF+WDgHtV2UU3ZDmND7Fq5YCets2lBg==
-  dependencies:
-    "@jupyterlab/apputils" "^3.6.1"
-    "@jupyterlab/coreutils" "^5.6.1"
-    "@jupyterlab/docmanager" "^3.6.1"
-    "@jupyterlab/docregistry" "^3.6.1"
-    "@jupyterlab/services" "^6.6.1"
-    "@jupyterlab/statedb" "^3.6.1"
-    "@jupyterlab/statusbar" "^3.6.1"
-    "@jupyterlab/translation" "^3.6.1"
-    "@jupyterlab/ui-components" "^3.6.1"
+"@jupyterlab/filebrowser@^3.6", "@jupyterlab/filebrowser@^3.6.3":
+  version "3.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/filebrowser/-/filebrowser-3.6.3.tgz#169b880e19a8686f9a669a750027c2817b4b6cef"
+  integrity sha512-Qu+Mtx3d0QY7qCMIxg5nQtkQYh+kZ2kGO7tgS+yfKjo0cluPsxo+Zr56KtJU6zyDYjylVCtLYIK2RflwRKhdng==
+  dependencies:
+    "@jupyterlab/apputils" "^3.6.3"
+    "@jupyterlab/coreutils" "^5.6.3"
+    "@jupyterlab/docmanager" "^3.6.3"
+    "@jupyterlab/docregistry" "^3.6.3"
+    "@jupyterlab/services" "^6.6.3"
+    "@jupyterlab/statedb" "^3.6.3"
+    "@jupyterlab/statusbar" "^3.6.3"
+    "@jupyterlab/translation" "^3.6.3"
+    "@jupyterlab/ui-components" "^3.6.3"
     "@lumino/algorithm" "^1.9.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/domutils" "^1.8.0"
     "@lumino/dragdrop" "^1.13.0"
     "@lumino/messaging" "^1.10.0"
     "@lumino/polling" "^1.9.0"
     "@lumino/signaling" "^1.10.0"
     "@lumino/virtualdom" "^1.14.0"
-    "@lumino/widgets" "^1.37.1"
+    "@lumino/widgets" "^1.37.2"
     react "^17.0.1"
 
 "@jupyterlab/launcher@^3.6":
-  version "3.6.1"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/launcher/-/launcher-3.6.1.tgz#f525e04f9a341d633afd32d61db76594cc3027bb"
-  integrity sha512-DZFirXQei8jwR4LC5h6ezCqVfkkLjvXhUSLwX3Wtj4VcJ5ErTcXlZGQwqDECgEVMbdoXNcizMfSaUAM1JPsvmQ==
-  dependencies:
-    "@jupyterlab/apputils" "^3.6.1"
-    "@jupyterlab/translation" "^3.6.1"
-    "@jupyterlab/ui-components" "^3.6.1"
+  version "3.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/launcher/-/launcher-3.6.3.tgz#e3d28fc96063542950c1cfc53b9a324ede76dd9d"
+  integrity sha512-fQQ4DyDWeOUdXl70xi6EWAVAG0AXN7TYqFRx+hyPKg3WtRIypQ0End8uKIzzHXAXqtBJdyF+iEZwUeE3wEkDow==
+  dependencies:
+    "@jupyterlab/apputils" "^3.6.3"
+    "@jupyterlab/translation" "^3.6.3"
+    "@jupyterlab/ui-components" "^3.6.3"
     "@lumino/algorithm" "^1.9.0"
     "@lumino/commands" "^1.19.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/properties" "^1.8.0"
-    "@lumino/widgets" "^1.37.1"
+    "@lumino/widgets" "^1.37.2"
     react "^17.0.1"
 
-"@jupyterlab/mainmenu@^3.6":
-  version "3.6.1"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/mainmenu/-/mainmenu-3.6.1.tgz#aa7ea5364566adef08453bfa645d62e347d09455"
-  integrity sha512-wZqFNHC8DKRNl6rKMIZZWE//ZG9YbYyQ+sX4UOPqA4mg8fmQX90V57+vqV76d0dgivSQffO06CktKhnhD6J94Q==
-  dependencies:
-    "@jupyterlab/apputils" "^3.6.1"
-    "@jupyterlab/services" "^6.6.1"
-    "@jupyterlab/translation" "^3.6.1"
-    "@jupyterlab/ui-components" "^3.6.1"
+"@jupyterlab/logconsole@^3.0.0":
+  version "3.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/logconsole/-/logconsole-3.6.3.tgz#9ecc3a7545aa7848a6ca34eb546f58aede8343ba"
+  integrity sha512-fjhRbkf1wW6QD7nrlGjWAke0C3w2NB0ta5nBMXcc/wulBFjRQ4h7pY0wdSOsr7xMad21lrWEeRmxBdekazUBnw==
+  dependencies:
+    "@jupyterlab/coreutils" "^5.6.3"
+    "@jupyterlab/nbformat" "^3.6.3"
+    "@jupyterlab/outputarea" "^3.6.3"
+    "@jupyterlab/rendermime" "^3.6.3"
+    "@jupyterlab/services" "^6.6.3"
+    "@jupyterlab/translation" "^3.6.3"
+    "@lumino/coreutils" "^1.11.0"
+    "@lumino/disposable" "^1.10.0"
+    "@lumino/messaging" "^1.10.0"
+    "@lumino/signaling" "^1.10.0"
+    "@lumino/widgets" "^1.37.2"
+
+"@jupyterlab/mainmenu@^3.0.0", "@jupyterlab/mainmenu@^3.6":
+  version "3.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/mainmenu/-/mainmenu-3.6.3.tgz#5d322db9b8d742b7042109ab7e8c733696ae38fc"
+  integrity sha512-ohZzHDeReKX3zbLz2bUsYRSdkX6bVhNoCer3Rat8gjfb8vr/bqK9ReAvvoA4rRqm0mrfqwotpZSzbE4+y5KqZA==
+  dependencies:
+    "@jupyterlab/apputils" "^3.6.3"
+    "@jupyterlab/services" "^6.6.3"
+    "@jupyterlab/translation" "^3.6.3"
+    "@jupyterlab/ui-components" "^3.6.3"
     "@lumino/algorithm" "^1.9.0"
     "@lumino/commands" "^1.19.0"
     "@lumino/coreutils" "^1.11.0"
-    "@lumino/widgets" "^1.37.1"
+    "@lumino/widgets" "^1.37.2"
 
-"@jupyterlab/nbformat@^3.0.0 || ^4.0.0-alpha.15", "@jupyterlab/nbformat@^3.6.1":
-  version "3.6.1"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/nbformat/-/nbformat-3.6.1.tgz#84f1239ff0a54d693beed21534aef1baeaa93518"
-  integrity sha512-fLJTAwnQZ/5H9dBV/noqlkbGmGBbcsgd0FHWyMVIq+efKFX6CW1MOk61uM76rfahkke3XgYgvlXsw7i7lEIhcA==
+"@jupyterlab/nbformat@^3.0.0", "@jupyterlab/nbformat@^3.0.0 || ^4.0.0-alpha.15", "@jupyterlab/nbformat@^3.6.3":
+  version "3.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/nbformat/-/nbformat-3.6.3.tgz#8520338e3679cbe8ce2ea8eb5a9b816f8b774ad3"
+  integrity sha512-0qJLa4dtOmu9EmHFeM7gaZi4qheovIPc9ZrgGGRuG0obajs4YYlvh4MQvCSgpVhme4AuBfGlcfzhlx+Gbzr5Xw==
   dependencies:
     "@lumino/coreutils" "^1.11.0"
 
-"@jupyterlab/observables@^4.6.1":
-  version "4.6.1"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/observables/-/observables-4.6.1.tgz#7d05b60192e85732db29de5f9e8525798a08aee6"
-  integrity sha512-ez+fxyE3qwQ9grZ0nj2fpgcPIGySs/cNfojfcQatziV2rbFZzrBJJsWFSBhPO55vJd1Mue21aPw1eEK3ok4Wfw==
+"@jupyterlab/notebook@^3.0.0":
+  version "3.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/notebook/-/notebook-3.6.3.tgz#1584be72184d67d59291e2b22f55bc257afde436"
+  integrity sha512-id1KD5/9IDPr/IZFCl/YX4Vc+Q198LZshhFNEcVJZcRdjD7Vh+LGvWcLOh80OAv86J4XSTTAsp3gHPr4iSwPDg==
+  dependencies:
+    "@jupyter/ydoc" "~0.2.3"
+    "@jupyterlab/apputils" "^3.6.3"
+    "@jupyterlab/cells" "^3.6.3"
+    "@jupyterlab/codeeditor" "^3.6.3"
+    "@jupyterlab/coreutils" "^5.6.3"
+    "@jupyterlab/docregistry" "^3.6.3"
+    "@jupyterlab/nbformat" "^3.6.3"
+    "@jupyterlab/observables" "^4.6.3"
+    "@jupyterlab/rendermime" "^3.6.3"
+    "@jupyterlab/services" "^6.6.3"
+    "@jupyterlab/settingregistry" "^3.6.3"
+    "@jupyterlab/statusbar" "^3.6.3"
+    "@jupyterlab/translation" "^3.6.3"
+    "@jupyterlab/ui-components" "^3.6.3"
+    "@lumino/algorithm" "^1.9.0"
+    "@lumino/coreutils" "^1.11.0"
+    "@lumino/domutils" "^1.8.0"
+    "@lumino/dragdrop" "^1.13.0"
+    "@lumino/messaging" "^1.10.0"
+    "@lumino/properties" "^1.8.0"
+    "@lumino/signaling" "^1.10.0"
+    "@lumino/virtualdom" "^1.14.0"
+    "@lumino/widgets" "^1.37.2"
+    react "^17.0.1"
+
+"@jupyterlab/observables@^4.6.3":
+  version "4.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/observables/-/observables-4.6.3.tgz#49a9ca49fbda7428abbd1bfb8a4006ecd406c18d"
+  integrity sha512-CvQoL+9WHXOy/CXp/PQLi4c5iZVJ4psz11+GrycDDinX1AdVQ8a43OLTC0gxWl3Tk2C8ZvAi1sgn4FS68E1ACQ==
   dependencies:
     "@lumino/algorithm" "^1.9.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/messaging" "^1.10.0"
     "@lumino/signaling" "^1.10.0"
 
-"@jupyterlab/outputarea@^3.6.1":
-  version "3.6.1"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/outputarea/-/outputarea-3.6.1.tgz#904d0933d4e8c4bedb6e4179da8d4b6cfd32630d"
-  integrity sha512-/OWU9LvKeRUk5mzQskhPQtWY6/NIiRy3bzhbFesSJ1+3f+L1pk7mXCHmRxiG6FSw2ujeCV3vO4uFTXGLxoqiAw==
-  dependencies:
-    "@jupyterlab/apputils" "^3.6.1"
-    "@jupyterlab/nbformat" "^3.6.1"
-    "@jupyterlab/observables" "^4.6.1"
-    "@jupyterlab/rendermime" "^3.6.1"
-    "@jupyterlab/rendermime-interfaces" "^3.6.1"
-    "@jupyterlab/services" "^6.6.1"
+"@jupyterlab/outputarea@^3.0.0", "@jupyterlab/outputarea@^3.6.3":
+  version "3.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/outputarea/-/outputarea-3.6.3.tgz#acf7a604eb352109d096d2a9fdd1fbbddbf80af1"
+  integrity sha512-SSmkDWS8MhdXl7+rQoLu/5wJBKTq1YEkxlQcKh1Z0VN4VjYDCA/bKFGjOmKN7wMmoVP/zRmWvUwl/DLJCHx/Tw==
+  dependencies:
+    "@jupyterlab/apputils" "^3.6.3"
+    "@jupyterlab/nbformat" "^3.6.3"
+    "@jupyterlab/observables" "^4.6.3"
+    "@jupyterlab/rendermime" "^3.6.3"
+    "@jupyterlab/rendermime-interfaces" "^3.6.3"
+    "@jupyterlab/services" "^6.6.3"
     "@lumino/algorithm" "^1.9.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/messaging" "^1.10.0"
     "@lumino/properties" "^1.8.0"
     "@lumino/signaling" "^1.10.0"
-    "@lumino/widgets" "^1.37.1"
+    "@lumino/widgets" "^1.37.2"
     resize-observer-polyfill "^1.5.1"
 
-"@jupyterlab/rendermime-interfaces@^3.6.1":
-  version "3.6.1"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/rendermime-interfaces/-/rendermime-interfaces-3.6.1.tgz#d531a6ba228df83b581aee0df5041f7f9a1b4495"
-  integrity sha512-IB0rFBTRpguGbAF/WmNPa//UfXcZLRur5DuSwP5tRz2iUZIu/dAFeLDq3j8NL2POz1+yeXyQSQyp2Xu9w8CrFw==
+"@jupyterlab/rendermime-interfaces@^3.0.0", "@jupyterlab/rendermime-interfaces@^3.6.3":
+  version "3.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/rendermime-interfaces/-/rendermime-interfaces-3.6.3.tgz#80009705d5ded65a4b27c4b826b295f40f126902"
+  integrity sha512-VHZVnqB0K1nmoQMOhFGHwvSYMQmxqcOC3wWDRFeUOv8S+tejTYfbrKXPOZJvhdGB52Jn8XNIesXOuNpLhl4HmQ==
   dependencies:
-    "@jupyterlab/translation" "^3.6.1"
+    "@jupyterlab/translation" "^3.6.3"
     "@lumino/coreutils" "^1.11.0"
-    "@lumino/widgets" "^1.37.1"
+    "@lumino/widgets" "^1.37.2"
 
-"@jupyterlab/rendermime@^3.6", "@jupyterlab/rendermime@^3.6.1":
-  version "3.6.1"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/rendermime/-/rendermime-3.6.1.tgz#ebeef56293cf83f6aa8eb8f12edcd16c4eaafae7"
-  integrity sha512-v4YHIxSd+0foqyzTaloBPevdYUBgZ4Tk1uuXzTdCVIdceS9MG76UfjBu8EPl86AZI8R2ihlHh01pxpgLX0Smdw==
-  dependencies:
-    "@jupyterlab/apputils" "^3.6.1"
-    "@jupyterlab/codemirror" "^3.6.1"
-    "@jupyterlab/coreutils" "^5.6.1"
-    "@jupyterlab/nbformat" "^3.6.1"
-    "@jupyterlab/observables" "^4.6.1"
-    "@jupyterlab/rendermime-interfaces" "^3.6.1"
-    "@jupyterlab/services" "^6.6.1"
-    "@jupyterlab/translation" "^3.6.1"
+"@jupyterlab/rendermime@^3.0.0", "@jupyterlab/rendermime@^3.6", "@jupyterlab/rendermime@^3.6.3":
+  version "3.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/rendermime/-/rendermime-3.6.3.tgz#48d83c70493b0356d4dac6d89a863d8a5a84f68e"
+  integrity sha512-w3e38OddJin9fbfe7EWsKiiup/0ayvHPrAsacde8PqGLvi/sLeAXT98PqihsKt8EAlOgXSkSO0Ivjbd0JzgGgA==
+  dependencies:
+    "@jupyterlab/apputils" "^3.6.3"
+    "@jupyterlab/codemirror" "^3.6.3"
+    "@jupyterlab/coreutils" "^5.6.3"
+    "@jupyterlab/nbformat" "^3.6.3"
+    "@jupyterlab/observables" "^4.6.3"
+    "@jupyterlab/rendermime-interfaces" "^3.6.3"
+    "@jupyterlab/services" "^6.6.3"
+    "@jupyterlab/translation" "^3.6.3"
     "@lumino/algorithm" "^1.9.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/messaging" "^1.10.0"
     "@lumino/signaling" "^1.10.0"
-    "@lumino/widgets" "^1.37.1"
+    "@lumino/widgets" "^1.37.2"
     lodash.escape "^4.0.1"
     marked "^4.0.17"
 
-"@jupyterlab/services@^6.6", "@jupyterlab/services@^6.6.1":
-  version "6.6.1"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/services/-/services-6.6.1.tgz#5fd96574bb1eee2e4217a6d039b4dcdeb51bb66f"
-  integrity sha512-4YIwTsfx7+JO7Lz9YFTpUvniA3aHdR5dDQJfdo9TsCMxs+NDVfjNAvp9VHa1xNJWYll4Ay31lYWbvuN/SI+KEA==
-  dependencies:
-    "@jupyterlab/coreutils" "^5.6.1"
-    "@jupyterlab/nbformat" "^3.6.1"
-    "@jupyterlab/observables" "^4.6.1"
-    "@jupyterlab/settingregistry" "^3.6.1"
-    "@jupyterlab/statedb" "^3.6.1"
+"@jupyterlab/services@^6.0.0", "@jupyterlab/services@^6.6", "@jupyterlab/services@^6.6.3":
+  version "6.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/services/-/services-6.6.3.tgz#303938e5dc5aebce7a86324a64ed89c25c61c9e7"
+  integrity sha512-BxEOMRl9X18T5wY7iV6ZJhARnibFghpD3OruqeSbnGdbRv6XJi8prsRbCQQ6Mf9agvf81B20KmDvYKikPHC0xQ==
+  dependencies:
+    "@jupyterlab/coreutils" "^5.6.3"
+    "@jupyterlab/nbformat" "^3.6.3"
+    "@jupyterlab/observables" "^4.6.3"
+    "@jupyterlab/settingregistry" "^3.6.3"
+    "@jupyterlab/statedb" "^3.6.3"
     "@lumino/algorithm" "^1.9.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/polling" "^1.9.0"
     "@lumino/signaling" "^1.10.0"
     node-fetch "^2.6.0"
     ws "^7.4.6"
 
-"@jupyterlab/settingregistry@^3.6", "@jupyterlab/settingregistry@^3.6.1":
-  version "3.6.1"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/settingregistry/-/settingregistry-3.6.1.tgz#cd04e64d598598950c64aa99e1fc8a2c962d8c31"
-  integrity sha512-zNCYIK6/oWG6JnhmwRGE/Zvn5Xhj0kovcJgTlOSHGyIiHqLfJA9TzHZDNUDANqqxAg4+H9fYdh1+agi4XWGL8A==
+"@jupyterlab/settingregistry@^3.0.0", "@jupyterlab/settingregistry@^3.6", "@jupyterlab/settingregistry@^3.6.3":
+  version "3.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/settingregistry/-/settingregistry-3.6.3.tgz#642f8b6449d626821ef13a7e778ae716fa8331c9"
+  integrity sha512-pnzIge0ZC8V63R97HiNroJ0eaPM0DN6x65SStyLuv/K8Qez4XqpOdc0Wfell5ri5mxMvm1qKekuFeTikqSXQKQ==
   dependencies:
-    "@jupyterlab/statedb" "^3.6.1"
+    "@jupyterlab/statedb" "^3.6.3"
     "@lumino/commands" "^1.19.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/signaling" "^1.10.0"
     ajv "^6.12.3"
     json5 "^2.1.1"
 
-"@jupyterlab/statedb@^3.6.1":
-  version "3.6.1"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/statedb/-/statedb-3.6.1.tgz#3f64bfee22ff7779404835fa87b08c67e66716c3"
-  integrity sha512-6+fGzKUCaWBKX/fZDdXR++WgfvYE+Dv5ma8gkgcHaS2vEup2snkmgZ8fBUJXm5xVpU4KhXjTUb7dafLfG7BL3Q==
+"@jupyterlab/statedb@^3.6.3":
+  version "3.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/statedb/-/statedb-3.6.3.tgz#6ba2166af9232c9a185cf0077cf1272f24cc9a69"
+  integrity sha512-A36L+0NN8f0WOES2GdtZjp9uFuC7IBjhKiO/RlKRX5AFjNxoJ9oO3PZtoxJQYPnGBljMqVdRa+m9aYEfvKhYyQ==
   dependencies:
     "@lumino/commands" "^1.19.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/properties" "^1.8.0"
     "@lumino/signaling" "^1.10.0"
 
-"@jupyterlab/statusbar@^3.6.1":
-  version "3.6.1"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/statusbar/-/statusbar-3.6.1.tgz#382c32eb6599973176d5ac0497e4a0c9dfa8df37"
-  integrity sha512-rpQa6G6agR+lu3Djt/YTroQ4W3ZasfGmtmO24IXsm3C5418nPIl2oQeEJTc7OsXRvsdoCoAK7c/Rh9TeyhBhug==
-  dependencies:
-    "@jupyterlab/apputils" "^3.6.1"
-    "@jupyterlab/codeeditor" "^3.6.1"
-    "@jupyterlab/services" "^6.6.1"
-    "@jupyterlab/translation" "^3.6.1"
-    "@jupyterlab/ui-components" "^3.6.1"
+"@jupyterlab/statusbar@^3.6.3":
+  version "3.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/statusbar/-/statusbar-3.6.3.tgz#29c24427a2d6b205349b94583de0ccb8b9435d88"
+  integrity sha512-m59NLR0Zghm53PU6hDzRF4XVORnJx/YRx0svcjj/TGLk8LSffpQbUDBy24dl3tOuChk4D5cCdgeDH1X30TzCaA==
+  dependencies:
+    "@jupyterlab/apputils" "^3.6.3"
+    "@jupyterlab/codeeditor" "^3.6.3"
+    "@jupyterlab/services" "^6.6.3"
+    "@jupyterlab/translation" "^3.6.3"
+    "@jupyterlab/ui-components" "^3.6.3"
     "@lumino/algorithm" "^1.9.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/messaging" "^1.10.0"
     "@lumino/signaling" "^1.10.0"
-    "@lumino/widgets" "^1.37.1"
+    "@lumino/widgets" "^1.37.2"
     csstype "~3.0.3"
     react "^17.0.1"
     typestyle "^2.0.4"
 
-"@jupyterlab/translation@^3.6", "@jupyterlab/translation@^3.6.1":
-  version "3.6.1"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/translation/-/translation-3.6.1.tgz#db1380c349f2e8645b58a9eac4986f3f1c6b320b"
-  integrity sha512-+I1zzQnYNVnU9rrr7ceHPexiyMFavfK0t6I3qdgAHQ1TTLsLVQMp5m/T7S2SaJjPK7/GtRml5DgmErRyy5becA==
-  dependencies:
-    "@jupyterlab/coreutils" "^5.6.1"
-    "@jupyterlab/services" "^6.6.1"
-    "@jupyterlab/statedb" "^3.6.1"
+"@jupyterlab/translation@^3.0.0", "@jupyterlab/translation@^3.6", "@jupyterlab/translation@^3.6.3":
+  version "3.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/translation/-/translation-3.6.3.tgz#3fd95f726316762bc1799a7b7be0243d5465932a"
+  integrity sha512-m+wwBv/hiN5Y6Sb7Ij150ZhPXZdhN5wI8CT3afnzARwKr2Aww5AIURO3upmMwnKaPVQTrWqsS3+7bZS/21JuJA==
+  dependencies:
+    "@jupyterlab/coreutils" "^5.6.3"
+    "@jupyterlab/services" "^6.6.3"
+    "@jupyterlab/statedb" "^3.6.3"
     "@lumino/coreutils" "^1.11.0"
 
-"@jupyterlab/ui-components@^3.6", "@jupyterlab/ui-components@^3.6.1":
-  version "3.6.1"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/ui-components/-/ui-components-3.6.1.tgz#1e12b23614288a1c45fda50c2d141483b879bebf"
-  integrity sha512-p9wH9iidGuuKSm2yXFGhHs6gzpoBpsHRCiOJw9bmj2PBsDKEGjh65Rh0YBv0d7TD6VVgAwMmokaT01KqjUmY+g==
+"@jupyterlab/ui-components@^3.6", "@jupyterlab/ui-components@^3.6.3":
+  version "3.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/ui-components/-/ui-components-3.6.3.tgz#36555036b383c5d80346f409a7a168d13c9d8c85"
+  integrity sha512-XzseUo2IXclPlYcGxCIz8evjWF+dCBMmbJlvoE5OF29BYBvI5N/DUaTem8bHN5kmQwHIXX6BImHu7rbC9Xjl6w==
   dependencies:
     "@blueprintjs/core" "^3.36.0"
     "@blueprintjs/select" "^3.15.0"
-    "@jupyterlab/coreutils" "^5.6.1"
-    "@jupyterlab/translation" "^3.6.1"
+    "@jupyterlab/coreutils" "^5.6.3"
+    "@jupyterlab/translation" "^3.6.3"
     "@lumino/algorithm" "^1.9.0"
     "@lumino/commands" "^1.19.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/signaling" "^1.10.0"
     "@lumino/virtualdom" "^1.14.0"
-    "@lumino/widgets" "^1.37.1"
+    "@lumino/widgets" "^1.37.2"
     "@rjsf/core" "^3.1.0"
     react "^17.0.1"
     react-dom "^17.0.1"
     typestyle "^2.0.4"
 
 "@lerna/child-process@6.5.1":
   version "6.5.1"
@@ -705,32 +833,27 @@
     pify "^5.0.0"
     semver "^7.3.4"
     slash "^3.0.0"
     validate-npm-package-license "^3.0.4"
     validate-npm-package-name "^4.0.0"
     yargs-parser "20.2.4"
 
-"@lumino/algorithm@^1.9.0", "@lumino/algorithm@^1.9.2":
+"@lumino/algorithm@^1.9.0", "@lumino/algorithm@^1.9.1", "@lumino/algorithm@^1.9.2":
   version "1.9.2"
   resolved "https://registry.yarnpkg.com/@lumino/algorithm/-/algorithm-1.9.2.tgz#b95e6419aed58ff6b863a51bfb4add0f795141d3"
   integrity sha512-Z06lp/yuhz8CtIir3PNTGnuk7909eXt4ukJsCzChsGuot2l5Fbs96RJ/FOHgwCedaX74CtxPjXHXoszFbUA+4A==
 
-"@lumino/algorithm@^2.0.0":
-  version "2.0.0"
-  resolved "https://registry.yarnpkg.com/@lumino/algorithm/-/algorithm-2.0.0.tgz#f36e4b6bf6d2b9bde66dc3162afc9a0d2ef47530"
-  integrity sha512-SwM/8U1zlMWMJj00wTCThdTUit9zap2Xghuo4uUxvZ+mfog5b1UIk2j1dP8TPpzEXHCDPEb85s2/ERo1tee3Dw==
-
-"@lumino/application@^1.31.3":
-  version "1.31.3"
-  resolved "https://registry.yarnpkg.com/@lumino/application/-/application-1.31.3.tgz#c5a9bc84212a2505be8f5d43516e0603d9100965"
-  integrity sha512-XnsXm5PD9QevJRl/pHJziYmhRKqJYjEOTL6Vh9dtKpPPML57uswOj59Pokxx/yCvym1xRF9iDVvujy3KallRwQ==
+"@lumino/application@^1.31.4":
+  version "1.31.4"
+  resolved "https://registry.yarnpkg.com/@lumino/application/-/application-1.31.4.tgz#b804fcc46fb77deb41aee94c48bea990f735d6b9"
+  integrity sha512-dOSsDJ1tXOxC3fnSHvtDQK5RcICLEVPtO19HeCGwurb5W2ZZ55SZT2b5jZu6V/v8lGdtkNbr1RJltRpJRSRb/A==
   dependencies:
     "@lumino/commands" "^1.21.1"
     "@lumino/coreutils" "^1.12.1"
-    "@lumino/widgets" "^1.37.1"
+    "@lumino/widgets" "^1.37.2"
 
 "@lumino/collections@^1.9.3":
   version "1.9.3"
   resolved "https://registry.yarnpkg.com/@lumino/collections/-/collections-1.9.3.tgz#370dc2d50aa91371288a4f7376bea5a3191fc5dc"
   integrity sha512-2i2Wf1xnfTgEgdyKEpqM16bcYRIhUOGCDzaVCEZACVG9R1CgYwOe3zfn71slBQOVSjjRgwYrgLXu4MBpt6YK+g==
   dependencies:
     "@lumino/algorithm" "^1.9.2"
@@ -744,58 +867,46 @@
     "@lumino/coreutils" "^1.12.1"
     "@lumino/disposable" "^1.10.4"
     "@lumino/domutils" "^1.8.2"
     "@lumino/keyboard" "^1.8.2"
     "@lumino/signaling" "^1.11.1"
     "@lumino/virtualdom" "^1.14.3"
 
-"@lumino/coreutils@^1.11.0", "@lumino/coreutils@^1.12.1":
+"@lumino/coreutils@^1.11.0", "@lumino/coreutils@^1.11.0 || ^2.0.0-alpha.6", "@lumino/coreutils@^1.11.1", "@lumino/coreutils@^1.12.1":
   version "1.12.1"
   resolved "https://registry.yarnpkg.com/@lumino/coreutils/-/coreutils-1.12.1.tgz#79860c9937483ddf6cda87f6c2b9da8eb1a5d768"
   integrity sha512-JLu3nTHzJk9N8ohZ85u75YxemMrmDzJdNgZztfP7F7T7mxND3YVNCkJG35a6aJ7edu1sIgCjBxOvV+hv27iYvQ==
 
-"@lumino/coreutils@^1.11.0 || ^2.0.0-alpha.6", "@lumino/coreutils@^2.0.0":
-  version "2.0.0"
-  resolved "https://registry.yarnpkg.com/@lumino/coreutils/-/coreutils-2.0.0.tgz#f7a82e616156bda83197ee4e176810af6799a27b"
-  integrity sha512-eMPssdjM/qYsX7AwX4gWI07ijzxDFyM7i8dT35YY7P6r0OeqIzmVruu/3RJhHfKoVJ/fINlS9B8EsOC81GMIGA==
-
-"@lumino/disposable@^1.10.0", "@lumino/disposable@^1.10.4":
+"@lumino/disposable@^1.10.0", "@lumino/disposable@^1.10.0 || ^2.0.0-alpha.6", "@lumino/disposable@^1.10.1", "@lumino/disposable@^1.10.4":
   version "1.10.4"
   resolved "https://registry.yarnpkg.com/@lumino/disposable/-/disposable-1.10.4.tgz#73b452044fecf988d7fa73fac9451b1a7f987323"
   integrity sha512-4ZxyYcyzUS+ZeB2KAH9oAH3w0DUUceiVr+FIZHZ2TAYGWZI/85WlqJtfm0xjwEpCwLLW1TDqJrISuZu3iMmVMA==
   dependencies:
     "@lumino/algorithm" "^1.9.2"
     "@lumino/signaling" "^1.11.1"
 
-"@lumino/disposable@^1.10.0 || ^2.0.0-alpha.6":
-  version "2.0.0"
-  resolved "https://registry.yarnpkg.com/@lumino/disposable/-/disposable-2.0.0.tgz#6ad4927aaee03b8c55b870a8466fca5b759d5a1e"
-  integrity sha512-2PcwxbKU1xYd02wWCsk5F/Ufh/tbNAMb+zXJEOGcRPrgOihkIz3FEDtbhOVGuGw8FtYlisKIs1m+pq37LUHL6A==
-  dependencies:
-    "@lumino/signaling" "^2.0.0"
-
-"@lumino/domutils@^1.8.0", "@lumino/domutils@^1.8.2":
+"@lumino/domutils@^1.8.0", "@lumino/domutils@^1.8.1", "@lumino/domutils@^1.8.2":
   version "1.8.2"
   resolved "https://registry.yarnpkg.com/@lumino/domutils/-/domutils-1.8.2.tgz#d15cdbae12bea52852bbc13c4629360f9f05b7f5"
   integrity sha512-QIpMfkPJrs4GrWBuJf2Sn1fpyVPmvqUUAeD8xAQo8+4V5JAT0vUDLxZ9HijefMgNCi3+Bs8Z3lQwRCrz+cFP1A==
 
-"@lumino/dragdrop@^1.13.0", "@lumino/dragdrop@^1.14.4":
-  version "1.14.4"
-  resolved "https://registry.yarnpkg.com/@lumino/dragdrop/-/dragdrop-1.14.4.tgz#b6ec4cf4f470c17a849e31f299d5a24acdc8c7d3"
-  integrity sha512-IHX2M8Yqs2YsFHHXKSKiYLgv9DEuhyyKoDS85Chg34J9OaPC5ocT0AmNVnpeq9T4A50sg3vdL9mSRCZ0f302Gw==
+"@lumino/dragdrop@^1.13.0", "@lumino/dragdrop@^1.14.5":
+  version "1.14.5"
+  resolved "https://registry.yarnpkg.com/@lumino/dragdrop/-/dragdrop-1.14.5.tgz#1db76c8a01f74cb1b0428db6234e820bb58b93ba"
+  integrity sha512-LC5xB82+xGF8hFyl716TMpV32OIMIMl+s3RU1PaqDkD6B7PkgiVk6NkJ4X9/GcEvl2igkvlGQt/3L7qxDAJNxw==
   dependencies:
     "@lumino/coreutils" "^1.12.1"
     "@lumino/disposable" "^1.10.4"
 
 "@lumino/keyboard@^1.8.2":
   version "1.8.2"
   resolved "https://registry.yarnpkg.com/@lumino/keyboard/-/keyboard-1.8.2.tgz#714dbe671f0718f516d1ec23188b31a9ccd82fb2"
   integrity sha512-Dy+XqQ1wXbcnuYtjys5A0pAqf4SpAFl9NY6owyIhXAo0Va7w3LYp3jgiP1xAaBAwMuUppiUAfrbjrysZuZ625g==
 
-"@lumino/messaging@^1.10.0", "@lumino/messaging@^1.10.3":
+"@lumino/messaging@^1.10.0", "@lumino/messaging@^1.10.1", "@lumino/messaging@^1.10.3":
   version "1.10.3"
   resolved "https://registry.yarnpkg.com/@lumino/messaging/-/messaging-1.10.3.tgz#b6227bdfc178a8542571625ecb68063691b6af3c"
   integrity sha512-F/KOwMCdqvdEG8CYAJcBSadzp6aI7a47Fr60zAKGqZATSRRRV41q53iXU7HjFPqQqQIvdn9Z7J32rBEAyQAzww==
   dependencies:
     "@lumino/algorithm" "^1.9.2"
     "@lumino/collections" "^1.9.3"
 
@@ -804,53 +915,45 @@
   resolved "https://registry.yarnpkg.com/@lumino/polling/-/polling-1.11.4.tgz#ddfe47da5b41af4cfa474898542c099e445c0e6c"
   integrity sha512-yC7JLssj3mqVK6TsYj7dg4AG0rcsC42YtpoDLtz9yzO84Q5flQUfmjAPQB6oPA6wZOlISs3iasF+uO2w1ls5jg==
   dependencies:
     "@lumino/coreutils" "^1.12.1"
     "@lumino/disposable" "^1.10.4"
     "@lumino/signaling" "^1.11.1"
 
-"@lumino/properties@^1.8.0", "@lumino/properties@^1.8.2":
+"@lumino/properties@^1.8.0", "@lumino/properties@^1.8.1", "@lumino/properties@^1.8.2":
   version "1.8.2"
   resolved "https://registry.yarnpkg.com/@lumino/properties/-/properties-1.8.2.tgz#91131f2ca91a902faa138771eb63341db78fc0fd"
   integrity sha512-EkjI9Cw8R0U+xC9HxdFSu7X1tz1H1vKu20cGvJ2gU+CXlMB1DvoYJCYxCThByHZ+kURTAap4SE5x8HvKwNPbig==
 
-"@lumino/signaling@^1.10.0", "@lumino/signaling@^1.11.1":
+"@lumino/signaling@^1.10.0", "@lumino/signaling@^1.10.0 || ^2.0.0-alpha.6", "@lumino/signaling@^1.10.1", "@lumino/signaling@^1.11.1":
   version "1.11.1"
   resolved "https://registry.yarnpkg.com/@lumino/signaling/-/signaling-1.11.1.tgz#438f447a1b644fd286549804f9851b5aec9679a2"
   integrity sha512-YCUmgw08VoyMN5KxzqPO3KMx+cwdPv28tAN06C0K7Q/dQf+oufb1XocuhZb5selTrTmmuXeizaYxgLIQGdS1fA==
   dependencies:
     "@lumino/algorithm" "^1.9.2"
     "@lumino/properties" "^1.8.2"
 
-"@lumino/signaling@^1.10.0 || ^2.0.0-alpha.6", "@lumino/signaling@^2.0.0":
-  version "2.0.0"
-  resolved "https://registry.yarnpkg.com/@lumino/signaling/-/signaling-2.0.0.tgz#56ad85d966719adde7532c2888f3c73562de5c86"
-  integrity sha512-v5VRG4asmrVV5yy9rrpZgS5s9djkLbnmI60dVFXIbMWKyNUziVaUB9SkMzsCOOF6b9IKxXVdrMxjcieX7F9qfA==
-  dependencies:
-    "@lumino/algorithm" "^2.0.0"
-    "@lumino/coreutils" "^2.0.0"
-
 "@lumino/virtualdom@^1.14.0", "@lumino/virtualdom@^1.14.3":
   version "1.14.3"
   resolved "https://registry.yarnpkg.com/@lumino/virtualdom/-/virtualdom-1.14.3.tgz#e490c36ff506d877cf45771d6968e3e26a8919fd"
   integrity sha512-5joUC1yuxeXbpfbSBm/OR8Mu9HoTo6PDX0RKqzlJ9o97iml7zayFN/ynzcxScKGQAo9iaXOY8uVIvGUT8FnsGw==
   dependencies:
     "@lumino/algorithm" "^1.9.2"
 
-"@lumino/widgets@^1.37.1":
-  version "1.37.1"
-  resolved "https://registry.yarnpkg.com/@lumino/widgets/-/widgets-1.37.1.tgz#d7a2398b276e15e60aff4fec58c035d46549a75b"
-  integrity sha512-/whz5B/hL0fjv0bR8JYZ+Emx+CH7HBwXc4TqI9PrrHGm3g6+jRJAyIFGZcQubqkPxxHrRE/VxQgoDKGhINw/Gw==
+"@lumino/widgets@^1.30.0", "@lumino/widgets@^1.37.1", "@lumino/widgets@^1.37.2":
+  version "1.37.2"
+  resolved "https://registry.yarnpkg.com/@lumino/widgets/-/widgets-1.37.2.tgz#b408fae221ecec2f1b028607782fbe1e82588bce"
+  integrity sha512-NHKu1NBDo6ETBDoNrqSkornfUCwc8EFFzw6+LWBfYVxn2PIwciq2SdiJGEyNqL+0h/A9eVKb5ui5z4cwpRekmQ==
   dependencies:
     "@lumino/algorithm" "^1.9.2"
     "@lumino/commands" "^1.21.1"
     "@lumino/coreutils" "^1.12.1"
     "@lumino/disposable" "^1.10.4"
     "@lumino/domutils" "^1.8.2"
-    "@lumino/dragdrop" "^1.14.4"
+    "@lumino/dragdrop" "^1.14.5"
     "@lumino/keyboard" "^1.8.2"
     "@lumino/messaging" "^1.10.3"
     "@lumino/properties" "^1.8.2"
     "@lumino/signaling" "^1.11.1"
     "@lumino/virtualdom" "^1.14.3"
 
 "@nodelib/fs.scandir@2.1.5":
@@ -1267,14 +1370,22 @@
     react-is "^16.9.0"
 
 "@tootallnate/once@2":
   version "2.0.0"
   resolved "https://registry.yarnpkg.com/@tootallnate/once/-/once-2.0.0.tgz#f544a148d3ab35801c1f633a7441fd87c2e484bf"
   integrity sha512-XCuKFP5PS55gnMVu3dty8KPatLqUoy/ZYzDzAGCQ8JNFCkLXzmI7vNHCR+XpbZaMWQK/vQubr7PkYq8g470J/A==
 
+"@types/backbone@1.4.14":
+  version "1.4.14"
+  resolved "https://registry.yarnpkg.com/@types/backbone/-/backbone-1.4.14.tgz#4b71f0c25d89cfa9a10b18042f0b03d35a53364c"
+  integrity sha512-85ldQ99fiYTJFBlZuAJRaCdvTZKZ2p1fSs3fVf+6Ub6k1X0g0hNJ0qJ/2FOByyyAQYLtbEz3shX5taKQfBKBDw==
+  dependencies:
+    "@types/jquery" "*"
+    "@types/underscore" "*"
+
 "@types/dom4@^2.0.1":
   version "2.0.2"
   resolved "https://registry.yarnpkg.com/@types/dom4/-/dom4-2.0.2.tgz#6495303f049689ce936ed328a3e5ede9c51408ee"
   integrity sha512-Rt4IC1T7xkCWa0OG1oSsPa0iqnxlDeQqKXZAHrQGLb7wFGncWm85MaxKUjAGejOrUynOgWlFi4c6S6IyJwoK4g==
 
 "@types/eslint-scope@^3.7.3":
   version "3.7.4"
@@ -1298,19 +1409,31 @@
   integrity sha512-WulqXMDUTYAXCjZnk6JtIHPigp55cVtDgDrO2gHRwhyJto21+1zbVCtOYB2L1F9w4qCQ0rOGWBnBe0FNTiEJIQ==
 
 "@types/estree@^0.0.51":
   version "0.0.51"
   resolved "https://registry.yarnpkg.com/@types/estree/-/estree-0.0.51.tgz#cfd70924a25a3fd32b218e5e420e6897e1ac4f40"
   integrity sha512-CuPgU6f3eT/XgKKPqKd/gLZV1Xmvf1a2R5POBOGQa6uv82xpls89HU5zKeVoyR8XzHd1RGNOlQlvUe3CFkjWNQ==
 
+"@types/jquery@*":
+  version "3.5.16"
+  resolved "https://registry.yarnpkg.com/@types/jquery/-/jquery-3.5.16.tgz#632131baf30951915b0317d48c98e9890bdf051d"
+  integrity sha512-bsI7y4ZgeMkmpG9OM710RRzDFp+w4P1RGiIt30C1mSBT+ExCleeh4HObwgArnDFELmRrOpXgSYN9VF1hj+f1lw==
+  dependencies:
+    "@types/sizzle" "*"
+
 "@types/json-schema@*", "@types/json-schema@^7.0.5", "@types/json-schema@^7.0.7", "@types/json-schema@^7.0.8", "@types/json-schema@^7.0.9":
   version "7.0.11"
   resolved "https://registry.yarnpkg.com/@types/json-schema/-/json-schema-7.0.11.tgz#d421b6c527a3037f7c84433fd2c4229e016863d3"
   integrity sha512-wOuvG1SN4Us4rez+tylwwwCV1psiNVOkJeM3AUWUNWg/jDQY2+HE/444y5gc+jBmRqASOm2Oeh5c1axHobwRKQ==
 
+"@types/lodash@^4.14.134":
+  version "4.14.194"
+  resolved "https://registry.yarnpkg.com/@types/lodash/-/lodash-4.14.194.tgz#b71eb6f7a0ff11bff59fc987134a093029258a76"
+  integrity sha512-r22s9tAS7imvBt2lyHC9B8AGwWnXaYb1tY09oyLkXDs4vArpYJzw09nj8MLx5VfciBPGIb+ZwG0ssYnEPJxn/g==
+
 "@types/minimatch@^3.0.3":
   version "3.0.5"
   resolved "https://registry.yarnpkg.com/@types/minimatch/-/minimatch-3.0.5.tgz#1001cc5e6a3704b83c236027e77f2f58ea010f40"
   integrity sha512-Klz949h02Gz2uZCMGwDUSDS1YBlTdDDgbWHi+81l29tQALUtvz4rAYi5uoVhE5Lagoq6DeqAUlbrHvW/mXDgdQ==
 
 "@types/minimist@^1.2.0":
   version "1.2.2"
@@ -1352,19 +1475,29 @@
   integrity sha512-hppQEBDmlwhFAXKJX2KnWLYu5yMfi91yazPb2l+lbJiwW+wdo1gNeRA+3RgNSO39WYX2euey41KEwnqesU2Jew==
 
 "@types/semver@^7.3.12":
   version "7.3.13"
   resolved "https://registry.yarnpkg.com/@types/semver/-/semver-7.3.13.tgz#da4bfd73f49bd541d28920ab0e2bf0ee80f71c91"
   integrity sha512-21cFJr9z3g5dW8B0CVI9g2O9beqaThGQ6ZFBqHfwhzLDKUxaqTIy3vnfah/UPkfOiF2pLq+tGz+W8RyCskuslw==
 
+"@types/sizzle@*":
+  version "2.3.3"
+  resolved "https://registry.yarnpkg.com/@types/sizzle/-/sizzle-2.3.3.tgz#ff5e2f1902969d305225a047c8a0fd5c915cebef"
+  integrity sha512-JYM8x9EGF163bEyhdJBpR2QX1R5naCJHC8ucJylJ3w9/CVBaskdQ8WqBf8MmQrd1kRvp/a4TS8HJ+bxzR7ZJYQ==
+
 "@types/source-list-map@*":
   version "0.1.2"
   resolved "https://registry.yarnpkg.com/@types/source-list-map/-/source-list-map-0.1.2.tgz#0078836063ffaf17412349bba364087e0ac02ec9"
   integrity sha512-K5K+yml8LTo9bWJI/rECfIPrGgxdpeNbj+d53lwN4QjW1MCwlkhUms+gtdzigTeUyBr09+u8BwOIY3MXvHdcsA==
 
+"@types/underscore@*":
+  version "1.11.4"
+  resolved "https://registry.yarnpkg.com/@types/underscore/-/underscore-1.11.4.tgz#62e393f8bc4bd8a06154d110c7d042a93751def3"
+  integrity sha512-uO4CD2ELOjw8tasUrAhvnn2W4A0ZECOvMjCivJr4gA9pGgjv+qxKWY9GLTMVEK8ej85BxQOocUyE7hImmSQYcg==
+
 "@types/webpack-sources@^0.1.5":
   version "0.1.9"
   resolved "https://registry.yarnpkg.com/@types/webpack-sources/-/webpack-sources-0.1.9.tgz#da69b06eb34f6432e6658acb5a6893c55d983920"
   integrity sha512-bvzMnzqoK16PQIC8AYHNdW45eREJQMd6WG/msQWX5V2+vZmODCOPb4TJcbgRljTZZTwTM4wUMcsI8FftNA7new==
   dependencies:
     "@types/node" "*"
     "@types/source-list-map" "*"
@@ -1890,20 +2023,27 @@
   resolved "https://registry.yarnpkg.com/axios/-/axios-1.3.4.tgz#f5760cefd9cfb51fd2481acf88c05f67c4523024"
   integrity sha512-toYm+Bsyl6VC5wSkfkbbNB6ROv7KY93PEBBL6xyDczaIHasAiv4wPqQ/c4RjoQzipxRD2W5g21cOqQulZ7rHwQ==
   dependencies:
     follow-redirects "^1.15.0"
     form-data "^4.0.0"
     proxy-from-env "^1.1.0"
 
+backbone@1.4.0:
+  version "1.4.0"
+  resolved "https://registry.yarnpkg.com/backbone/-/backbone-1.4.0.tgz#54db4de9df7c3811c3f032f34749a4cd27f3bd12"
+  integrity sha512-RLmDrRXkVdouTg38jcgHhyQ/2zjg7a8E6sz2zxfz21Hh17xDJYUHBZimVIt5fUyS8vbfpeSmTL3gUjTEvUV3qQ==
+  dependencies:
+    underscore ">=1.8.3"
+
 balanced-match@^1.0.0:
   version "1.0.2"
   resolved "https://registry.yarnpkg.com/balanced-match/-/balanced-match-1.0.2.tgz#e83e3a7e3f300b34cb9d87f615fa0cbf357690ee"
   integrity sha512-3oSeUO0TMV67hN1AmbXsK4yaqU7tjiHlbxRDZOpH0KW9+CeX4bRAaX0Anxt0tx2MrpRpWwQaPwIlISEJhYU5Pw==
 
-base64-js@^1.3.1:
+base64-js@^1.2.1, base64-js@^1.3.1:
   version "1.5.1"
   resolved "https://registry.yarnpkg.com/base64-js/-/base64-js-1.5.1.tgz#1b1b440160a5bf7ad40b650f095963481903930a"
   integrity sha512-AKpaYlHn8t4SVbOHCy+b5+KKgvR4vrsD8vbvrbiQJps7fKDTkjkDry6ji0rUJjC0kzbNePLwzxq8iypo41qeWA==
 
 before-after-hook@^2.2.0:
   version "2.2.3"
   resolved "https://registry.yarnpkg.com/before-after-hook/-/before-after-hook-2.2.3.tgz#c51e809c81a4e354084422b9b26bad88249c517c"
@@ -2511,14 +2651,24 @@
   integrity sha512-DJR/VvkAvSZW9bTouZue2sSxDwdTN92uHjqeKVm+0dAqdfNykRzQ95tay8aXMBAAPpUiq4Qcug2L7neoRh2Egw==
 
 csstype@~3.0.3:
   version "3.0.11"
   resolved "https://registry.yarnpkg.com/csstype/-/csstype-3.0.11.tgz#d66700c5eacfac1940deb4e3ee5642792d85cd33"
   integrity sha512-sa6P2wJ+CAbgyy4KFssIb/JNMLxFvKF1pCYCSXS8ZMuqZnMsrxqI2E5sPyoTpxoPU/gVZMzr2zjOfg8GIZOMsw==
 
+d3-color@^3.0.1:
+  version "3.1.0"
+  resolved "https://registry.yarnpkg.com/d3-color/-/d3-color-3.1.0.tgz#395b2833dfac71507f12ac2f7af23bf819de24e2"
+  integrity sha512-zg/chbXyeBtMQ1LbD/WSoW2DpC3I0mpmPdW+ynRTj/x2DAWYrIY7qeZIHidozwV24m4iavr15lNwIwLxRmOxhA==
+
+d3-format@^3.0.1:
+  version "3.1.0"
+  resolved "https://registry.yarnpkg.com/d3-format/-/d3-format-3.1.0.tgz#9260e23a28ea5cb109e93b21a06e24e2ebd55641"
+  integrity sha512-YyUI6AEuY/Wpt8KWLgZHsIU86atmikuoOmCfommt0LYHiQSPjvX2AcFc38PX0CBpr2RCyZhjex+NS/LPOv6YqA==
+
 dargs@^7.0.0:
   version "7.0.0"
   resolved "https://registry.yarnpkg.com/dargs/-/dargs-7.0.0.tgz#04015c41de0bcb69ec84050f3d9be0caf8d6d5cc"
   integrity sha512-2iy1EkLdlBzQGvbweYRFxmFath8+K7+AKB0TlhHWkNuH+TmovaMH/Wp7V7R4u7f4SnX3OgLsU9t1NI9ioDnUpg==
 
 data-urls@^2.0.0:
   version "2.0.0"
@@ -2694,20 +2844,29 @@
   resolved "https://registry.yarnpkg.com/dom-serializer/-/dom-serializer-1.4.1.tgz#de5d41b1aea290215dc45a6dae8adcf1d32e2d30"
   integrity sha512-VHwB3KfrcOOkelEG2ZOfxqLZdfkil8PtJi4P8N2MMXucZq2yLp75ClViUlOVwyoHEDjYU433Aq+5zWP61+RGag==
   dependencies:
     domelementtype "^2.0.1"
     domhandler "^4.2.0"
     entities "^2.0.0"
 
+dom-serializer@^2.0.0:
+  version "2.0.0"
+  resolved "https://registry.yarnpkg.com/dom-serializer/-/dom-serializer-2.0.0.tgz#e41b802e1eedf9f6cae183ce5e622d789d7d8e53"
+  integrity sha512-wIkAryiqt/nV5EQKqQpo3SToSOV9J0DnbJqwK7Wv/Trc92zIAYZ4FlMu+JPFW1DfGFt81ZTCGgDEabffXeLyJg==
+  dependencies:
+    domelementtype "^2.3.0"
+    domhandler "^5.0.2"
+    entities "^4.2.0"
+
 dom4@^2.1.5:
   version "2.1.6"
   resolved "https://registry.yarnpkg.com/dom4/-/dom4-2.1.6.tgz#c90df07134aa0dbd81ed4d6ba1237b36fc164770"
   integrity sha512-JkCVGnN4ofKGbjf5Uvc8mmxaATIErKQKSgACdBXpsQ3fY6DlIpAyWfiBSrGkttATssbDCp3psiAKWXk5gmjycA==
 
-domelementtype@^2.0.1, domelementtype@^2.2.0:
+domelementtype@^2.0.1, domelementtype@^2.2.0, domelementtype@^2.3.0:
   version "2.3.0"
   resolved "https://registry.yarnpkg.com/domelementtype/-/domelementtype-2.3.0.tgz#5c45e8e869952626331d7aab326d01daf65d589d"
   integrity sha512-OLETBj6w0OsagBwdXnPdN0cnMfF9opN69co+7ZrbfPGrdpPVNBUj02spi6B1N7wChLQiPn4CSH/zJvXw56gmHw==
 
 domexception@^4.0.0:
   version "4.0.0"
   resolved "https://registry.yarnpkg.com/domexception/-/domexception-4.0.0.tgz#4ad1be56ccadc86fc76d033353999a8037d03673"
@@ -2718,23 +2877,39 @@
 domhandler@^4.0.0, domhandler@^4.2.0:
   version "4.3.1"
   resolved "https://registry.yarnpkg.com/domhandler/-/domhandler-4.3.1.tgz#8d792033416f59d68bc03a5aa7b018c1ca89279c"
   integrity sha512-GrwoxYN+uWlzO8uhUXRl0P+kHE4GtVPfYzVLcUxPL7KNdHKj66vvlhiweIHqYYXWlw+T8iLMp42Lm67ghw4WMQ==
   dependencies:
     domelementtype "^2.2.0"
 
+domhandler@^5.0.1, domhandler@^5.0.2, domhandler@^5.0.3:
+  version "5.0.3"
+  resolved "https://registry.yarnpkg.com/domhandler/-/domhandler-5.0.3.tgz#cc385f7f751f1d1fc650c21374804254538c7d31"
+  integrity sha512-cgwlv/1iFQiFnU96XXgROh8xTeetsnJiDsTc7TYCLFd9+/WNkIqPTxiM/8pSd8VIrhXGTf1Ny1q1hquVqDJB5w==
+  dependencies:
+    domelementtype "^2.3.0"
+
 domutils@^2.5.2:
   version "2.8.0"
   resolved "https://registry.yarnpkg.com/domutils/-/domutils-2.8.0.tgz#4437def5db6e2d1f5d6ee859bd95ca7d02048135"
   integrity sha512-w96Cjofp72M5IIhpjgobBimYEfoPjx1Vx0BSX9P30WBdZW2WIKU0T1Bd0kz2eNZ9ikjKgHbEyKx8BB6H1L3h3A==
   dependencies:
     dom-serializer "^1.0.1"
     domelementtype "^2.2.0"
     domhandler "^4.2.0"
 
+domutils@^3.0.1:
+  version "3.0.1"
+  resolved "https://registry.yarnpkg.com/domutils/-/domutils-3.0.1.tgz#696b3875238338cb186b6c0612bd4901c89a4f1c"
+  integrity sha512-z08c1l761iKhDFtfXO04C7kTdPBLi41zwOZl00WS8b5eiaebNpY00HKbztwBq+e3vyqWNwWF3mP9YLUeqIrF+Q==
+  dependencies:
+    dom-serializer "^2.0.0"
+    domelementtype "^2.3.0"
+    domhandler "^5.0.1"
+
 dot-prop@6.0.1:
   version "6.0.1"
   resolved "https://registry.yarnpkg.com/dot-prop/-/dot-prop-6.0.1.tgz#fc26b3cf142b9e59b74dbd39ed66ce620c681083"
   integrity sha512-tE7ztYzXHIeyvc7N+hR3oi7FIbf/NIjVP9hmAt3yMXzrQ072/fpjGLx2GxNxGxUl5V73MEqYzioOMoVhGMJ5cA==
   dependencies:
     is-obj "^2.0.0"
 
@@ -2827,14 +3002,19 @@
     ansi-colors "^4.1.1"
 
 entities@^2.0.0:
   version "2.2.0"
   resolved "https://registry.yarnpkg.com/entities/-/entities-2.2.0.tgz#098dc90ebb83d8dffa089d55256b351d34c4da55"
   integrity sha512-p92if5Nz619I0w+akJrLZH0MX0Pb5DX39XOwQTtXSdQQOaYH03S1uIQp4mhOZtAXrxq4ViO67YTiLBo2638o9A==
 
+entities@^4.2.0:
+  version "4.5.0"
+  resolved "https://registry.yarnpkg.com/entities/-/entities-4.5.0.tgz#5d268ea5e7113ec74c4d033b79ea5a35a488fb48"
+  integrity sha512-V0hjH4dGPh9Ao5p0MoRY6BVqtwCjhz6vI5LT8AJ55H+4g9/4vbHx1I54fS0XuclLhDHArPQCiMjDxjaL8fPxhw==
+
 entities@^4.4.0:
   version "4.4.0"
   resolved "https://registry.yarnpkg.com/entities/-/entities-4.4.0.tgz#97bdaba170339446495e653cfd2db78962900174"
   integrity sha512-oYp7156SP8LkeGD0GF85ad1X9Ai79WtRsZ2gxJqtBuzH+98YUV6jkHEKlZkMbcrjJjIVJNIDP/3WL9wQkoPbWA==
 
 env-paths@^2.2.0:
   version "2.2.1"
@@ -3729,14 +3909,24 @@
   integrity sha512-gyyPk6rgonLFEDGoeRgQNaEUvdJ4ktTmmUh/h2t7s+M8oPpIPxgNACWa+6ESR57kXstwqPiCut0V8NRpcwgU7A==
   dependencies:
     domelementtype "^2.0.1"
     domhandler "^4.0.0"
     domutils "^2.5.2"
     entities "^2.0.0"
 
+htmlparser2@^8.0.0:
+  version "8.0.2"
+  resolved "https://registry.yarnpkg.com/htmlparser2/-/htmlparser2-8.0.2.tgz#f002151705b383e62433b5cf466f5b716edaec21"
+  integrity sha512-GYdjWKDkbRLkZ5geuHs5NY1puJ+PXwP7+fHPRz06Eirsb9ugf6d8kkXav6ADhcODhFFPMIXyxkxSuMf3D6NCFA==
+  dependencies:
+    domelementtype "^2.3.0"
+    domhandler "^5.0.3"
+    domutils "^3.0.1"
+    entities "^4.4.0"
+
 http-cache-semantics@^4.1.0:
   version "4.1.1"
   resolved "https://registry.yarnpkg.com/http-cache-semantics/-/http-cache-semantics-4.1.1.tgz#abe02fcb2985460bf0323be664436ec3476a6d5a"
   integrity sha512-er295DKPVsV82j5kw1Gjt+ADA/XYHsajl82cGNQG2eyoPkvgUhX+nDIyelzhIWbbsXP39EHcI6l5tYs2FYqYXQ==
 
 http-proxy-agent@^5.0.0:
   version "5.0.0"
@@ -4181,14 +4371,19 @@
   resolved "https://registry.yarnpkg.com/jest-worker/-/jest-worker-27.5.1.tgz#8d146f0900e8973b106b6f73cc1e9a8cb86f8db0"
   integrity sha512-7vuh85V5cdDofPyxn58nrPjBktZo0u9x1g8WtjQol+jZDaE+fhN+cIvTj11GndBnMnyfrUOG1sZQxCdjKh+DKg==
   dependencies:
     "@types/node" "*"
     merge-stream "^2.0.0"
     supports-color "^8.0.0"
 
+jquery@^3.1.1:
+  version "3.6.4"
+  resolved "https://registry.yarnpkg.com/jquery/-/jquery-3.6.4.tgz#ba065c188142100be4833699852bf7c24dc0252f"
+  integrity sha512-v28EW9DWDFpzcD9O5iyJXg3R3+q+mET5JhnjJzQUZMHOv67bpSIHq81GEYpPNZHG+XXHsfSme3nxp/hndKEcsQ==
+
 js-sdsl@^4.1.4:
   version "4.3.0"
   resolved "https://registry.yarnpkg.com/js-sdsl/-/js-sdsl-4.3.0.tgz#aeefe32a451f7af88425b11fdb5f58c90ae1d711"
   integrity sha512-mifzlm2+5nZ+lEcLJMoBK0/IH/bDg8XnJfd/Wq6IP+xoCjLZsTOnV2QpxlVbX9bMnkl5PdEjNtBJ9Cj1NjifhQ==
 
 "js-tokens@^3.0.0 || ^4.0.0", js-tokens@^4.0.0:
   version "4.0.0"
@@ -4530,21 +4725,28 @@
   version "0.3.0"
   resolved "https://registry.yarnpkg.com/levn/-/levn-0.3.0.tgz#3b09924edf9f083c0490fdd4c0bc4421e04764ee"
   integrity sha512-0OO4y2iOHix2W6ujICbKIaEQXvFQHue65vUG3pb5EUomzPI90z9hsA1VsO/dbIIpC53J8gxM9Q4Oho0jrCM/yA==
   dependencies:
     prelude-ls "~1.1.2"
     type-check "~0.3.2"
 
-lib0@^0.2.31, lib0@^0.2.42, lib0@^0.2.49, lib0@^0.2.52:
+lib0@^0.2.31, lib0@^0.2.42, lib0@^0.2.52:
   version "0.2.67"
   resolved "https://registry.yarnpkg.com/lib0/-/lib0-0.2.67.tgz#c89e09d6af804cff11ad8220ef04a69e8f966d35"
   integrity sha512-/eAwO2Zog4Ar07YAHvgo+mja04tENZDsNYLJuAGv4cl+ss/IL1scjvl0ogrKBGxchCxTWoGX6TOF6B2iDd/gpg==
   dependencies:
     isomorphic.js "^0.2.4"
 
+lib0@^0.2.72:
+  version "0.2.73"
+  resolved "https://registry.yarnpkg.com/lib0/-/lib0-0.2.73.tgz#af7d7ce9ad523fa3e241d437cc3ab1862f9a1f29"
+  integrity sha512-aJJIElCLWnHMcYZPtsM07QoSfHwpxCy4VUzBYGXFYEmh/h2QS5uZNbCCfL0CqnkOE30b7Tp9DVfjXag+3qzZjQ==
+  dependencies:
+    isomorphic.js "^0.2.4"
+
 libnpmaccess@6.0.3:
   version "6.0.3"
   resolved "https://registry.yarnpkg.com/libnpmaccess/-/libnpmaccess-6.0.3.tgz#473cc3e4aadb2bc713419d92e45d23b070d8cded"
   integrity sha512-4tkfUZprwvih2VUZYMozL7EMKgQ5q9VW2NtRyxWtQWlkLTAWHRklcAvBN49CVqEkhUw7vTX2fNgB5LzgUucgYg==
   dependencies:
     aproba "^2.0.0"
     minipass "^3.1.1"
@@ -5114,14 +5316,19 @@
     validate-npm-package-license "^3.0.4"
 
 normalize.css@^8.0.1:
   version "8.0.1"
   resolved "https://registry.yarnpkg.com/normalize.css/-/normalize.css-8.0.1.tgz#9b98a208738b9cc2634caacbc42d131c97487bf3"
   integrity sha512-qizSNPO93t1YUuUhP22btGOo3chcvDFqFaj2TRybP0DMxkHOCTYwp3n34fel4a31ORXy4m1Xq0Gyqpb5m33qIg==
 
+nouislider@15.4.0:
+  version "15.4.0"
+  resolved "https://registry.yarnpkg.com/nouislider/-/nouislider-15.4.0.tgz#ac0d988e9ba59366062e5712e7cd37eb2e48630d"
+  integrity sha512-AV7UMhGhZ4Mj6ToMT812Ib8OJ4tAXR2/Um7C4l4ZvvsqujF0WpQTpqqHJ+9xt4174R7ueQOUrBR4yakJpAIPCA==
+
 npm-bundled@^1.1.1, npm-bundled@^1.1.2:
   version "1.1.2"
   resolved "https://registry.yarnpkg.com/npm-bundled/-/npm-bundled-1.1.2.tgz#944c78789bd739035b70baa2ca5cc32b8d860bc1"
   integrity sha512-x5DHup0SuyQcmL3s7Rx/YQ8sbw/Hzg0rj48eN0dV7hf5cmQq5PXIeioroH3raV1QC1yh3uTYuMThvEQF3iKgGQ==
   dependencies:
     npm-normalize-package-bin "^1.0.1"
 
@@ -6318,14 +6525,26 @@
     is-regex "^1.1.4"
 
 "safer-buffer@>= 2.1.2 < 3", "safer-buffer@>= 2.1.2 < 3.0.0":
   version "2.1.2"
   resolved "https://registry.yarnpkg.com/safer-buffer/-/safer-buffer-2.1.2.tgz#44fa161b0187b9549dd84bb91802f9bd8385cd6a"
   integrity sha512-YZo3K82SD7Riyi0E1EQPojLz7kpepnSQI9IyPbHHg1XXXevb5dJI7tpyN2ADxGcQbHG7vcyRHk0cbwqcQriUtg==
 
+sanitize-html@^2.3:
+  version "2.10.0"
+  resolved "https://registry.yarnpkg.com/sanitize-html/-/sanitize-html-2.10.0.tgz#74d28848dfcf72c39693139131895c78900ab452"
+  integrity sha512-JqdovUd81dG4k87vZt6uA6YhDfWkUGruUu/aPmXLxXi45gZExnt9Bnw/qeQU8oGf82vPyaE0vO4aH0PbobB9JQ==
+  dependencies:
+    deepmerge "^4.2.2"
+    escape-string-regexp "^4.0.0"
+    htmlparser2 "^8.0.0"
+    is-plain-object "^5.0.0"
+    parse-srcset "^1.0.2"
+    postcss "^8.3.11"
+
 sanitize-html@~2.7.3:
   version "2.7.3"
   resolved "https://registry.yarnpkg.com/sanitize-html/-/sanitize-html-2.7.3.tgz#166c868444ee4f9fd7352ac8c63fa86c343fc2bd"
   integrity sha512-jMaHG29ak4miiJ8wgqA1849iInqORgNv7SLfSw9LtfOhEUQ1C0YHKH73R+hgyufBW9ZFeJrb057k9hjlfBCVlw==
   dependencies:
     deepmerge "^4.2.2"
     escape-string-regexp "^4.0.0"
@@ -7060,14 +7279,19 @@
   integrity sha512-61pPlCD9h51VoreyJ0BReideM3MDKMKnh6+V9L08331ipq6Q8OFXZYiqP6n/tbHx4s5I9uRhcye6BrbkizkBDw==
   dependencies:
     call-bind "^1.0.2"
     has-bigints "^1.0.2"
     has-symbols "^1.0.3"
     which-boxed-primitive "^1.0.2"
 
+underscore@>=1.8.3:
+  version "1.13.6"
+  resolved "https://registry.yarnpkg.com/underscore/-/underscore-1.13.6.tgz#04786a1f589dc6c09f761fc5f45b89e935136441"
+  integrity sha512-+A5Sja4HP1M08MaXya7p5LvjuM7K6q/2EaC0+iovj/wOcMsTzMvDFbasi/oSapiwOlt252IqsKqPjCl7huKS0A==
+
 unique-filename@^1.1.1:
   version "1.1.1"
   resolved "https://registry.yarnpkg.com/unique-filename/-/unique-filename-1.1.1.tgz#1d69769369ada0583103a1e6ae87681b56573230"
   integrity sha512-Vmp0jIp2ln35UTXuryvjzkjGdRyf9b2lTXuSYUiPmzRcl3FDtYqAwOnTJkAngD9SWhnoJzDbTKwaOrZ+STtxNQ==
   dependencies:
     unique-slug "^2.0.0"
 
@@ -7556,15 +7780,15 @@
 y-protocols@^1.0.5:
   version "1.0.5"
   resolved "https://registry.yarnpkg.com/y-protocols/-/y-protocols-1.0.5.tgz#91d574250060b29fcac8f8eb5e276fbad594245e"
   integrity sha512-Wil92b7cGk712lRHDqS4T90IczF6RkcvCwAD0A2OPg+adKmOe+nOiT/N2hvpQIWS3zfjmtL4CPaH5sIW1Hkm/A==
   dependencies:
     lib0 "^0.2.42"
 
-y-websocket@^1.3.15:
+y-websocket@^1.4.6:
   version "1.5.0"
   resolved "https://registry.yarnpkg.com/y-websocket/-/y-websocket-1.5.0.tgz#3c13ed205f1553185e1d144eac94150b5b5d55d6"
   integrity sha512-A8AO6XtnQlYwWFytWdkDCeXg4l8ghRTIw5h2YUgUYDmEC9ugWGIwYNW80yadhSFAF7CvuWTEkQNEpevnH6EiZw==
   dependencies:
     lib0 "^0.2.52"
     lodash.debounce "^4.0.8"
     y-protocols "^1.0.5"
@@ -7634,18 +7858,18 @@
   integrity sha512-wH2+dyLt1cCMx91kmfiB8GhHiZPVmfD9PULoWGryiqgvA+uvcR3k1yaDbB+K/bTx/NBiMhpnSTFdeWM6MqROYQ==
   dependencies:
     "@yarnpkg/lockfile" "^1.1.0"
     commander "^9.4.1"
     semver "^7.3.8"
     tslib "^2.4.1"
 
-yjs@^13.5.17, yjs@^13.5.40:
-  version "13.5.50"
-  resolved "https://registry.yarnpkg.com/yjs/-/yjs-13.5.50.tgz#ab0605c677922163c9fe49295d3fd47c04c8e0e9"
-  integrity sha512-Q2KVNfovwjtJV4Yxz+HaFYT6vTYBaFagOSpTL3jbPc7Sbv/My68fLTfPlYy9FmNO87pV8dMBd5XuVar+9WsAWg==
+yjs@^13.5.40:
+  version "13.5.52"
+  resolved "https://registry.yarnpkg.com/yjs/-/yjs-13.5.52.tgz#aec0535e16d45ed4defd6489fffae2b17e30fdb3"
+  integrity sha512-wTajR70VeI6uztpUk4kMcXYHSRzuUlNyJPdBG9NII0EcFf27DwGduZEm3XbP7VSzlGx5n6uenBhOPX+YuPH/tA==
   dependencies:
-    lib0 "^0.2.49"
+    lib0 "^0.2.72"
 
 yocto-queue@^0.1.0:
   version "0.1.0"
   resolved "https://registry.yarnpkg.com/yocto-queue/-/yocto-queue-0.1.0.tgz#0294eb3dee05028d31ee1a5fa2c556a6aaf10a1b"
   integrity sha512-rVksvsnNCdJ/ohGc6xgPwyN8eheCxsiLM8mxuE/t/mOVqJewPuO1miLpTHQiRgTKCLexL4MeAFVagts7HmNZ2Q==
```

### Comparing `jupyterlab_blockly-0.3.0a0/assets/info_full_release.png` & `jupyterlab_blockly-0.3.0a1/assets/info_full_release.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/assets/merge_changelog.png` & `jupyterlab_blockly-0.3.0a1/assets/merge_changelog.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/assets/run_draft_changelog.png` & `jupyterlab_blockly-0.3.0a1/assets/run_draft_changelog.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/assets/run_full_release.png` & `jupyterlab_blockly-0.3.0a1/assets/run_full_release.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/docs/Makefile` & `jupyterlab_blockly-0.3.0a1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/docs/blockly_editor.md` & `jupyterlab_blockly-0.3.0a1/docs/blockly_editor.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/docs/conf.py` & `jupyterlab_blockly-0.3.0a1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/docs/example.jpblockly` & `jupyterlab_blockly-0.3.0a1/docs/example.jpblockly`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/docs/examples.md` & `jupyterlab_blockly-0.3.0a1/docs/examples.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/docs/functions.jpblockly` & `jupyterlab_blockly-0.3.0a1/docs/functions.jpblockly`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/docs/index.rst` & `jupyterlab_blockly-0.3.0a1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/docs/installation.md` & `jupyterlab_blockly-0.3.0a1/docs/installation.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/docs/jupyterlab_integration.md` & `jupyterlab_blockly-0.3.0a1/docs/jupyterlab_integration.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/docs/kernels.md` & `jupyterlab_blockly-0.3.0a1/docs/kernels.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/docs/logic.jpblockly` & `jupyterlab_blockly-0.3.0a1/docs/logic.jpblockly`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/docs/loops.jpblockly` & `jupyterlab_blockly-0.3.0a1/docs/loops.jpblockly`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/docs/make.bat` & `jupyterlab_blockly-0.3.0a1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/docs/other_extensions.md` & `jupyterlab_blockly-0.3.0a1/docs/other_extensions.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/docs/text_and_lists.jpblockly` & `jupyterlab_blockly-0.3.0a1/docs/text_and_lists.jpblockly`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/docs/toolbox.md` & `jupyterlab_blockly-0.3.0a1/docs/toolbox.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/docs/_static/BlocklyOverview.png` & `jupyterlab_blockly-0.3.0a1/docs/_static/BlocklyOverview.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/docs/_static/OverviewBlockly.gif` & `jupyterlab_blockly-0.3.0a1/docs/_static/OverviewBlockly.gif`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/docs/_static/changeKernel.png` & `jupyterlab_blockly-0.3.0a1/docs/_static/changeKernel.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/docs/_static/commentBlock.png` & `jupyterlab_blockly-0.3.0a1/docs/_static/commentBlock.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/docs/_static/creatingVariable.gif` & `jupyterlab_blockly-0.3.0a1/docs/_static/creatingVariable.gif`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/docs/_static/darkBlockly.png` & `jupyterlab_blockly-0.3.0a1/docs/_static/darkBlockly.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/docs/_static/ifBlock.gif` & `jupyterlab_blockly-0.3.0a1/docs/_static/ifBlock.gif`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/docs/_static/openBlocklyEditor.png` & `jupyterlab_blockly-0.3.0a1/docs/_static/openBlocklyEditor.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/docs/_static/openFromLauncher.png` & `jupyterlab_blockly-0.3.0a1/docs/_static/openFromLauncher.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/docs/_static/selectKernel.png` & `jupyterlab_blockly-0.3.0a1/docs/_static/selectKernel.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/docs/_static/shortBlocklyDemo.gif` & `jupyterlab_blockly-0.3.0a1/docs/_static/shortBlocklyDemo.gif`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/docs/_static/toolboxSwitch.png` & `jupyterlab_blockly-0.3.0a1/docs/_static/toolboxSwitch.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/docs/_static/toolboxView.gif` & `jupyterlab_blockly-0.3.0a1/docs/_static/toolboxView.gif`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/examples/example.jpblockly` & `jupyterlab_blockly-0.3.0a1/examples/example.jpblockly`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/examples/functions.jpblockly` & `jupyterlab_blockly-0.3.0a1/examples/functions.jpblockly`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/examples/logic.jpblockly` & `jupyterlab_blockly-0.3.0a1/examples/logic.jpblockly`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/examples/loops.jpblockly` & `jupyterlab_blockly-0.3.0a1/examples/loops.jpblockly`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/examples/text_and_lists.jpblockly` & `jupyterlab_blockly-0.3.0a1/examples/text_and_lists.jpblockly`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/_version.py` & `jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/_version.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/package.json` & `jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/package.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9670833333333333%*

 * *Differences: {"'dependencies'": "{'jupyterlab-blockly': '^0.3.0-alpha.1', '@jupyter-widgets/base': '^6.0.4', "*

 * *                   "'@jupyter-widgets/jupyterlab-manager': '^5.0.7', '@jupyterlab/cells': '^3.6'}",*

 * * "'jupyterlab'": "{'sharedPackages': {'@jupyter-widgets/base': OrderedDict([('bundled', False), "*

 * *                 "('singleton', True)]), '@jupyter-widgets/jupyterlab-manager': "*

 * *                 "OrderedDict([('bundled', False), ('singleton', True)])}, '_build': {'load': "*

 * *                 "'static/remoteEntry. […]*

```diff
@@ -3,25 +3,28 @@
         "email": "",
         "name": "quantstack"
     },
     "bugs": {
         "url": "https://github.com/quantstack/jupyterlab-blockly/issues"
     },
     "dependencies": {
+        "@jupyter-widgets/base": "^6.0.4",
+        "@jupyter-widgets/jupyterlab-manager": "^5.0.7",
         "@jupyterlab/application": "^3.6",
         "@jupyterlab/apputils": "^3.6",
+        "@jupyterlab/cells": "^3.6",
         "@jupyterlab/codeeditor": "^3.6",
         "@jupyterlab/filebrowser": "^3.6",
         "@jupyterlab/launcher": "^3.6",
         "@jupyterlab/mainmenu": "^3.6",
         "@jupyterlab/rendermime": "^3.6",
         "@jupyterlab/settingregistry": "^3.6",
         "@jupyterlab/translation": "^3.6",
         "@jupyterlab/ui-components": "^3.6",
-        "jupyterlab-blockly": "^0.3.0-alpha.0"
+        "jupyterlab-blockly": "^0.3.0-alpha.1"
     },
     "description": "Blockly extension for JupyterLab.",
     "devDependencies": {
         "@jupyterlab/builder": "^3.6",
         "npm-run-all": "^4.1.5",
         "rimraf": "^4.4.0",
         "source-map-loader": "^4.0.1",
@@ -31,20 +34,28 @@
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/quantstack/jupyterlab-blockly",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.64321718d51bd0ccabe6.js",
+            "load": "static/remoteEntry.fd0c0fecc472143c1077.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "../../jupyterlab_blockly/labextension",
         "sharedPackages": {
+            "@jupyter-widgets/base": {
+                "bundled": false,
+                "singleton": true
+            },
+            "@jupyter-widgets/jupyterlab-manager": {
+                "bundled": false,
+                "singleton": true
+            },
             "blockly": {
                 "bundled": true,
                 "singleton": true
             },
             "jupyterlab-blockly": {
                 "bundled": true,
                 "singleton": true
@@ -85,9 +96,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.3.0-alpha.0"
+    "version": "0.3.0-alpha.1"
 }
```

### Comparing `jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/109.624848fd57458c5dd4f0.js` & `jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/109.624848fd57458c5dd4f0.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/109.624848fd57458c5dd4f0.js.map` & `jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/109.624848fd57458c5dd4f0.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/157.921bbfb16083689ff62a.js` & `jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/157.921bbfb16083689ff62a.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/157.921bbfb16083689ff62a.js.map` & `jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/157.921bbfb16083689ff62a.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/168.8383bc2d0a83f2b959fd.js` & `jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/168.8383bc2d0a83f2b959fd.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/168.8383bc2d0a83f2b959fd.js.map` & `jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/168.8383bc2d0a83f2b959fd.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/173.df5a30c1440df850aa82.js` & `jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/173.df5a30c1440df850aa82.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/173.df5a30c1440df850aa82.js.map` & `jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/173.df5a30c1440df850aa82.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/210.35c06ed0583039490182.js` & `jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/210.35c06ed0583039490182.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/210.35c06ed0583039490182.js.map` & `jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/210.35c06ed0583039490182.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/215.82ec42ef5a24d2ff187f.js` & `jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/215.82ec42ef5a24d2ff187f.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/215.82ec42ef5a24d2ff187f.js.map` & `jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/215.82ec42ef5a24d2ff187f.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/216.011d737685936c4c8e1a.js` & `jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/216.751d5114e75a3795211f.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -1,111 +1,116 @@
 "use strict";
 (self.webpackChunkjupyterlab_blockly_extension = self.webpackChunkjupyterlab_blockly_extension || []).push([
     [216], {
         4216: (e, n, t) => {
             t.r(n), t.d(n, {
-                default: () => w
+                default: () => h
             });
-            var o = t(6866),
-                c = t(6591),
-                a = t(5510),
-                r = t(841),
-                s = t(3606),
-                i = t(3535),
-                l = t(1279),
-                d = t(5442),
-                p = t(1598),
-                y = t(5705),
-                g = t(3591);
-            const m = new c.LabIcon({
+            var o = t(5687),
+                c = t(2502),
+                r = t(3033),
+                a = t(2086),
+                i = t(2486),
+                s = t(7280),
+                l = t(1467),
+                d = t(3169),
+                p = t(4038),
+                g = t(5344),
+                y = t(2673),
+                m = t(9814),
+                u = t(8916);
+            const k = new c.LabIcon({
                     name: "blockly:icon/logo",
                     svgstr: '<?xml version="1.0" encoding="UTF-8" standalone="no"?>\n<svg\n   xmlns:dc="http://purl.org/dc/elements/1.1/"\n   xmlns:cc="http://creativecommons.org/ns#"\n   xmlns:rdf="http://www.w3.org/1999/02/22-rdf-syntax-ns#"\n   xmlns:svg="http://www.w3.org/2000/svg"\n   xmlns="http://www.w3.org/2000/svg"\n   xmlns:sodipodi="http://sodipodi.sourceforge.net/DTD/sodipodi-0.dtd"\n   xmlns:inkscape="http://www.inkscape.org/namespaces/inkscape"\n   id="Layer_6"\n   data-name="Layer 6"\n   viewBox="0 0 192 192"\n   version="1.1"\n   sodipodi:docname="logo-only.svg"\n   inkscape:version="0.92.2pre0 (973e216, 2017-07-25)"\n   inkscape:export-filename="/usr/local/google/home/epastern/Documents/Blockly Logos/Square/logo-only.png"\n   inkscape:export-xdpi="96"\n   inkscape:export-ydpi="96">\n  <metadata\n     id="metadata913">\n    <rdf:RDF>\n      <cc:Work\n         rdf:about="">\n        <dc:format>image/svg+xml</dc:format>\n        <dc:type\n           rdf:resource="http://purl.org/dc/dcmitype/StillImage" />\n        <dc:title>blockly-logo</dc:title>\n      </cc:Work>\n    </rdf:RDF>\n  </metadata>\n  <sodipodi:namedview\n     pagecolor="#ffffff"\n     bordercolor="#666666"\n     borderopacity="1"\n     objecttolerance="10"\n     gridtolerance="10"\n     guidetolerance="10"\n     inkscape:pageopacity="0"\n     inkscape:pageshadow="2"\n     inkscape:window-width="2560"\n     inkscape:window-height="1379"\n     id="namedview911"\n     showgrid="false"\n     inkscape:zoom="2"\n     inkscape:cx="239.87642"\n     inkscape:cy="59.742687"\n     inkscape:window-x="0"\n     inkscape:window-y="0"\n     inkscape:window-maximized="1"\n     inkscape:current-layer="g1013" />\n  <defs\n     id="defs902">\n    <style\n       id="style900">.cls-1{fill:#4285f4;}.cls-2{fill:#c8d1db;}</style>\n  </defs>\n  <title\n     id="title904">blockly-logo</title>\n  <g\n     id="g1013"\n     transform="translate(23.500002,-7.9121105)"\n     inkscape:export-xdpi="96"\n     inkscape:export-ydpi="96">\n    <path\n       id="path906"\n       d="M 20.140625,32 C 13.433598,31.994468 7.9944684,37.433598 8,44.140625 V 148.85938 C 7.99447,155.56641 13.433598,161.00553 20.140625,161 h 4.726563 c 2.330826,8.74182 10.245751,14.82585 19.292968,14.83008 C 53.201562,175.81878 61.108176,169.73621 63.4375,161 h 4.841797 15.726562 c 4.418278,0 8,-3.58172 8,-8 V 40 l -8,-8 z"\n       style="fill:#4285f4"\n       inkscape:connector-curvature="0"\n       sodipodi:nodetypes="ccccccccssccc" />\n    <path\n       sodipodi:nodetypes="ccccccccccccccccc"\n       inkscape:connector-curvature="0"\n       id="path908"\n       d="M 80.007812,31.994141 C 79.997147,49.696887 80,67.396525 80,85.109375 L 63.369141,75.710938 C 60.971784,74.358189 58.004891,76.087168 58,78.839844 v 40.621096 c 0.0049,2.75267 2.971786,4.48165 5.369141,3.1289 L 80,113.18945 v 37.5918 2.21875 8 h 8 1.425781 36.054689 c 6.36195,-2.6e-4 11.51927,-5.15758 11.51953,-11.51953 V 43.480469 C 136.97822,37.133775 131.8272,32.000222 125.48047,32 Z"\n       style="fill:#c8d1db" />\n  </g>\n</svg>\n'
                 }),
-                k = "Blockly editor";
-            var u;
-            ! function(e) {
+                w = "Blockly editor";
+            var f;
+
+            function* x(e) {
+                for (const n of e) n instanceof m.WidgetRenderer && (yield n)
+            }! function(e) {
                 e.createNew = "blockly:create-new-blockly-file"
-            }(u || (u = {}));
-            const w = {
+            }(f || (f = {}));
+            const h = {
                 id: "jupyterlab-blocky:plugin",
                 autoStart: !0,
-                requires: [o.ILayoutRestorer, r.IRenderMimeRegistry, s.IEditorServices, i.IFileBrowserFactory, p.ISettingRegistry, d.ITranslator],
-                optional: [l.ILauncher, a.ICommandPalette, y.IMainMenu],
-                provides: g.IBlocklyRegistry,
-                activate: (e, n, t, o, r, s, i, l, d, p) => {
+                requires: [o.ILayoutRestorer, a.IRenderMimeRegistry, i.IEditorServices, s.IFileBrowserFactory, p.ISettingRegistry, d.ITranslator],
+                optional: [l.ILauncher, r.ICommandPalette, g.IMainMenu, y.IJupyterWidgetRegistry],
+                provides: u.IBlocklyRegistry,
+                activate: (e, n, t, o, a, i, s, l, d, p, g) => {
                     console.log("JupyterLab extension jupyterlab-blocky is activated!");
-                    const y = new a.WidgetTracker({
+                    const y = new r.WidgetTracker({
                         namespace: "jupyterlab-blocky"
                     });
                     n && n.restore(y, {
                         command: "docmanager:open",
                         args: e => ({
                             path: e.context.path,
-                            factory: k
+                            factory: w
                         }),
                         name: e => e.context.path
                     });
                     const {
-                        commands: w
-                    } = e, v = new g.BlocklyEditorFactory({
-                        name: k,
+                        commands: h
+                    } = e, v = new u.BlocklyEditorFactory({
+                        name: w,
                         modelName: "text",
                         fileTypes: ["blockly"],
                         defaultFor: ["blockly"],
                         canStartKernel: !0,
                         preferKernel: !0,
                         shutdownOnClose: !0,
                         rendermime: t,
                         mimetypeService: o.mimeTypeService,
-                        translator: i
+                        translator: s
                     });
 
-                    function h(e) {
+                    function b(e) {
                         return e.get("locale").composite
                     }
                     return v.widgetCreated.connect(((e, n) => {
-                        n.title.icon = m, n.context.pathChanged.connect((() => {
+                        n.title.icon = k, n.context.pathChanged.connect((() => {
                             y.save(n)
                         })), y.add(n)
                     })), e.docRegistry.addFileType({
                         name: "blockly",
                         displayName: "Blockly",
                         contentType: "file",
                         fileFormat: "json",
                         extensions: [".jpblockly"],
                         mimeTypes: ["application/json"],
                         icon: c.jsonIcon,
                         iconLabel: "JupyterLab-Blockly"
-                    }), e.docRegistry.addWidgetFactory(v), s.load("@jupyterlab/translation-extension:plugin").then((e => {
-                        const n = h(e);
-                        e.changed.connect(h);
+                    }), e.docRegistry.addWidgetFactory(v), i.load("@jupyterlab/translation-extension:plugin").then((e => {
+                        const n = b(e);
+                        e.changed.connect(b);
                         const t = n[n.length - 2].toUpperCase() + n[n.length - 1].toLowerCase();
                         console.log(`Current Language : '${t}'`), v.registry.setlanguage(t)
-                    })), w.addCommand(u.createNew, {
+                    })), h.addCommand(f.createNew, {
                         label: e => e.isPalette ? "New Blockly Editor" : "Blockly Editor",
                         caption: "Create a new Blockly Editor",
-                        icon: e => e.isPalette ? null : m,
+                        icon: e => e.isPalette ? null : k,
                         execute: async e => {
-                            const n = e.cwd || r.tracker.currentWidget.model.path,
-                                t = await w.execute("docmanager:new-untitled", {
+                            const n = e.cwd || a.tracker.currentWidget.model.path,
+                                t = await h.execute("docmanager:new-untitled", {
                                     path: n,
                                     type: "file",
                                     ext: ".jpblockly"
                                 });
-                            return w.execute("docmanager:open", {
+                            return h.execute("docmanager:open", {
                                 path: t.path,
-                                factory: k
+                                factory: w
                             })
                         }
                     }), l && l.add({
-                        command: u.createNew,
+                        command: f.createNew,
                         category: "Other",
                         rank: 1
                     }), d && d.addItem({
-                        command: u.createNew,
+                        command: f.createNew,
                         args: {
                             isPalette: !0
                         },
                         category: "Blockly editor"
                     }), p && p.kernelMenu.kernelUsers.add({
                         tracker: y,
                         interruptKernel: e => {
@@ -120,14 +125,18 @@
                         },
                         restartKernel: e => {
                             var n;
                             const t = null === (n = e.context.sessionContext.session) || void 0 === n ? void 0 : n.kernel;
                             return t ? t.restart() : Promise.resolve(void 0)
                         },
                         shutdownKernel: e => e.context.sessionContext.shutdown()
-                    }), v.registry
+                    }), g && (y.forEach((e => {
+                        (0, m.registerWidgetManager)(e.context, e.content.rendermime, x([e.content.cell]))
+                    })), y.widgetAdded.connect(((e, n) => {
+                        (0, m.registerWidgetManager)(n.context, n.content.rendermime, x([n.content.cell]))
+                    }))), v.registry
                 }
             }
         }
     }
 ]);
-//# sourceMappingURL=216.011d737685936c4c8e1a.js.map?v=011d737685936c4c8e1a
+//# sourceMappingURL=216.751d5114e75a3795211f.js.map?v=751d5114e75a3795211f
```

### Comparing `jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/216.011d737685936c4c8e1a.js.map` & `jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/216.751d5114e75a3795211f.js.map`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.814885496183206%*

 * *Differences: {"'file'": "'216.751d5114e75a3795211f.js?v=751d5114e75a3795211f'",*

 * * "'mappings'": "'+SAAA,MCEaA,EAAe,IAAI,EAAAC,QAAQ,CACpCC,KAAM,oBACNC,ODJJ,o+FEkBMC,EAAU,iBAEhB,IAAIC,EAwLJ,SAAUC,EAAgBC,GACtB,IAAK,MAAMC,KAAKD,EACRC,aAAa,EAAAC,uBACPD,EAGlB,EA7LA,SAAWH,GACPA,EAAWK,UAAY,iCAC1B,CAFD,CAEGL,IAAeA,EAAa,CAAC,IA4LhC,QApLe,CACXM,GAAI,2BACJC,WAAW,EACXC,SAAU,CACN,EAAAC,gBACA,EAAAC,oBACA,EAAAC,gBACA,EAAAC,oBACA,EAAAC,iBACA,EAAAC,aAEJC,SAAU,CAAC,EAAAC,UAAW,EAAAC,gBAAiB,EAAAC,UAAW,EAAAC,wBAClDC,SAAU,EAAAC,iBACVC,SAAU,CAA […]*

```diff
@@ -1,44 +1,50 @@
 {
-    "file": "216.011d737685936c4c8e1a.js?v=011d737685936c4c8e1a",
-    "mappings": "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",
+    "file": "216.751d5114e75a3795211f.js?v=751d5114e75a3795211f",
+    "mappings": "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",
     "names": [
         "blockly_icon",
         "LabIcon",
         "name",
         "svgstr",
         "FACTORY",
         "CommandIDs",
+        "widgetRenderers",
+        "cells",
+        "w",
+        "WidgetRenderer",
         "createNew",
         "id",
         "autoStart",
         "requires",
         "ILayoutRestorer",
         "IRenderMimeRegistry",
         "IEditorServices",
         "IFileBrowserFactory",
         "ISettingRegistry",
         "ITranslator",
         "optional",
         "ILauncher",
         "ICommandPalette",
         "IMainMenu",
+        "IJupyterWidgetRegistry",
         "provides",
         "IBlocklyRegistry",
         "activate",
         "app",
         "restorer",
         "rendermime",
         "editorServices",
         "browserFactory",
         "settings",
         "translator",
         "launcher",
         "palette",
         "mainMenu",
+        "widgetRegistry",
         "console",
         "log",
         "tracker",
         "WidgetTracker",
         "namespace",
         "restore",
         "command",
@@ -116,22 +122,28 @@
         "Promise",
         "resolve",
         "reconnectToKernel",
         "reconnect",
         "restartKernel",
         "restart",
         "shutdownKernel",
-        "shutdown"
+        "shutdown",
+        "forEach",
+        "panel",
+        "registerWidgetManager",
+        "content",
+        "cell",
+        "widgetAdded"
     ],
     "sourceRoot": "",
     "sources": [
         "webpack://jupyterlab-blockly-extension/./style/icons/blockly_logo.svg",
         "webpack://jupyterlab-blockly-extension/./lib/icons.js",
         "webpack://jupyterlab-blockly-extension/./lib/index.js"
     ],
     "sourcesContent": [
         "export default \"<?xml version=\\\"1.0\\\" encoding=\\\"UTF-8\\\" standalone=\\\"no\\\"?>\\n<svg\\n   xmlns:dc=\\\"http://purl.org/dc/elements/1.1/\\\"\\n   xmlns:cc=\\\"http://creativecommons.org/ns#\\\"\\n   xmlns:rdf=\\\"http://www.w3.org/1999/02/22-rdf-syntax-ns#\\\"\\n   xmlns:svg=\\\"http://www.w3.org/2000/svg\\\"\\n   xmlns=\\\"http://www.w3.org/2000/svg\\\"\\n   xmlns:sodipodi=\\\"http://sodipodi.sourceforge.net/DTD/sodipodi-0.dtd\\\"\\n   xmlns:inkscape=\\\"http://www.inkscape.org/namespaces/inkscape\\\"\\n   id=\\\"Layer_6\\\"\\n   data-name=\\\"Layer 6\\\"\\n   viewBox=\\\"0 0 192 192\\\"\\n   version=\\\"1.1\\\"\\n   sodipodi:docname=\\\"logo-only.svg\\\"\\n   inkscape:version=\\\"0.92.2pre0 (973e216, 2017-07-25)\\\"\\n   inkscape:export-filename=\\\"/usr/local/google/home/epastern/Documents/Blockly Logos/Square/logo-only.png\\\"\\n   inkscape:export-xdpi=\\\"96\\\"\\n   inkscape:export-ydpi=\\\"96\\\">\\n  <metadata\\n     id=\\\"metadata913\\\">\\n    <rdf:RDF>\\n      <cc:Work\\n         rdf:about=\\\"\\\">\\n        <dc:format>image/svg+xml</dc:format>\\n        <dc:type\\n           rdf:resource=\\\"http://purl.org/dc/dcmitype/StillImage\\\" />\\n        <dc:title>blockly-logo</dc:title>\\n      </cc:Work>\\n    </rdf:RDF>\\n  </metadata>\\n  <sodipodi:namedview\\n     pagecolor=\\\"#ffffff\\\"\\n     bordercolor=\\\"#666666\\\"\\n     borderopacity=\\\"1\\\"\\n     objecttolerance=\\\"10\\\"\\n     gridtolerance=\\\"10\\\"\\n     guidetolerance=\\\"10\\\"\\n     inkscape:pageopacity=\\\"0\\\"\\n     inkscape:pageshadow=\\\"2\\\"\\n     inkscape:window-width=\\\"2560\\\"\\n     inkscape:window-height=\\\"1379\\\"\\n     id=\\\"namedview911\\\"\\n     showgrid=\\\"false\\\"\\n     inkscape:zoom=\\\"2\\\"\\n     inkscape:cx=\\\"239.87642\\\"\\n     inkscape:cy=\\\"59.742687\\\"\\n     inkscape:window-x=\\\"0\\\"\\n     inkscape:window-y=\\\"0\\\"\\n     inkscape:window-maximized=\\\"1\\\"\\n     inkscape:current-layer=\\\"g1013\\\" />\\n  <defs\\n     id=\\\"defs902\\\">\\n    <style\\n       id=\\\"style900\\\">.cls-1{fill:#4285f4;}.cls-2{fill:#c8d1db;}</style>\\n  </defs>\\n  <title\\n     id=\\\"title904\\\">blockly-logo</title>\\n  <g\\n     id=\\\"g1013\\\"\\n     transform=\\\"translate(23.500002,-7.9121105)\\\"\\n     inkscape:export-xdpi=\\\"96\\\"\\n     inkscape:export-ydpi=\\\"96\\\">\\n    <path\\n       id=\\\"path906\\\"\\n       d=\\\"M 20.140625,32 C 13.433598,31.994468 7.9944684,37.433598 8,44.140625 V 148.85938 C 7.99447,155.56641 13.433598,161.00553 20.140625,161 h 4.726563 c 2.330826,8.74182 10.245751,14.82585 19.292968,14.83008 C 53.201562,175.81878 61.108176,169.73621 63.4375,161 h 4.841797 15.726562 c 4.418278,0 8,-3.58172 8,-8 V 40 l -8,-8 z\\\"\\n       style=\\\"fill:#4285f4\\\"\\n       inkscape:connector-curvature=\\\"0\\\"\\n       sodipodi:nodetypes=\\\"ccccccccssccc\\\" />\\n    <path\\n       sodipodi:nodetypes=\\\"ccccccccccccccccc\\\"\\n       inkscape:connector-curvature=\\\"0\\\"\\n       id=\\\"path908\\\"\\n       d=\\\"M 80.007812,31.994141 C 79.997147,49.696887 80,67.396525 80,85.109375 L 63.369141,75.710938 C 60.971784,74.358189 58.004891,76.087168 58,78.839844 v 40.621096 c 0.0049,2.75267 2.971786,4.48165 5.369141,3.1289 L 80,113.18945 v 37.5918 2.21875 8 h 8 1.425781 36.054689 c 6.36195,-2.6e-4 11.51927,-5.15758 11.51953,-11.51953 V 43.480469 C 136.97822,37.133775 131.8272,32.000222 125.48047,32 Z\\\"\\n       style=\\\"fill:#c8d1db\\\" />\\n  </g>\\n</svg>\\n\";",
         "import { LabIcon } from '@jupyterlab/ui-components';\nimport blockly_logo from '/style/icons/blockly_logo.svg';\nexport const blockly_icon = new LabIcon({\n    name: 'blockly:icon/logo',\n    svgstr: blockly_logo\n});\n//# sourceMappingURL=icons.js.map",
-        "import { ILayoutRestorer } from '@jupyterlab/application';\nimport { jsonIcon } from '@jupyterlab/ui-components';\nimport { WidgetTracker, ICommandPalette } from '@jupyterlab/apputils';\nimport { IRenderMimeRegistry } from '@jupyterlab/rendermime';\nimport { IEditorServices } from '@jupyterlab/codeeditor';\nimport { IFileBrowserFactory } from '@jupyterlab/filebrowser';\nimport { ILauncher } from '@jupyterlab/launcher';\nimport { ITranslator } from '@jupyterlab/translation';\nimport { ISettingRegistry } from '@jupyterlab/settingregistry';\nimport { IMainMenu } from '@jupyterlab/mainmenu';\nimport { BlocklyEditorFactory } from 'jupyterlab-blockly';\nimport { IBlocklyRegistry } from 'jupyterlab-blockly';\nimport { blockly_icon } from './icons';\n/**\n * The name of the factory that creates the editor widgets.\n */\nconst FACTORY = 'Blockly editor';\nconst PALETTE_CATEGORY = 'Blockly editor';\nvar CommandIDs;\n(function (CommandIDs) {\n    CommandIDs.createNew = 'blockly:create-new-blockly-file';\n})(CommandIDs || (CommandIDs = {}));\n/**\n * The id of the translation plugin.\n */\nconst PLUGIN_ID = '@jupyterlab/translation-extension:plugin';\n/**\n * Initialization data for the jupyterlab-blocky extension.\n */\nconst plugin = {\n    id: 'jupyterlab-blocky:plugin',\n    autoStart: true,\n    requires: [\n        ILayoutRestorer,\n        IRenderMimeRegistry,\n        IEditorServices,\n        IFileBrowserFactory,\n        ISettingRegistry,\n        ITranslator\n    ],\n    optional: [ILauncher, ICommandPalette, IMainMenu],\n    provides: IBlocklyRegistry,\n    activate: (app, restorer, rendermime, editorServices, browserFactory, settings, translator, launcher, palette, mainMenu) => {\n        console.log('JupyterLab extension jupyterlab-blocky is activated!');\n        // Namespace for the tracker\n        const namespace = 'jupyterlab-blocky';\n        // Creating the tracker for the document\n        const tracker = new WidgetTracker({ namespace });\n        // Handle state restoration.\n        if (restorer) {\n            // When restoring the app, if the document was open, reopen it\n            restorer.restore(tracker, {\n                command: 'docmanager:open',\n                args: widget => ({ path: widget.context.path, factory: FACTORY }),\n                name: widget => widget.context.path\n            });\n        }\n        const { commands } = app;\n        // Creating the widget factory to register it so the document manager knows about\n        // our new DocumentWidget\n        const widgetFactory = new BlocklyEditorFactory({\n            name: FACTORY,\n            modelName: 'text',\n            fileTypes: ['blockly'],\n            defaultFor: ['blockly'],\n            // Kernel options, in this case we need to execute the code generated\n            // in the blockly editor. The best way would be to use kernels, for\n            // that reason, we tell the widget factory to start a kernel session\n            // when opening the editor, and close the session when closing the editor.\n            canStartKernel: true,\n            preferKernel: true,\n            shutdownOnClose: true,\n            // The rendermime instance, necessary to render the outputs\n            // after a code execution. And the mimeType service to get the\n            // mimeType from the kernel language\n            rendermime: rendermime,\n            mimetypeService: editorServices.mimeTypeService,\n            // The translator instance, used for the internalization of the plugin.\n            translator: translator\n        });\n        // Add the widget to the tracker when it's created\n        widgetFactory.widgetCreated.connect((sender, widget) => {\n            // Adding the Blockly icon for the widget so it appears next to the file name.\n            widget.title.icon = blockly_icon;\n            // Notify the instance tracker if restore data needs to update.\n            widget.context.pathChanged.connect(() => {\n                tracker.save(widget);\n            });\n            tracker.add(widget);\n        });\n        // Registering the file type\n        app.docRegistry.addFileType({\n            name: 'blockly',\n            displayName: 'Blockly',\n            contentType: 'file',\n            fileFormat: 'json',\n            extensions: ['.jpblockly'],\n            mimeTypes: ['application/json'],\n            icon: jsonIcon,\n            iconLabel: 'JupyterLab-Blockly'\n        });\n        // Registering the widget factory\n        app.docRegistry.addWidgetFactory(widgetFactory);\n        function getSetting(setting) {\n            // Read the settings and convert to the correct type\n            const currentLocale = setting.get('locale').composite;\n            return currentLocale;\n        }\n        // Wait for the application to be restored and\n        // for the settings for this plugin to be loaded\n        settings.load(PLUGIN_ID).then(setting => {\n            // Read the settings\n            const currentLocale = getSetting(setting);\n            // Listen for our plugin setting changes using Signal\n            setting.changed.connect(getSetting);\n            // Get new language and call the function that modifies the language name accordingly.\n            // Also, make the transformation to have the name of the language package as in Blockly.\n            const language = currentLocale[currentLocale.length - 2].toUpperCase() +\n                currentLocale[currentLocale.length - 1].toLowerCase();\n            console.log(`Current Language : '${language}'`);\n            // Transmitting the current language to the manager.\n            widgetFactory.registry.setlanguage(language);\n        });\n        commands.addCommand(CommandIDs.createNew, {\n            label: args => args['isPalette'] ? 'New Blockly Editor' : 'Blockly Editor',\n            caption: 'Create a new Blockly Editor',\n            icon: args => (args['isPalette'] ? null : blockly_icon),\n            execute: async (args) => {\n                // Get the directory in which the Blockly file must be created;\n                // otherwise take the current filebrowser directory\n                const cwd = args['cwd'] || browserFactory.tracker.currentWidget.model.path;\n                // Create a new untitled Blockly file\n                const model = await commands.execute('docmanager:new-untitled', {\n                    path: cwd,\n                    type: 'file',\n                    ext: '.jpblockly'\n                });\n                // Open the newly created file with the 'Editor'\n                return commands.execute('docmanager:open', {\n                    path: model.path,\n                    factory: FACTORY\n                });\n            }\n        });\n        // Add the command to the launcher\n        if (launcher) {\n            launcher.add({\n                command: CommandIDs.createNew,\n                category: 'Other',\n                rank: 1\n            });\n        }\n        // Add the command to the palette\n        if (palette) {\n            palette.addItem({\n                command: CommandIDs.createNew,\n                args: { isPalette: true },\n                category: PALETTE_CATEGORY\n            });\n        }\n        // Add the command to the main menu\n        if (mainMenu) {\n            mainMenu.kernelMenu.kernelUsers.add({\n                tracker,\n                interruptKernel: current => {\n                    var _a;\n                    const kernel = (_a = current.context.sessionContext.session) === null || _a === void 0 ? void 0 : _a.kernel;\n                    if (kernel) {\n                        return kernel.interrupt();\n                    }\n                    return Promise.resolve(void 0);\n                },\n                reconnectToKernel: current => {\n                    var _a;\n                    const kernel = (_a = current.context.sessionContext.session) === null || _a === void 0 ? void 0 : _a.kernel;\n                    if (kernel) {\n                        return kernel.reconnect();\n                    }\n                    return Promise.resolve(void 0);\n                },\n                restartKernel: current => {\n                    var _a;\n                    const kernel = (_a = current.context.sessionContext.session) === null || _a === void 0 ? void 0 : _a.kernel;\n                    if (kernel) {\n                        return kernel.restart();\n                    }\n                    return Promise.resolve(void 0);\n                },\n                shutdownKernel: current => current.context.sessionContext.shutdown()\n            });\n        }\n        return widgetFactory.registry;\n    }\n};\nexport default plugin;\n//# sourceMappingURL=index.js.map"
+        "import { ILayoutRestorer } from '@jupyterlab/application';\nimport { jsonIcon } from '@jupyterlab/ui-components';\nimport { WidgetTracker, ICommandPalette } from '@jupyterlab/apputils';\nimport { IRenderMimeRegistry } from '@jupyterlab/rendermime';\nimport { IEditorServices } from '@jupyterlab/codeeditor';\nimport { IFileBrowserFactory } from '@jupyterlab/filebrowser';\nimport { ILauncher } from '@jupyterlab/launcher';\nimport { ITranslator } from '@jupyterlab/translation';\nimport { ISettingRegistry } from '@jupyterlab/settingregistry';\nimport { IMainMenu } from '@jupyterlab/mainmenu';\nimport { IJupyterWidgetRegistry } from '@jupyter-widgets/base';\nimport { WidgetRenderer, registerWidgetManager } from '@jupyter-widgets/jupyterlab-manager';\nimport { BlocklyEditorFactory } from 'jupyterlab-blockly';\nimport { IBlocklyRegistry } from 'jupyterlab-blockly';\nimport { blockly_icon } from './icons';\n/**\n * The name of the factory that creates the editor widgets.\n */\nconst FACTORY = 'Blockly editor';\nconst PALETTE_CATEGORY = 'Blockly editor';\nvar CommandIDs;\n(function (CommandIDs) {\n    CommandIDs.createNew = 'blockly:create-new-blockly-file';\n})(CommandIDs || (CommandIDs = {}));\n/**\n * The id of the translation plugin.\n */\nconst PLUGIN_ID = '@jupyterlab/translation-extension:plugin';\n/**\n * Initialization data for the jupyterlab-blocky extension.\n */\nconst plugin = {\n    id: 'jupyterlab-blocky:plugin',\n    autoStart: true,\n    requires: [\n        ILayoutRestorer,\n        IRenderMimeRegistry,\n        IEditorServices,\n        IFileBrowserFactory,\n        ISettingRegistry,\n        ITranslator\n    ],\n    optional: [ILauncher, ICommandPalette, IMainMenu, IJupyterWidgetRegistry],\n    provides: IBlocklyRegistry,\n    activate: (app, restorer, rendermime, editorServices, browserFactory, settings, translator, launcher, palette, mainMenu, widgetRegistry) => {\n        console.log('JupyterLab extension jupyterlab-blocky is activated!');\n        // Namespace for the tracker\n        const namespace = 'jupyterlab-blocky';\n        // Creating the tracker for the document\n        const tracker = new WidgetTracker({ namespace });\n        // Handle state restoration.\n        if (restorer) {\n            // When restoring the app, if the document was open, reopen it\n            restorer.restore(tracker, {\n                command: 'docmanager:open',\n                args: widget => ({ path: widget.context.path, factory: FACTORY }),\n                name: widget => widget.context.path\n            });\n        }\n        const { commands } = app;\n        // Creating the widget factory to register it so the document manager knows about\n        // our new DocumentWidget\n        const widgetFactory = new BlocklyEditorFactory({\n            name: FACTORY,\n            modelName: 'text',\n            fileTypes: ['blockly'],\n            defaultFor: ['blockly'],\n            // Kernel options, in this case we need to execute the code generated\n            // in the blockly editor. The best way would be to use kernels, for\n            // that reason, we tell the widget factory to start a kernel session\n            // when opening the editor, and close the session when closing the editor.\n            canStartKernel: true,\n            preferKernel: true,\n            shutdownOnClose: true,\n            // The rendermime instance, necessary to render the outputs\n            // after a code execution. And the mimeType service to get the\n            // mimeType from the kernel language\n            rendermime: rendermime,\n            mimetypeService: editorServices.mimeTypeService,\n            // The translator instance, used for the internalization of the plugin.\n            translator: translator\n        });\n        // Add the widget to the tracker when it's created\n        widgetFactory.widgetCreated.connect((sender, widget) => {\n            // Adding the Blockly icon for the widget so it appears next to the file name.\n            widget.title.icon = blockly_icon;\n            // Notify the instance tracker if restore data needs to update.\n            widget.context.pathChanged.connect(() => {\n                tracker.save(widget);\n            });\n            tracker.add(widget);\n        });\n        // Registering the file type\n        app.docRegistry.addFileType({\n            name: 'blockly',\n            displayName: 'Blockly',\n            contentType: 'file',\n            fileFormat: 'json',\n            extensions: ['.jpblockly'],\n            mimeTypes: ['application/json'],\n            icon: jsonIcon,\n            iconLabel: 'JupyterLab-Blockly'\n        });\n        // Registering the widget factory\n        app.docRegistry.addWidgetFactory(widgetFactory);\n        function getSetting(setting) {\n            // Read the settings and convert to the correct type\n            const currentLocale = setting.get('locale').composite;\n            return currentLocale;\n        }\n        // Wait for the application to be restored and\n        // for the settings for this plugin to be loaded\n        settings.load(PLUGIN_ID).then(setting => {\n            // Read the settings\n            const currentLocale = getSetting(setting);\n            // Listen for our plugin setting changes using Signal\n            setting.changed.connect(getSetting);\n            // Get new language and call the function that modifies the language name accordingly.\n            // Also, make the transformation to have the name of the language package as in Blockly.\n            const language = currentLocale[currentLocale.length - 2].toUpperCase() +\n                currentLocale[currentLocale.length - 1].toLowerCase();\n            console.log(`Current Language : '${language}'`);\n            // Transmitting the current language to the manager.\n            widgetFactory.registry.setlanguage(language);\n        });\n        commands.addCommand(CommandIDs.createNew, {\n            label: args => args['isPalette'] ? 'New Blockly Editor' : 'Blockly Editor',\n            caption: 'Create a new Blockly Editor',\n            icon: args => (args['isPalette'] ? null : blockly_icon),\n            execute: async (args) => {\n                // Get the directory in which the Blockly file must be created;\n                // otherwise take the current filebrowser directory\n                const cwd = args['cwd'] || browserFactory.tracker.currentWidget.model.path;\n                // Create a new untitled Blockly file\n                const model = await commands.execute('docmanager:new-untitled', {\n                    path: cwd,\n                    type: 'file',\n                    ext: '.jpblockly'\n                });\n                // Open the newly created file with the 'Editor'\n                return commands.execute('docmanager:open', {\n                    path: model.path,\n                    factory: FACTORY\n                });\n            }\n        });\n        // Add the command to the launcher\n        if (launcher) {\n            launcher.add({\n                command: CommandIDs.createNew,\n                category: 'Other',\n                rank: 1\n            });\n        }\n        // Add the command to the palette\n        if (palette) {\n            palette.addItem({\n                command: CommandIDs.createNew,\n                args: { isPalette: true },\n                category: PALETTE_CATEGORY\n            });\n        }\n        // Add the command to the main menu\n        if (mainMenu) {\n            mainMenu.kernelMenu.kernelUsers.add({\n                tracker,\n                interruptKernel: current => {\n                    var _a;\n                    const kernel = (_a = current.context.sessionContext.session) === null || _a === void 0 ? void 0 : _a.kernel;\n                    if (kernel) {\n                        return kernel.interrupt();\n                    }\n                    return Promise.resolve(void 0);\n                },\n                reconnectToKernel: current => {\n                    var _a;\n                    const kernel = (_a = current.context.sessionContext.session) === null || _a === void 0 ? void 0 : _a.kernel;\n                    if (kernel) {\n                        return kernel.reconnect();\n                    }\n                    return Promise.resolve(void 0);\n                },\n                restartKernel: current => {\n                    var _a;\n                    const kernel = (_a = current.context.sessionContext.session) === null || _a === void 0 ? void 0 : _a.kernel;\n                    if (kernel) {\n                        return kernel.restart();\n                    }\n                    return Promise.resolve(void 0);\n                },\n                shutdownKernel: current => current.context.sessionContext.shutdown()\n            });\n        }\n        if (widgetRegistry) {\n            tracker.forEach(panel => {\n                registerWidgetManager(panel.context, panel.content.rendermime, widgetRenderers([panel.content.cell]));\n            });\n            tracker.widgetAdded.connect((sender, panel) => {\n                registerWidgetManager(panel.context, panel.content.rendermime, widgetRenderers([panel.content.cell]));\n            });\n        }\n        return widgetFactory.registry;\n    }\n};\nfunction* widgetRenderers(cells) {\n    for (const w of cells) {\n        if (w instanceof WidgetRenderer) {\n            yield w;\n        }\n    }\n}\nexport default plugin;\n//# sourceMappingURL=index.js.map"
     ],
     "version": 3
 }
```

### Comparing `jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/232.d5cb8a2dcc0d34fabd8a.js` & `jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/232.d5cb8a2dcc0d34fabd8a.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/232.d5cb8a2dcc0d34fabd8a.js.map` & `jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/232.d5cb8a2dcc0d34fabd8a.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/268.4eaefedf266ea50fd6df.js` & `jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/268.4eaefedf266ea50fd6df.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/268.4eaefedf266ea50fd6df.js.map` & `jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/268.4eaefedf266ea50fd6df.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/31.418331b4a22dffe518b4.js` & `jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/31.418331b4a22dffe518b4.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/31.418331b4a22dffe518b4.js.map` & `jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/31.418331b4a22dffe518b4.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/326.f8d1ef211f999b0b3dca.js` & `jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/326.f8d1ef211f999b0b3dca.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/326.f8d1ef211f999b0b3dca.js.map` & `jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/326.f8d1ef211f999b0b3dca.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/382.0016faf875cb665ac9b2.js` & `jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/382.0016faf875cb665ac9b2.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/382.0016faf875cb665ac9b2.js.map` & `jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/382.0016faf875cb665ac9b2.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/410.941cb48faa5e2d568b13.js` & `jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/410.941cb48faa5e2d568b13.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/410.941cb48faa5e2d568b13.js.map` & `jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/410.941cb48faa5e2d568b13.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/428.cb1cafd5e6ba8a81b05a.js` & `jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/428.cb1cafd5e6ba8a81b05a.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/428.cb1cafd5e6ba8a81b05a.js.map` & `jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/428.cb1cafd5e6ba8a81b05a.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/513.5646d474a0e4d9613886.js` & `jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/513.5646d474a0e4d9613886.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/513.5646d474a0e4d9613886.js.map` & `jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/513.5646d474a0e4d9613886.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/533.606434cc067b99350123.js` & `jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/533.606434cc067b99350123.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/533.606434cc067b99350123.js.map` & `jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/533.606434cc067b99350123.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/549.dbfa5147d8fec7e5a76f.js` & `jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/549.dbfa5147d8fec7e5a76f.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/549.dbfa5147d8fec7e5a76f.js.map` & `jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/549.dbfa5147d8fec7e5a76f.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/588.3e52218ff8bfd1512578.js` & `jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/588.3e52218ff8bfd1512578.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/588.3e52218ff8bfd1512578.js.map` & `jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/588.3e52218ff8bfd1512578.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/593.526fcc348e87fac11681.js` & `jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/593.526fcc348e87fac11681.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/593.526fcc348e87fac11681.js.map` & `jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/593.526fcc348e87fac11681.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/617.c198d75d062c9be68fef.js` & `jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/617.c198d75d062c9be68fef.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/617.c198d75d062c9be68fef.js.map` & `jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/617.c198d75d062c9be68fef.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/619.84aef6ceee0a82ac27ee.js` & `jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/619.84aef6ceee0a82ac27ee.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/619.84aef6ceee0a82ac27ee.js.map` & `jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/619.84aef6ceee0a82ac27ee.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/627.5da93440391d7167f88d.js` & `jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/627.5da93440391d7167f88d.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/627.5da93440391d7167f88d.js.map` & `jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/627.5da93440391d7167f88d.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/643.34f4f43b70e246a962a8.js` & `jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/643.34f4f43b70e246a962a8.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/643.34f4f43b70e246a962a8.js.map` & `jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/643.34f4f43b70e246a962a8.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/647.d729bd3d64d38278f913.js` & `jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/647.d729bd3d64d38278f913.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/647.d729bd3d64d38278f913.js.map` & `jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/647.d729bd3d64d38278f913.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/655.13bd86e04776bccddcee.js` & `jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/655.13bd86e04776bccddcee.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/655.13bd86e04776bccddcee.js.map` & `jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/655.13bd86e04776bccddcee.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/671.5cc50d235d821a731440.js` & `jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/671.5cc50d235d821a731440.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/671.5cc50d235d821a731440.js.map` & `jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/671.5cc50d235d821a731440.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/693.91ee036f7a5bf0e5a1b0.js` & `jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/693.91ee036f7a5bf0e5a1b0.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/693.91ee036f7a5bf0e5a1b0.js.map` & `jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/693.91ee036f7a5bf0e5a1b0.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/698.48373f0b62bef71acebe.js` & `jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/698.48373f0b62bef71acebe.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/698.48373f0b62bef71acebe.js.map` & `jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/698.48373f0b62bef71acebe.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/704.cf482c52df64c1afcb10.js` & `jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/704.cf482c52df64c1afcb10.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/704.cf482c52df64c1afcb10.js.map` & `jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/704.cf482c52df64c1afcb10.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/835.cbd12870eccd44d69cf0.js` & `jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/835.6f7e7b701fee67a1ec53.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -9,20 +9,20 @@
                 BlocklyManager: () => K,
                 BlocklyPanel: () => v,
                 BlocklyRegistry: () => T,
                 IBlocklyRegistry: () => M,
                 THEME: () => m,
                 TOOLBOX: () => h
             });
-            var o = n(4379),
-                l = n(6591),
-                a = n(1431),
+            var o = n(819),
+                l = n(2502),
+                a = n(8832),
                 s = n(1840),
-                i = n(5510),
-                r = n(1952),
+                i = n(3033),
+                r = n(2191),
                 c = n(8918),
                 d = n(1041);
             const h = {
                     kind: "categoryToolbox",
                     contents: [{
                         kind: "category",
                         name: "Logic",
@@ -298,14 +298,17 @@
                         renderer: a.SplitPanel.defaultRenderer,
                         orientation: "vertical"
                     }), this._manager = e, this._sessionContext = t, this._host = new a.Widget, this._cell = new r.CodeCell({
                         model: new r.CodeCellModel({}),
                         rendermime: n
                     }), this._cell.addClass("jp-blockly-codeCell"), this._cell.readOnly = !0, this._cell.model.trusted = !0, this._cell.model.mimeType = this._manager.mimeType, this._cell.node.style.overflow = "scroll", this._manager.changed.connect(this._onManagerChanged, this)
                 }
+                get cell() {
+                    return this._cell
+                }
                 get workspace() {
                     return d.serialization.workspaces.save(this._workspace)
                 }
                 set workspace(e) {
                     const t = null === e ? {
                         variables: []
                     } : e;
@@ -437,15 +440,21 @@
                     this.content.dispose(), super.dispose()
                 }
             }
             class v extends a.SplitPanel {
                 constructor(e, t, n) {
                     super({
                         layout: new b(t, e.sessionContext, n)
-                    }), this.addClass("jp-BlocklyPanel"), this._context = e, this._context.ready.then((() => this._load())), this._context.saveState.connect(this._onSave, this)
+                    }), this.addClass("jp-BlocklyPanel"), this._context = e, this._rendermime = n, this._context.ready.then((() => this._load())), this._context.saveState.connect(this._onSave, this)
+                }
+                get cell() {
+                    return this.layout.cell
+                }
+                get rendermime() {
+                    return this._rendermime
                 }
                 dispose() {
                     this.isDisposed || (s.Signal.clearData(this), super.dispose())
                 }
                 _load() {
                     const e = this._context.model.toJSON();
                     this.layout.workspace = e
@@ -655,21 +664,22 @@
                 constructor(e) {
                     super(e), this._registry = new T, this._rendermime = e.rendermime, this._mimetypeService = e.mimetypeService
                 }
                 get registry() {
                     return this._registry
                 }
                 createNewWidget(e) {
+                    e.model.metadata = new Map;
                     const t = new K(this._registry, e.sessionContext, this._mimetypeService),
                         n = new v(e, t, this._rendermime);
                     return new x({
                         context: e,
                         content: n,
                         manager: t
                     })
                 }
             }
             const M = new(n(1526).Token)("jupyterlab-blockly/registry")
         }
     }
 ]);
-//# sourceMappingURL=835.cbd12870eccd44d69cf0.js.map?v=cbd12870eccd44d69cf0
+//# sourceMappingURL=835.6f7e7b701fee67a1ec53.js.map?v=6f7e7b701fee67a1ec53
```

### Comparing `jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/835.cbd12870eccd44d69cf0.js.map` & `jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/835.6f7e7b701fee67a1ec53.js.map`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8231456043956044%*

 * *Differences: {"'file'": "'835.6f7e7b701fee67a1ec53.js?v=6f7e7b701fee67a1ec53'",*

 * * "'mappings'": "'gaAEO,MAAMA,EAAU,CACnBC,KAAM,kBACNC,SAAU,CACN,CACID,KAAM,WACNE,KAAM,QACNC,OAAQ,MACRF,SAAU,CACN,CACID,KAAM,QACNI,KAAM,eAEV,CACIJ,KAAM,QACNI,KAAM,iBAEV,CACIJ,KAAM,QACNK,SAAU,yCACVD,KAAM,mBAEV,CACIJ,KAAM,QACNK,SAAU,sCACVD,KAAM,gBAEV,CACIJ,KAAM,QACNK,SAAU,uCACVD,KAAM,iBAEV,CACIJ,KAAM,QACNK,SAAU,oCACVD,KAAM,cAEV,CACIJ,KAAM,QACNK,SAAU,uCACVD,KAAM,mBAIlB,CACIJ,KAAM,WACNE,KAAM,QACNC,OAAQ,MACRF,SAAU,CACN,CACID,KAAM,QACNK,SAAU,uNACVD, […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "835.cbd12870eccd44d69cf0.js?v=cbd12870eccd44d69cf0",
-    "mappings": "iaAEO,MAAMA,EAAU,CACnBC,KAAM,kBACNC,SAAU,CACN,CACID,KAAM,WACNE,KAAM,QACNC,OAAQ,MACRF,SAAU,CACN,CACID,KAAM,QACNI,KAAM,eAEV,CACIJ,KAAM,QACNI,KAAM,iBAEV,CACIJ,KAAM,QACNK,SAAU,yCACVD,KAAM,mBAEV,CACIJ,KAAM,QACNK,SAAU,sCACVD,KAAM,gBAEV,CACIJ,KAAM,QACNK,SAAU,uCACVD,KAAM,iBAEV,CACIJ,KAAM,QACNK,SAAU,oCACVD,KAAM,cAEV,CACIJ,KAAM,QACNK,SAAU,uCACVD,KAAM,mBAIlB,CACIJ,KAAM,WACNE,KAAM,QACNC,OAAQ,MACRF,SAAU,CACN,CACID,KAAM,QACNK,SAAU,uNACVD,KAAM,uBAEV,CACIJ,KAAM,QACNK,SAAU,6CACVD,KAAM,uBAEV,CACIJ,KAAM,QACNK,SAAU,ugBACVD,KAAM,gBAEV,CACIJ,KAAM,QACNK,SAAU,0CACVD,KAAM,oBAEV,CACIJ,KAAM,QACNK,SAAU,kDACVD,KAAM,8BAIlB,CACIJ,KAAM,WACNE,KAAM,OACNC,OAAQ,MACRF,SAAU,CACN,CACID,KAAM,QACNK,SAAU,qCACVD,KAAM,eAEV,CACIJ,KAAM,QACNK,SAAU,yWACVD,KAAM,mBAEV,CACIJ,KAAM,QACNK,SAAU,4MACVD,KAAM,eAEV,CACIJ,KAAM,QACNK,SAAU,2MACVD,KAAM,aAEV,CACIJ,KAAM,QACNK,SAAU,uCACVD,KAAM,iBAEV,CACIJ,KAAM,QACNK,SAAU,iOACVD,KAAM,wBAEV,CACIJ,KAAM,QACNK,SAAU,8MACVD,KAAM,eAEV,CACIJ,KAAM,QACNK,SAAU,6MACVD,KAAM,cAEV,CACIJ,KAAM,QACNK,SAAU,sCACVD,KAAM,gBAEV,CACIJ,KAAM,QACNK,SAAU,oXACVD,KAAM,eAEV,CACIJ,KAAM,QACNK,SAAU,+gBACVD,KAAM,kBAEV,CACIJ,KAAM,QACNK,SAAU,+WACVD,KAAM,mBAEV,CACIJ,KAAM,QACNK,SAAU,2CACVD,KAAM,uBAIlB,CACIJ,KAAM,WACNE,KAAM,OACNC,OAAQ,MACRF,SAAU,CACN,CACID,KAAM,QACNK,SAAU,8BACVD,KAAM,QAEV,CACIJ,KAAM,QACNK,SAAU,mCACVD,KAAM,aAEV,CACIJ,KAAM,QACNK,SAAU,6IACVD,KAAM,eAEV,CACIJ,KAAM,QACNK,SAAU,0MACVD,KAAM,eAEV,CACIJ,KAAM,QACNK,SAAU,wMACVD,KAAM,gBAEV,CACIJ,KAAM,QACNK,SAAU,4WACVD,KAAM,gBAEV,CACIJ,KAAM,QACNK,SAAU,iNACVD,KAAM,eAEV,CACIJ,KAAM,QACNK,SAAU,wNACVD,KAAM,qBAEV,CACIJ,KAAM,QACNK,SAAU,6MACVD,KAAM,mBAEV,CACIJ,KAAM,QACNK,SAAU,uMACVD,KAAM,aAEV,CACIJ,KAAM,QACNK,SAAU,wMACVD,KAAM,cAEV,CACIJ,KAAM,QACNK,SAAU,6MACVD,KAAM,qBAIlB,CACIJ,KAAM,WACNE,KAAM,QACNC,OAAQ,MACRF,SAAU,CACN,CACID,KAAM,QACNK,SAAU,gGACVD,KAAM,qBAEV,CACIJ,KAAM,QACNK,SAAU,2CACVD,KAAM,qBAEV,CACIJ,KAAM,QACNK,SAAU,6MACVD,KAAM,gBAEV,CACIJ,KAAM,QACNK,SAAU,sCACVD,KAAM,gBAEV,CACIJ,KAAM,QACNK,SAAU,uCACVD,KAAM,iBAEV,CACIJ,KAAM,QACNK,SAAU,mNACVD,KAAM,iBAEV,CACIJ,KAAM,QACNK,SAAU,oNACVD,KAAM,kBAEV,CACIJ,KAAM,QACNK,SAAU,mNACVD,KAAM,kBAEV,CACIJ,KAAM,QACNK,SAAU,qNACVD,KAAM,oBAEV,CACIJ,KAAM,QACNK,SAAU,wMACVD,KAAM,eAEV,CACIJ,KAAM,QACNK,SAAU,oCACVD,KAAM,gBAIlB,CACIJ,KAAM,WACNE,KAAM,QACNC,OAAQ,KACRF,SAAU,CACN,CACID,KAAM,QACNK,SAAU,uCACVD,KAAM,iBAEV,CACIJ,KAAM,QACNK,SAAU,uCACVD,KAAM,iBAEV,CACIJ,KAAM,QACNK,SAAU,2gBACVD,KAAM,cAEV,CACIJ,KAAM,QACNK,SAAU,yiBACVD,KAAM,kBAIlB,CACIJ,KAAM,OAEV,CACIA,KAAM,WACNG,OAAQ,MACRG,OAAQ,WACRJ,KAAM,aAEV,CACIF,KAAM,WACNG,OAAQ,MACRG,OAAQ,YACRJ,KAAM,eAwBLK,EAnBY,oBAA0B,aAAc,CAC7DL,KAAM,qBACNM,KAAM,iBACNC,gBAAiB,CACbC,0BAA2B,0BAC3BC,wBAAyB,0BACzBC,wBAAyB,2BACzBC,uBAAwB,0BACxBC,uBAAwB,0BACxBC,cAAe,EACfC,gBAAiB,0BACjBC,uBAAwB,GACxBC,iBAAkB,GAClBC,aAAc,wCAElBC,UAAW,CACPC,OAAQ,8BCzUT,MAAMC,UAAsB,EAAAC,YAK/BC,YAAYC,EAASC,EAAgBC,GACjCC,MAAM,CAAEC,SAAU,EAAAC,WAAA,gBAA4BC,YAAa,aAC3DC,KAAKC,SAAWR,EAChBO,KAAKE,gBAAkBR,EAGvBM,KAAKG,MAAQ,IAAI,EAAAC,OAGjBJ,KAAKK,MAAQ,IAAI,EAAAC,SAAS,CACtBC,MAAO,IAAI,EAAAC,cAAc,CAAC,GAC1Bb,eAGJK,KAAKK,MAAMI,SAAS,uBACpBT,KAAKK,MAAMK,UAAW,EACtBV,KAAKK,MAAME,MAAMI,SAAU,EAC3BX,KAAKK,MAAME,MAAMK,SAAWZ,KAAKC,SAASW,SAG1CZ,KAAKK,MAAMQ,KAAKC,MAAMC,SAAW,SACjCf,KAAKC,SAASe,QAAQC,QAAQjB,KAAKkB,kBAAmBlB,KAC1D,CACImB,gBAGA,OAAO,gCAAsCnB,KAAKoB,WACtD,CACID,cAAUA,GACV,MAAME,EAAqB,OAAdF,EAAqB,CAAEG,UAAW,IAAOH,EAGtD,gCAAsCE,EAAMrB,KAAKoB,WACrD,CAIAG,UACIvB,KAAKC,SAASe,QAAQQ,WAAWxB,KAAKyB,iBAAkBzB,MACxD,EAAA0B,OAAA,UAAiB1B,MACjBA,KAAKoB,WAAWG,UAChB3B,MAAM2B,SACV,CAIAI,OACI/B,MAAM+B,OAEN3B,KAAK4B,UAAU5B,KAAKG,OACpBH,KAAK4B,UAAU5B,KAAKK,MACxB,CAIAwB,OACI,OAAO,IAAI,EAAAC,cAAc,GAC7B,CAMAC,aAAaC,GAEb,CASAC,wBAGI,IAAIC,EAAoB,GAExB,MACMC,EAAcnC,KAAKoB,WAAWgB,cADpB,GAIhB,IAAK,MAAMC,KAASF,EAAa,CAC7B,MAAMG,EAAgBH,EAAYE,GAAOjE,KACrC,SAAekE,GAAeC,gBAI9BL,GADe,SAAeI,GAAeC,cAGrD,CAEA,OAAOL,CACX,CACAM,MAEI,MAEMC,EAFazC,KAAKiC,wBAEEjC,KAAKC,SAASyC,UAAUC,gBAAgB3C,KAAKoB,YACvEpB,KAAKK,MAAME,MAAMqC,YAAYC,UAAUJ,GAGnCzC,KAAKE,gBAAgB4C,aAErB,IAAAC,kBAAiB,wBAAyB,uMAK1C,EAAAzC,SAAA,QAAiBN,KAAKK,MAAOL,KAAKE,iBAC7B8C,MAAK,IAAMhD,KAAKyB,qBAChBwB,OAAMC,GAAKC,QAAQC,MAAMF,IAEtC,CAIAG,gBAAgBC,GACZ1D,MAAMyD,gBAAgBC,GACtBtD,KAAKyB,kBACT,CAIA8B,SAASD,GACL1D,MAAM2D,SAASD,GACftD,KAAKyB,kBACT,CAIA+B,aAAaF,GACT1D,MAAM4D,aAAaF,GACnBtD,KAAKyB,kBACT,CAIAgC,cAAcH,GACV1D,MAAM6D,cAAcH,GAEpBtD,KAAKoB,WAAa,SAAepB,KAAKG,MAAMU,KAAM,CAC9C6C,QAAS1D,KAAKC,SAASyD,QACvBC,MAAOpF,IAEXyB,KAAKoB,WAAWwC,mBAAkB,KAE9B,MAEMnB,EAFazC,KAAKiC,wBAEEjC,KAAKC,SAASyC,UAAUC,gBAAgB3C,KAAKoB,YACvEpB,KAAKK,MAAME,MAAMqC,YAAYC,UAAUJ,EAAK,GAEpD,CACAhB,mBAEI,YAAkBzB,KAAKoB,WAC3B,CACAF,kBAAkB2C,EAAQC,GACtB,GAAe,WAAXA,EAAqB,CAErB,MAEMrB,EAFazC,KAAKiC,wBAEEjC,KAAKC,SAASyC,UAAUC,gBAAgB3C,KAAKoB,YACvEpB,KAAKK,MAAME,MAAMqC,YAAYC,UAAUJ,GACvCzC,KAAKK,MAAME,MAAMK,SAAWZ,KAAKC,SAASW,QAC9C,CACe,YAAXkD,GACA9D,KAAKoB,WAAW2C,cAAc/D,KAAKC,SAASyD,QAEpD,ECvLG,MAAMM,UAAsB,EAAAC,cAC/BzE,YAAY0E,GACRtE,MAAMsE,GACNlE,KAAKS,SAAS,oBAClB,EAEG,MAAM0D,UAAe,EAAA/D,OACxBZ,cACII,QACAI,KAAKS,SAAS,oBAClB,E,uBCTG,MAAM2D,UAAsBJ,EAC/BxE,YAAY0E,GACRtE,MAAMsE,GACNlE,KAAKqE,aAAgBC,IACjBtE,KAAKC,SAASsE,WAAWD,EAAME,OAAOC,OACtCzE,KAAK0E,QAAQ,EAEjB1E,KAAKC,SAAWiE,EAAMzE,QACtBO,KAAKC,SAASe,QAAQC,QAAQjB,KAAK0E,OAAQ1E,KAC/C,CACAuB,UACI3B,MAAM2B,UACNvB,KAAKC,SAASe,QAAQQ,WAAWxB,KAAK0E,OAAQ1E,KAClD,CACA2E,SACI,OAAQ,kBAAoB,EAAAC,WAAY,CAAEC,SAAU7E,KAAKqE,aAAcI,MAAOzE,KAAKC,SAAS6E,aAAcC,QAAS/E,KAAKC,SAAS+E,iBACrI,EChBG,MAAMC,UAAwBjB,EACjCxE,YAAY0E,GACRtE,MAAMsE,GACNlE,KAAKqE,aAAgBC,IACjBtE,KAAKC,SAASiF,aAAaZ,EAAME,OAAOC,OACxCzE,KAAK0E,QAAQ,EAEjB1E,KAAKC,SAAWiE,EAAMzE,QACtBO,KAAKC,SAASe,QAAQC,QAAQjB,KAAK0E,OAAQ1E,KAC/C,CACAuB,UACI3B,MAAM2B,UACNvB,KAAKC,SAASe,QAAQQ,WAAWxB,KAAK0E,OAAQ1E,KAClD,CACA2E,SACI,MAAMQ,EAAUnF,KAAKC,SAASmF,cAI9B,MAH6B,cAAzBpF,KAAKC,SAASoF,QACdF,EAAQG,KAAK,CAAEC,MAAO,YAAad,MAAO,cAEtC,kBAAoB,EAAAG,WAAY,CAAEC,SAAU7E,KAAKqE,aAAcI,MAAOzE,KAAKC,SAASoF,OAAQN,QAASI,GACjH,ECdG,MAAMK,UAAsB,EAAAC,eAC/BjG,YAAYuF,GACRnF,MAAMmF,GAKN,MAAMW,EAAS,IAAI1B,EAAc,CAC7BuB,MAAO,GACPI,KAAM,EAAAC,QACNC,UAAW,uBACXC,QAAS,IAAM9F,KAAK+F,QAAQC,OAAOxD,MACnCyD,QAAS,aAEbjG,KAAKkG,QAAQC,QAAQ,MAAOT,GAC5B1F,KAAKkG,QAAQC,QAAQ,SAAU,IAAIhC,GACnCnE,KAAKkG,QAAQC,QAAQ,UAAW,IAAI/B,EAAc,CAC9CmB,MAAO,UACPU,QAAS,iBACTxG,QAASsF,EAAQtF,WAErBO,KAAKkG,QAAQC,QAAQ,YAAa,IAAIlB,EAAgB,CAClDM,MAAO,SACPU,QAAS,gBACTxG,QAASsF,EAAQtF,UAEzB,CAIA8B,UACIvB,KAAK+F,QAAQxE,UACb3B,MAAM2B,SACV,EAKG,MAAM6E,UAAqB,EAAAtG,WAM9BN,YAAY6G,EAAS5G,EAASE,GAC1BC,MAAM,CACFoG,OAAQ,IAAI1G,EAAcG,EAAS4G,EAAQ3G,eAAgBC,KAE/DK,KAAKS,SAAS,mBACdT,KAAKsG,SAAWD,EAEhBrG,KAAKsG,SAASC,MAAMvD,MAAK,IAAMhD,KAAKwG,UAEpCxG,KAAKsG,SAASG,UAAUxF,QAAQjB,KAAK0G,QAAS1G,KAClD,CAIAuB,UACQvB,KAAK2G,aAGT,EAAAjF,OAAA,UAAiB1B,MACjBJ,MAAM2B,UACV,CACAiF,QAEI,MAAMT,EAAU/F,KAAKsG,SAAS/F,MAAMqG,SACpC5G,KAAKgG,OAAO7E,UAAY4E,CAC5B,CACAW,QAAQ7C,EAAQgD,GACZ,GAAc,YAAVA,EAAqB,CACrB,MAAM1F,EAAYnB,KAAKgG,OAAO7E,UAC9BnB,KAAKsG,SAAS/F,MAAMuG,SAAS3F,EACjC,CACJ,E,ICVA4F,E,iDA9DG,MAAMC,EAITxH,cACIQ,KAAKiH,WAAa,IAAIC,IACtBlH,KAAKiH,WAAWE,IAAI,UAAWpJ,GAC/BiC,KAAKoH,YAAc,IAAIF,IACvBlH,KAAKoH,YAAYD,IAAI,SAAUE,EAAAC,iBAC/BtH,KAAKoH,YAAYD,IAAI,aAAcI,EAAAC,qBACnCxH,KAAKoH,YAAYD,IAAI,MAAOM,EAAAC,aAChC,CAIIC,gBACA,OAAO3H,KAAKiH,UAChB,CAIIW,iBACA,OAAO5H,KAAKoH,WAChB,CAQAS,gBAAgB3J,EAAMuG,GAClBzE,KAAKiH,WAAWE,IAAIjJ,EAAMuG,EAC9B,CAMAqD,eAAeC,GACX,4BAAkCA,EACtC,CAcAC,kBAAkB9J,EAAMwE,GACpB1C,KAAKoH,YAAYD,IAAIjJ,EAAMwE,EAC/B,CACAuF,YAAYC,GACRnB,EAAQoB,qBAAqBD,EACjC,GAGJ,SAAWnB,GA6GPA,EAAQoB,qBAzGRC,eAAoCF,GAChC,IAAIG,EACJ,OAAQH,GACJ,IAAK,KACDG,EAAS,4CACT,MACJ,IAAK,KACDA,EAAS,mCACT,MACJ,IAAK,KACDA,EAAS,mCACT,MACJ,IAAK,KACDA,EAAS,mCACT,MACJ,IAAK,KACDA,EAAS,mCACT,MACJ,IAAK,KACDA,EAAS,mCACT,MACJ,IAAK,KACDA,EAAS,mCACT,MACJ,IAAK,KACDA,EAAS,mCACT,MACJ,IAAK,KACDA,EAAS,mCACT,MACJ,IAAK,KACDA,EAAS,mCACT,MACJ,IAAK,KACDA,EAAS,mCACT,MACJ,IAAK,KACDA,EAAS,kCACT,MACJ,IAAK,KACDA,EAAS,mCACT,MACJ,IAAK,KACDA,EAAS,mCACT,MACJ,IAAK,KACDA,EAAS,mCACT,MACJ,IAAK,KACDA,EAAS,mCACT,MACJ,IAAK,KACDA,EAAS,mCACT,MACJ,IAAK,KACDA,EAAS,mCACT,MACJ,IAAK,KACDA,EAAS,mCACT,MACJ,IAAK,KACDA,EAAS,mCACT,MACJ,IAAK,KACDA,EAAS,mCACT,MACJ,IAAK,KACDA,EAAS,mCACT,MACJ,IAAK,KACDA,EAAS,mCACT,MACJ,IAAK,KACDA,EAAS,mCACT,MACJ,IAAK,KACDA,EAAS,kCACT,MACJ,IAAK,KACDA,EAAS,mCACT,MACJ,IAAK,KACDA,EAAS,mCACT,MACJ,IAAK,KACDA,EAAS,mCACT,MACJ,IAAK,KACDA,EAAS,kCACT,MACJ,QAIIlF,QAAQmF,KAAK,uCACbD,EAASE,QAAQC,QAAQ,KAIjCH,EAAOrF,MAAKyF,IAGR,YAAkBA,EAAK,GAE/B,CAEH,CA9GD,CA8GG1B,IAAYA,EAAU,CAAC,ICnLnB,MAAM2B,EAITlJ,YAAYmJ,EAAUjJ,EAAgBkJ,GAClC5I,KAAK6I,UAAYF,EACjB3I,KAAKE,gBAAkBR,EACvBM,KAAK8I,iBAAmBF,EACxB5I,KAAK+I,SAAW,UAChB/I,KAAKgJ,WAAahJ,KAAK6I,UAAUjB,WAAWqB,IAAI,UAChDjJ,KAAKkJ,SAAW,IAAI,EAAAxH,OAAO1B,MAC3BA,KAAKE,gBAAgBiJ,cAAclI,QAAQjB,KAAKoJ,iBAAkBpJ,KACtE,CAII0D,cACA,OAAO1D,KAAK6I,UAAUlB,UAAUsB,IAAIjJ,KAAK+I,SAC7C,CAOInI,eACA,OAAIZ,KAAKqJ,gBACErJ,KAAK8I,iBAAiBQ,sBAAsB,CAC/CpL,KAAM8B,KAAKqJ,gBAAgBnB,WAIxB,YAEf,CAII7C,aACA,IAAIkE,EACJ,OAAwC,QAA/BA,EAAKvJ,KAAKqJ,uBAAoC,IAAPE,OAAgB,EAASA,EAAGrL,OAAS,WACzF,CAIIwE,gBACA,OAAO1C,KAAKgJ,UAChB,CAIIhI,cACA,OAAOhB,KAAKkJ,QAChB,CAIA3H,UACIvB,KAAKE,gBAAgBiJ,cAAc3H,WAAWxB,KAAKoJ,iBAAkBpJ,KACzE,CAMA8E,aACI,OAAO9E,KAAK+I,QAChB,CAMAxE,WAAWrG,GACP,GAAI8B,KAAK+I,WAAa7K,EAAM,CACxB,MAAMwF,EAAU1D,KAAK6I,UAAUlB,UAAUsB,IAAI/K,GAC7C8B,KAAK+I,SAAWrF,EAAUxF,EAAO,UACjC8B,KAAKkJ,SAASM,KAAK,UACvB,CACJ,CAMAxE,gBACI,MAAMyE,EAAO,GAIb,OAHAzJ,KAAK6I,UAAUlB,UAAU+B,SAAQ,CAAChG,EAASxF,KACvCuL,EAAKnE,KAAK,CAAEC,MAAOrH,EAAMuG,MAAOvG,GAAO,IAEpCuL,CACX,CAMAvE,aAAahH,GACT8B,KAAKE,gBAAgByJ,aAAa,CAAEzL,QACxC,CAMAkH,cACI,MAAMwE,EAAQ5J,KAAKE,gBAAgB2J,aAAaD,MAAME,YAChDL,EAAO,GAOb,OANAM,OAAOC,KAAKJ,GAAOF,SAAQO,IACvB,MAAM/B,EAAW0B,EAAMK,GAAK/B,SACxBlI,KAAK6I,UAAUjB,WAAWsC,IAAIhC,IAC9BuB,EAAKnE,KAAK,CAAEC,MAAOqE,EAAMK,GAAKE,aAAc1F,MAAOmF,EAAMK,GAAK/L,MAClE,IAEGuL,CACX,CACAL,iBAAiBvF,EAAQuG,GACrB,MAAMR,EAAQ5J,KAAKE,gBAAgB2J,aAAaD,MAAME,YACtD,GAAIM,EAAKC,eAA0CC,IAA9BV,EAAMQ,EAAKC,SAASnM,MAAqB,CAC1D8B,KAAKqJ,gBAAkBO,EAAMQ,EAAKC,SAASnM,MAC3C,MAAMgK,EAAW0B,EAAMQ,EAAKC,SAASnM,MAAMgK,SAC3ClI,KAAKgJ,WAAahJ,KAAK6I,UAAUjB,WAAWqB,IAAIf,GAChDlI,KAAKkJ,SAASM,KAAK,SACvB,CACJ,EC3HG,MAAMe,UAA6B,EAAAC,iBAMtChL,YAAYuF,GACRnF,MAAMmF,GACN/E,KAAK6I,UAAY,IAAI7B,EACrBhH,KAAKyK,YAAc1F,EAAQpF,WAC3BK,KAAK8I,iBAAmB/D,EAAQ6D,eACpC,CACID,eACA,OAAO3I,KAAK6I,SAChB,CAOA6B,gBAAgBrE,GACZ,MAAM5G,EAAU,IAAIiJ,EAAe1I,KAAK6I,UAAWxC,EAAQ3G,eAAgBM,KAAK8I,kBAC1E/C,EAAU,IAAIK,EAAaC,EAAS5G,EAASO,KAAKyK,aACxD,OAAO,IAAIjF,EAAc,CAAEa,UAASN,UAAStG,WACjD,EC5BG,MAAMkL,EAAmB,I,QAAIC,OAAM,8B",
+    "file": "835.6f7e7b701fee67a1ec53.js?v=6f7e7b701fee67a1ec53",
+    "mappings": "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",
     "names": [
         "TOOLBOX",
         "kind",
         "contents",
         "name",
         "colour",
         "type",
@@ -50,14 +50,15 @@
         "mimeType",
         "node",
         "style",
         "overflow",
         "changed",
         "connect",
         "_onManagerChanged",
+        "cell",
         "workspace",
         "_workspace",
         "data",
         "variables",
         "dispose",
         "disconnect",
         "_resizeWorkspace",
@@ -134,14 +135,15 @@
         "layout",
         "tooltip",
         "toolbar",
         "addItem",
         "BlocklyPanel",
         "context",
         "_context",
+        "_rendermime",
         "ready",
         "_load",
         "saveState",
         "_onSave",
         "isDisposed",
         "toJSON",
         "state",
@@ -200,15 +202,14 @@
         "has",
         "display_name",
         "args",
         "newValue",
         "undefined",
         "BlocklyEditorFactory",
         "ABCWidgetFactory",
-        "_rendermime",
         "createNewWidget",
         "IBlocklyRegistry",
         "Token"
     ],
     "sourceRoot": "",
     "sources": [
         "webpack://jupyterlab-blockly-extension/../blockly/lib/utils.js",
@@ -220,19 +221,19 @@
         "webpack://jupyterlab-blockly-extension/../blockly/lib/registry.js",
         "webpack://jupyterlab-blockly-extension/../blockly/lib/manager.js",
         "webpack://jupyterlab-blockly-extension/../blockly/lib/factory.js",
         "webpack://jupyterlab-blockly-extension/../blockly/lib/token.js"
     ],
     "sourcesContent": [
         "import * as Blockly from 'blockly';\n// Creating a toolbox containing all the main (default) blocks.\nexport const TOOLBOX = {\n    kind: 'categoryToolbox',\n    contents: [\n        {\n            kind: 'category',\n            name: 'Logic',\n            colour: '210',\n            contents: [\n                {\n                    kind: 'block',\n                    type: 'controls_if'\n                },\n                {\n                    kind: 'BLOCK',\n                    type: 'logic_compare'\n                },\n                {\n                    kind: 'BLOCK',\n                    blockxml: '<block type=\"logic_operation\"></block>',\n                    type: 'logic_operation'\n                },\n                {\n                    kind: 'BLOCK',\n                    blockxml: '<block type=\"logic_negate\"></block>',\n                    type: 'logic_negate'\n                },\n                {\n                    kind: 'BLOCK',\n                    blockxml: '<block type=\"logic_boolean\"></block>',\n                    type: 'logic_boolean'\n                },\n                {\n                    kind: 'BLOCK',\n                    blockxml: '<block type=\"logic_null\"></block>',\n                    type: 'logic_null'\n                },\n                {\n                    kind: 'BLOCK',\n                    blockxml: '<block type=\"logic_ternary\"></block>',\n                    type: 'logic_ternary'\n                }\n            ]\n        },\n        {\n            kind: 'category',\n            name: 'Loops',\n            colour: '120',\n            contents: [\n                {\n                    kind: 'BLOCK',\n                    blockxml: '<block type=\"controls_repeat_ext\">\\n          <value name=\"TIMES\">\\n            <shadow type=\"math_number\">\\n              <field name=\"NUM\">10</field>\\n            </shadow>\\n          </value>\\n        </block>',\n                    type: 'controls_repeat_ext'\n                },\n                {\n                    kind: 'BLOCK',\n                    blockxml: '<block type=\"controls_whileUntil\"></block>',\n                    type: 'controls_whileUntil'\n                },\n                {\n                    kind: 'BLOCK',\n                    blockxml: '<block type=\"controls_for\">\\n          <value name=\"FROM\">\\n            <shadow type=\"math_number\">\\n              <field name=\"NUM\">1</field>\\n            </shadow>\\n          </value>\\n          <value name=\"TO\">\\n            <shadow type=\"math_number\">\\n              <field name=\"NUM\">10</field>\\n            </shadow>\\n          </value>\\n          <value name=\"BY\">\\n            <shadow type=\"math_number\">\\n              <field name=\"NUM\">1</field>\\n            </shadow>\\n          </value>\\n        </block>',\n                    type: 'controls_for'\n                },\n                {\n                    kind: 'BLOCK',\n                    blockxml: '<block type=\"controls_forEach\"></block>',\n                    type: 'controls_forEach'\n                },\n                {\n                    kind: 'BLOCK',\n                    blockxml: '<block type=\"controls_flow_statements\"></block>',\n                    type: 'controls_flow_statements'\n                }\n            ]\n        },\n        {\n            kind: 'CATEGORY',\n            name: 'Math',\n            colour: '230',\n            contents: [\n                {\n                    kind: 'BLOCK',\n                    blockxml: '<block type=\"math_number\"></block>',\n                    type: 'math_number'\n                },\n                {\n                    kind: 'BLOCK',\n                    blockxml: '<block type=\"math_arithmetic\">\\n          <value name=\"A\">\\n            <shadow type=\"math_number\">\\n              <field name=\"NUM\">1</field>\\n            </shadow>\\n          </value>\\n          <value name=\"B\">\\n            <shadow type=\"math_number\">\\n              <field name=\"NUM\">1</field>\\n            </shadow>\\n          </value>\\n        </block>',\n                    type: 'math_arithmetic'\n                },\n                {\n                    kind: 'BLOCK',\n                    blockxml: '<block type=\"math_single\">\\n          <value name=\"NUM\">\\n            <shadow type=\"math_number\">\\n              <field name=\"NUM\">9</field>\\n            </shadow>\\n          </value>\\n        </block>',\n                    type: 'math_single'\n                },\n                {\n                    kind: 'BLOCK',\n                    blockxml: '<block type=\"math_trig\">\\n          <value name=\"NUM\">\\n            <shadow type=\"math_number\">\\n              <field name=\"NUM\">45</field>\\n            </shadow>\\n          </value>\\n        </block>',\n                    type: 'math_trig'\n                },\n                {\n                    kind: 'BLOCK',\n                    blockxml: '<block type=\"math_constant\"></block>',\n                    type: 'math_constant'\n                },\n                {\n                    kind: 'BLOCK',\n                    blockxml: '<block type=\"math_number_property\">\\n          <value name=\"NUMBER_TO_CHECK\">\\n            <shadow type=\"math_number\">\\n              <field name=\"NUM\">0</field>\\n            </shadow>\\n          </value>\\n        </block>',\n                    type: 'math_number_property'\n                },\n                {\n                    kind: 'BLOCK',\n                    blockxml: '<block type=\"math_change\">\\n          <value name=\"DELTA\">\\n            <shadow type=\"math_number\">\\n              <field name=\"NUM\">1</field>\\n            </shadow>\\n          </value>\\n        </block>',\n                    type: 'math_change'\n                },\n                {\n                    kind: 'BLOCK',\n                    blockxml: '<block type=\"math_round\">\\n          <value name=\"NUM\">\\n            <shadow type=\"math_number\">\\n              <field name=\"NUM\">3.1</field>\\n            </shadow>\\n          </value>\\n        </block>',\n                    type: 'math_round'\n                },\n                {\n                    kind: 'BLOCK',\n                    blockxml: '<block type=\"math_on_list\"></block>',\n                    type: 'math_on_list'\n                },\n                {\n                    kind: 'BLOCK',\n                    blockxml: '<block type=\"math_modulo\">\\n          <value name=\"DIVIDEND\">\\n            <shadow type=\"math_number\">\\n              <field name=\"NUM\">64</field>\\n            </shadow>\\n          </value>\\n          <value name=\"DIVISOR\">\\n            <shadow type=\"math_number\">\\n              <field name=\"NUM\">10</field>\\n            </shadow>\\n          </value>\\n        </block>',\n                    type: 'math_modulo'\n                },\n                {\n                    kind: 'BLOCK',\n                    blockxml: '<block type=\"math_constrain\">\\n          <value name=\"VALUE\">\\n            <shadow type=\"math_number\">\\n              <field name=\"NUM\">50</field>\\n            </shadow>\\n          </value>\\n          <value name=\"LOW\">\\n            <shadow type=\"math_number\">\\n              <field name=\"NUM\">1</field>\\n            </shadow>\\n          </value>\\n          <value name=\"HIGH\">\\n            <shadow type=\"math_number\">\\n              <field name=\"NUM\">100</field>\\n            </shadow>\\n          </value>\\n        </block>',\n                    type: 'math_constrain'\n                },\n                {\n                    kind: 'BLOCK',\n                    blockxml: '<block type=\"math_random_int\">\\n          <value name=\"FROM\">\\n            <shadow type=\"math_number\">\\n              <field name=\"NUM\">1</field>\\n            </shadow>\\n          </value>\\n          <value name=\"TO\">\\n            <shadow type=\"math_number\">\\n              <field name=\"NUM\">100</field>\\n            </shadow>\\n          </value>\\n        </block>',\n                    type: 'math_random_int'\n                },\n                {\n                    kind: 'BLOCK',\n                    blockxml: '<block type=\"math_random_float\"></block>',\n                    type: 'math_random_float'\n                }\n            ]\n        },\n        {\n            kind: 'CATEGORY',\n            name: 'Text',\n            colour: '160',\n            contents: [\n                {\n                    kind: 'BLOCK',\n                    blockxml: '<block type=\"text\"></block>',\n                    type: 'text'\n                },\n                {\n                    kind: 'BLOCK',\n                    blockxml: '<block type=\"text_join\"></block>',\n                    type: 'text_join'\n                },\n                {\n                    kind: 'BLOCK',\n                    blockxml: '<block type=\"text_append\">\\n          <value name=\"TEXT\">\\n            <shadow type=\"text\"></shadow>\\n          </value>\\n        </block>',\n                    type: 'text_append'\n                },\n                {\n                    kind: 'BLOCK',\n                    blockxml: '<block type=\"text_length\">\\n          <value name=\"VALUE\">\\n            <shadow type=\"text\">\\n              <field name=\"TEXT\">abc</field>\\n            </shadow>\\n          </value>\\n        </block>',\n                    type: 'text_length'\n                },\n                {\n                    kind: 'BLOCK',\n                    blockxml: '<block type=\"text_isEmpty\">\\n          <value name=\"VALUE\">\\n            <shadow type=\"text\">\\n              <field name=\"TEXT\"></field>\\n            </shadow>\\n          </value>\\n        </block>',\n                    type: 'text_isEmpty'\n                },\n                {\n                    kind: 'BLOCK',\n                    blockxml: '<block type=\"text_indexOf\">\\n          <value name=\"VALUE\">\\n            <block type=\"variables_get\">\\n              <field name=\"VAR\">text</field>\\n            </block>\\n          </value>\\n          <value name=\"FIND\">\\n            <shadow type=\"text\">\\n              <field name=\"TEXT\">abc</field>\\n            </shadow>\\n          </value>\\n        </block>',\n                    type: 'text_indexOf'\n                },\n                {\n                    kind: 'BLOCK',\n                    blockxml: '<block type=\"text_charAt\">\\n          <value name=\"VALUE\">\\n            <block type=\"variables_get\">\\n              <field name=\"VAR\">text</field>\\n            </block>\\n          </value>\\n        </block>',\n                    type: 'text_charAt'\n                },\n                {\n                    kind: 'BLOCK',\n                    blockxml: '<block type=\"text_getSubstring\">\\n          <value name=\"STRING\">\\n            <block type=\"variables_get\">\\n              <field name=\"VAR\">text</field>\\n            </block>\\n          </value>\\n        </block>',\n                    type: 'text_getSubstring'\n                },\n                {\n                    kind: 'BLOCK',\n                    blockxml: '<block type=\"text_changeCase\">\\n          <value name=\"TEXT\">\\n            <shadow type=\"text\">\\n              <field name=\"TEXT\">abc</field>\\n            </shadow>\\n          </value>\\n        </block>',\n                    type: 'text_changeCase'\n                },\n                {\n                    kind: 'BLOCK',\n                    blockxml: '<block type=\"text_trim\">\\n          <value name=\"TEXT\">\\n            <shadow type=\"text\">\\n              <field name=\"TEXT\">abc</field>\\n            </shadow>\\n          </value>\\n        </block>',\n                    type: 'text_trim'\n                },\n                {\n                    kind: 'BLOCK',\n                    blockxml: '<block type=\"text_print\">\\n          <value name=\"TEXT\">\\n            <shadow type=\"text\">\\n              <field name=\"TEXT\">abc</field>\\n            </shadow>\\n          </value>\\n        </block>',\n                    type: 'text_print'\n                },\n                {\n                    kind: 'BLOCK',\n                    blockxml: '<block type=\"text_prompt_ext\">\\n          <value name=\"TEXT\">\\n            <shadow type=\"text\">\\n              <field name=\"TEXT\">abc</field>\\n            </shadow>\\n          </value>\\n        </block>',\n                    type: 'text_prompt_ext'\n                }\n            ]\n        },\n        {\n            kind: 'CATEGORY',\n            name: 'Lists',\n            colour: '260',\n            contents: [\n                {\n                    kind: 'BLOCK',\n                    blockxml: '<block type=\"lists_create_with\">\\n          <mutation items=\"0\"></mutation>\\n        </block>',\n                    type: 'lists_create_with'\n                },\n                {\n                    kind: 'BLOCK',\n                    blockxml: '<block type=\"lists_create_with\"></block>',\n                    type: 'lists_create_with'\n                },\n                {\n                    kind: 'BLOCK',\n                    blockxml: '<block type=\"lists_repeat\">\\n          <value name=\"NUM\">\\n            <shadow type=\"math_number\">\\n              <field name=\"NUM\">5</field>\\n            </shadow>\\n          </value>\\n        </block>',\n                    type: 'lists_repeat'\n                },\n                {\n                    kind: 'BLOCK',\n                    blockxml: '<block type=\"lists_length\"></block>',\n                    type: 'lists_length'\n                },\n                {\n                    kind: 'BLOCK',\n                    blockxml: '<block type=\"lists_isEmpty\"></block>',\n                    type: 'lists_isEmpty'\n                },\n                {\n                    kind: 'BLOCK',\n                    blockxml: '<block type=\"lists_indexOf\">\\n          <value name=\"VALUE\">\\n            <block type=\"variables_get\">\\n              <field name=\"VAR\">list</field>\\n            </block>\\n          </value>\\n        </block>',\n                    type: 'lists_indexOf'\n                },\n                {\n                    kind: 'BLOCK',\n                    blockxml: '<block type=\"lists_getIndex\">\\n          <value name=\"VALUE\">\\n            <block type=\"variables_get\">\\n              <field name=\"VAR\">list</field>\\n            </block>\\n          </value>\\n        </block>',\n                    type: 'lists_getIndex'\n                },\n                {\n                    kind: 'BLOCK',\n                    blockxml: '<block type=\"lists_setIndex\">\\n          <value name=\"LIST\">\\n            <block type=\"variables_get\">\\n              <field name=\"VAR\">list</field>\\n            </block>\\n          </value>\\n        </block>',\n                    type: 'lists_setIndex'\n                },\n                {\n                    kind: 'BLOCK',\n                    blockxml: '<block type=\"lists_getSublist\">\\n          <value name=\"LIST\">\\n            <block type=\"variables_get\">\\n              <field name=\"VAR\">list</field>\\n            </block>\\n          </value>\\n        </block>',\n                    type: 'lists_getSublist'\n                },\n                {\n                    kind: 'BLOCK',\n                    blockxml: '<block type=\"lists_split\">\\n          <value name=\"DELIM\">\\n            <shadow type=\"text\">\\n              <field name=\"TEXT\">,</field>\\n            </shadow>\\n          </value>\\n        </block>',\n                    type: 'lists_split'\n                },\n                {\n                    kind: 'BLOCK',\n                    blockxml: '<block type=\"lists_sort\"></block>',\n                    type: 'lists_sort'\n                }\n            ]\n        },\n        {\n            kind: 'CATEGORY',\n            name: 'Color',\n            colour: '20',\n            contents: [\n                {\n                    kind: 'BLOCK',\n                    blockxml: '<block type=\"colour_picker\"></block>',\n                    type: 'colour_picker'\n                },\n                {\n                    kind: 'BLOCK',\n                    blockxml: '<block type=\"colour_random\"></block>',\n                    type: 'colour_random'\n                },\n                {\n                    kind: 'BLOCK',\n                    blockxml: '<block type=\"colour_rgb\">\\n          <value name=\"RED\">\\n            <shadow type=\"math_number\">\\n              <field name=\"NUM\">100</field>\\n            </shadow>\\n          </value>\\n          <value name=\"GREEN\">\\n            <shadow type=\"math_number\">\\n              <field name=\"NUM\">50</field>\\n            </shadow>\\n          </value>\\n          <value name=\"BLUE\">\\n            <shadow type=\"math_number\">\\n              <field name=\"NUM\">0</field>\\n            </shadow>\\n          </value>\\n        </block>',\n                    type: 'colour_rgb'\n                },\n                {\n                    kind: 'BLOCK',\n                    blockxml: '<block type=\"colour_blend\">\\n          <value name=\"COLOUR1\">\\n            <shadow type=\"colour_picker\">\\n              <field name=\"COLOUR\">#ff0000</field>\\n            </shadow>\\n          </value>\\n          <value name=\"COLOUR2\">\\n            <shadow type=\"colour_picker\">\\n              <field name=\"COLOUR\">#3333ff</field>\\n            </shadow>\\n          </value>\\n          <value name=\"RATIO\">\\n            <shadow type=\"math_number\">\\n              <field name=\"NUM\">0.5</field>\\n            </shadow>\\n          </value>\\n        </block>',\n                    type: 'colour_blend'\n                }\n            ]\n        },\n        {\n            kind: 'SEP'\n        },\n        {\n            kind: 'CATEGORY',\n            colour: '330',\n            custom: 'VARIABLE',\n            name: 'Variables'\n        },\n        {\n            kind: 'CATEGORY',\n            colour: '290',\n            custom: 'PROCEDURE',\n            name: 'Functions'\n        }\n    ]\n};\n// Defining a Blockly Theme in accordance with the current JupyterLab Theme.\nconst jupyterlab_theme = Blockly.Theme.defineTheme('jupyterlab', {\n    name: 'JupyterLab Blockly',\n    base: Blockly.Themes.Classic,\n    componentStyles: {\n        workspaceBackgroundColour: 'var(--jp-layout-color0)',\n        toolboxBackgroundColour: 'var(--jp-layout-color2)',\n        toolboxForegroundColour: 'var(--jp-ui-font-color0)',\n        flyoutBackgroundColour: 'var(--jp-border-color2)',\n        flyoutForegroundColour: 'var(--jp-layout-color3)',\n        flyoutOpacity: 1,\n        scrollbarColour: 'var(--jp-border-color0)',\n        insertionMarkerOpacity: 0.3,\n        scrollbarOpacity: 0.4,\n        cursorColour: 'var(--jp-scrollbar-background-color)'\n    },\n    fontStyle: {\n        family: 'var(--jp-ui-font-family)'\n    }\n});\nexport const THEME = jupyterlab_theme;\n//# sourceMappingURL=utils.js.map",
-        "import { showErrorMessage } from '@jupyterlab/apputils';\nimport { CodeCell, CodeCellModel } from '@jupyterlab/cells';\nimport { SplitLayout, SplitPanel, Widget } from '@lumino/widgets';\nimport { ArrayIterator } from '@lumino/algorithm';\nimport { Signal } from '@lumino/signaling';\nimport * as Blockly from 'blockly';\nimport { THEME } from './utils';\n/**\n * A blockly layout to host the Blockly editor.\n */\nexport class BlocklyLayout extends SplitLayout {\n    /**\n     * Construct a `BlocklyLayout`.\n     *\n     */\n    constructor(manager, sessionContext, rendermime) {\n        super({ renderer: SplitPanel.defaultRenderer, orientation: 'vertical' });\n        this._manager = manager;\n        this._sessionContext = sessionContext;\n        // Creating the container for the Blockly editor\n        // and the output area to render the execution replies.\n        this._host = new Widget();\n        // Creating a CodeCell widget to render the code and\n        // outputs from the execution reply.\n        this._cell = new CodeCell({\n            model: new CodeCellModel({}),\n            rendermime\n        });\n        // Trust the outputs and set the mimeType for the code\n        this._cell.addClass('jp-blockly-codeCell');\n        this._cell.readOnly = true;\n        this._cell.model.trusted = true;\n        this._cell.model.mimeType = this._manager.mimeType;\n        // adding the style to the element as a quick fix\n        // we should make it work with the css class\n        this._cell.node.style.overflow = 'scroll';\n        this._manager.changed.connect(this._onManagerChanged, this);\n    }\n    get workspace() {\n        // eslint-disable-next-line @typescript-eslint/ban-ts-comment\n        // @ts-ignore\n        return Blockly.serialization.workspaces.save(this._workspace);\n    }\n    set workspace(workspace) {\n        const data = workspace === null ? { variables: [] } : workspace;\n        // eslint-disable-next-line @typescript-eslint/ban-ts-comment\n        // @ts-ignore\n        Blockly.serialization.workspaces.load(data, this._workspace);\n    }\n    /**\n     * Dispose of the resources held by the widget.\n     */\n    dispose() {\n        this._manager.changed.disconnect(this._resizeWorkspace, this);\n        Signal.clearData(this);\n        this._workspace.dispose();\n        super.dispose();\n    }\n    /**\n     * Init the blockly layout\n     */\n    init() {\n        super.init();\n        // Add the blockly container into the DOM\n        this.addWidget(this._host);\n        this.addWidget(this._cell);\n    }\n    /**\n     * Create an iterator over the widgets in the layout.\n     */\n    iter() {\n        return new ArrayIterator([]);\n    }\n    /**\n     * Remove a widget from the layout.\n     *\n     * @param widget - The `widget` to remove.\n     */\n    removeWidget(widget) {\n        return;\n    }\n    /**\n     * Return the extra coded (if it exists), composed of the individual\n     * data from each block in the workspace, which are defined in the\n     * toplevel_init property. (e.g. : imports needed for the block)\n     *\n     * Add extra code example:\n     * Blockly.Blocks['block_name'].toplevel_init = `import numpy`\n     */\n    getBlocksToplevelInit() {\n        // Initalize string which will return the extra code provided\n        // by the blocks, in the toplevel_init property.\n        let finalToplevelInit = '';\n        // Get all the blocks in the workspace in order.\n        const ordered = true;\n        const used_blocks = this._workspace.getAllBlocks(ordered);\n        // For each block in the workspace, check if theres is a toplevel_init,\n        // if there is, add it to the final string.\n        for (const block in used_blocks) {\n            const current_block = used_blocks[block].type;\n            if (Blockly.Blocks[current_block].toplevel_init) {\n                // console.log(Blockly.Blocks[current_block].toplevel_init);\n                // Attach it to the final string\n                const string = Blockly.Blocks[current_block].toplevel_init;\n                finalToplevelInit = finalToplevelInit + string;\n            }\n        }\n        // console.log(finalToplevelInit);\n        return finalToplevelInit;\n    }\n    run() {\n        // Get extra code from the blocks in the workspace.\n        const extra_init = this.getBlocksToplevelInit();\n        // Serializing our workspace into the chosen language generator.\n        const code = extra_init + this._manager.generator.workspaceToCode(this._workspace);\n        this._cell.model.sharedModel.setSource(code);\n        // Execute the code using the kernel, by using a static method from the\n        // same class to make an execution request.\n        if (this._sessionContext.hasNoKernel) {\n            // Check whether there is a kernel\n            showErrorMessage('Select a valid kernel', `There is not a valid kernel selected, select one from the dropdown menu in the toolbar.\n        If there isn't a valid kernel please install 'xeus-python' from Pypi.org or using mamba.\n        `);\n        }\n        else {\n            CodeCell.execute(this._cell, this._sessionContext)\n                .then(() => this._resizeWorkspace())\n                .catch(e => console.error(e));\n        }\n    }\n    /**\n     * Handle `update-request` messages sent to the widget.\n     */\n    onUpdateRequest(msg) {\n        super.onUpdateRequest(msg);\n        this._resizeWorkspace();\n    }\n    /**\n     * Handle `resize-request` messages sent to the widget.\n     */\n    onResize(msg) {\n        super.onResize(msg);\n        this._resizeWorkspace();\n    }\n    /**\n     * Handle `fit-request` messages sent to the widget.\n     */\n    onFitRequest(msg) {\n        super.onFitRequest(msg);\n        this._resizeWorkspace();\n    }\n    /**\n     * Handle `after-attach` messages sent to the widget.\n     */\n    onAfterAttach(msg) {\n        super.onAfterAttach(msg);\n        //inject Blockly with appropiate JupyterLab theme.\n        this._workspace = Blockly.inject(this._host.node, {\n            toolbox: this._manager.toolbox,\n            theme: THEME\n        });\n        this._workspace.addChangeListener(() => {\n            // Get extra code from the blocks in the workspace.\n            const extra_init = this.getBlocksToplevelInit();\n            // Serializing our workspace into the chosen language generator.\n            const code = extra_init + this._manager.generator.workspaceToCode(this._workspace);\n            this._cell.model.sharedModel.setSource(code);\n        });\n    }\n    _resizeWorkspace() {\n        //Resize logic.\n        Blockly.svgResize(this._workspace);\n    }\n    _onManagerChanged(sender, change) {\n        if (change === 'kernel') {\n            // Get extra code from the blocks in the workspace.\n            const extra_init = this.getBlocksToplevelInit();\n            // Serializing our workspace into the chosen language generator.\n            const code = extra_init + this._manager.generator.workspaceToCode(this._workspace);\n            this._cell.model.sharedModel.setSource(code);\n            this._cell.model.mimeType = this._manager.mimeType;\n        }\n        if (change === 'toolbox') {\n            this._workspace.updateToolbox(this._manager.toolbox);\n        }\n    }\n}\n//# sourceMappingURL=layout.js.map",
+        "import { showErrorMessage } from '@jupyterlab/apputils';\nimport { CodeCell, CodeCellModel } from '@jupyterlab/cells';\nimport { SplitLayout, SplitPanel, Widget } from '@lumino/widgets';\nimport { ArrayIterator } from '@lumino/algorithm';\nimport { Signal } from '@lumino/signaling';\nimport * as Blockly from 'blockly';\nimport { THEME } from './utils';\n/**\n * A blockly layout to host the Blockly editor.\n */\nexport class BlocklyLayout extends SplitLayout {\n    /**\n     * Construct a `BlocklyLayout`.\n     *\n     */\n    constructor(manager, sessionContext, rendermime) {\n        super({ renderer: SplitPanel.defaultRenderer, orientation: 'vertical' });\n        this._manager = manager;\n        this._sessionContext = sessionContext;\n        // Creating the container for the Blockly editor\n        // and the output area to render the execution replies.\n        this._host = new Widget();\n        // Creating a CodeCell widget to render the code and\n        // outputs from the execution reply.\n        this._cell = new CodeCell({\n            model: new CodeCellModel({}),\n            rendermime\n        });\n        // Trust the outputs and set the mimeType for the code\n        this._cell.addClass('jp-blockly-codeCell');\n        this._cell.readOnly = true;\n        this._cell.model.trusted = true;\n        this._cell.model.mimeType = this._manager.mimeType;\n        // adding the style to the element as a quick fix\n        // we should make it work with the css class\n        this._cell.node.style.overflow = 'scroll';\n        this._manager.changed.connect(this._onManagerChanged, this);\n    }\n    /*\n     * The code cell.\n     */\n    get cell() {\n        return this._cell;\n    }\n    /*\n     * The current workspace.\n     */\n    get workspace() {\n        // eslint-disable-next-line @typescript-eslint/ban-ts-comment\n        // @ts-ignore\n        return Blockly.serialization.workspaces.save(this._workspace);\n    }\n    /*\n     * Set a new workspace.\n     */\n    set workspace(workspace) {\n        const data = workspace === null ? { variables: [] } : workspace;\n        // eslint-disable-next-line @typescript-eslint/ban-ts-comment\n        // @ts-ignore\n        Blockly.serialization.workspaces.load(data, this._workspace);\n    }\n    /**\n     * Dispose of the resources held by the widget.\n     */\n    dispose() {\n        this._manager.changed.disconnect(this._resizeWorkspace, this);\n        Signal.clearData(this);\n        this._workspace.dispose();\n        super.dispose();\n    }\n    /**\n     * Init the blockly layout\n     */\n    init() {\n        super.init();\n        // Add the blockly container into the DOM\n        this.addWidget(this._host);\n        this.addWidget(this._cell);\n    }\n    /**\n     * Create an iterator over the widgets in the layout.\n     */\n    iter() {\n        return new ArrayIterator([]);\n    }\n    /**\n     * Remove a widget from the layout.\n     *\n     * @param widget - The `widget` to remove.\n     */\n    removeWidget(widget) {\n        return;\n    }\n    /**\n     * Return the extra coded (if it exists), composed of the individual\n     * data from each block in the workspace, which are defined in the\n     * toplevel_init property. (e.g. : imports needed for the block)\n     *\n     * Add extra code example:\n     * Blockly.Blocks['block_name'].toplevel_init = `import numpy`\n     */\n    getBlocksToplevelInit() {\n        // Initalize string which will return the extra code provided\n        // by the blocks, in the toplevel_init property.\n        let finalToplevelInit = '';\n        // Get all the blocks in the workspace in order.\n        const ordered = true;\n        const used_blocks = this._workspace.getAllBlocks(ordered);\n        // For each block in the workspace, check if theres is a toplevel_init,\n        // if there is, add it to the final string.\n        for (const block in used_blocks) {\n            const current_block = used_blocks[block].type;\n            if (Blockly.Blocks[current_block].toplevel_init) {\n                // console.log(Blockly.Blocks[current_block].toplevel_init);\n                // Attach it to the final string\n                const string = Blockly.Blocks[current_block].toplevel_init;\n                finalToplevelInit = finalToplevelInit + string;\n            }\n        }\n        // console.log(finalToplevelInit);\n        return finalToplevelInit;\n    }\n    /*\n     * Generates and runs the code from the current workspace.\n     */\n    run() {\n        // Get extra code from the blocks in the workspace.\n        const extra_init = this.getBlocksToplevelInit();\n        // Serializing our workspace into the chosen language generator.\n        const code = extra_init + this._manager.generator.workspaceToCode(this._workspace);\n        //const code = \"import ipywidgets as widgets\\nwidgets.IntSlider()\";\n        this._cell.model.sharedModel.setSource(code);\n        // Execute the code using the kernel, by using a static method from the\n        // same class to make an execution request.\n        if (this._sessionContext.hasNoKernel) {\n            // Check whether there is a kernel\n            showErrorMessage('Select a valid kernel', `There is not a valid kernel selected, select one from the dropdown menu in the toolbar.\n        If there isn't a valid kernel please install 'xeus-python' from Pypi.org or using mamba.\n        `);\n        }\n        else {\n            CodeCell.execute(this._cell, this._sessionContext)\n                .then(() => this._resizeWorkspace())\n                .catch(e => console.error(e));\n        }\n    }\n    /**\n     * Handle `update-request` messages sent to the widget.\n     */\n    onUpdateRequest(msg) {\n        super.onUpdateRequest(msg);\n        this._resizeWorkspace();\n    }\n    /**\n     * Handle `resize-request` messages sent to the widget.\n     */\n    onResize(msg) {\n        super.onResize(msg);\n        this._resizeWorkspace();\n    }\n    /**\n     * Handle `fit-request` messages sent to the widget.\n     */\n    onFitRequest(msg) {\n        super.onFitRequest(msg);\n        this._resizeWorkspace();\n    }\n    /**\n     * Handle `after-attach` messages sent to the widget.\n     */\n    onAfterAttach(msg) {\n        super.onAfterAttach(msg);\n        //inject Blockly with appropiate JupyterLab theme.\n        this._workspace = Blockly.inject(this._host.node, {\n            toolbox: this._manager.toolbox,\n            theme: THEME\n        });\n        this._workspace.addChangeListener(() => {\n            // Get extra code from the blocks in the workspace.\n            const extra_init = this.getBlocksToplevelInit();\n            // Serializing our workspace into the chosen language generator.\n            const code = extra_init + this._manager.generator.workspaceToCode(this._workspace);\n            this._cell.model.sharedModel.setSource(code);\n        });\n    }\n    _resizeWorkspace() {\n        //Resize logic.\n        Blockly.svgResize(this._workspace);\n    }\n    _onManagerChanged(sender, change) {\n        if (change === 'kernel') {\n            // Get extra code from the blocks in the workspace.\n            const extra_init = this.getBlocksToplevelInit();\n            // Serializing our workspace into the chosen language generator.\n            const code = extra_init + this._manager.generator.workspaceToCode(this._workspace);\n            this._cell.model.sharedModel.setSource(code);\n            this._cell.model.mimeType = this._manager.mimeType;\n        }\n        if (change === 'toolbox') {\n            this._workspace.updateToolbox(this._manager.toolbox);\n        }\n    }\n}\n//# sourceMappingURL=layout.js.map",
         "import { ToolbarButton } from '@jupyterlab/apputils';\nimport { Widget } from '@lumino/widgets';\nexport class BlocklyButton extends ToolbarButton {\n    constructor(props) {\n        super(props);\n        this.addClass('jp-blockly-button');\n    }\n}\nexport class Spacer extends Widget {\n    constructor() {\n        super();\n        this.addClass('jp-Toolbar-spacer');\n    }\n}\n//# sourceMappingURL=utils.js.map",
         "import { HTMLSelect } from '@jupyterlab/ui-components';\nimport React from 'react';\nimport { BlocklyButton } from './utils';\nexport class SelectToolbox extends BlocklyButton {\n    constructor(props) {\n        super(props);\n        this.handleChange = (event) => {\n            this._manager.setToolbox(event.target.value);\n            this.update();\n        };\n        this._manager = props.manager;\n        this._manager.changed.connect(this.update, this);\n    }\n    dispose() {\n        super.dispose();\n        this._manager.changed.disconnect(this.update, this);\n    }\n    render() {\n        return (React.createElement(HTMLSelect, { onChange: this.handleChange, value: this._manager.getToolbox(), options: this._manager.listToolboxes() }));\n    }\n}\n//# sourceMappingURL=toolbox.js.map",
         "import { HTMLSelect } from '@jupyterlab/ui-components';\nimport React from 'react';\nimport { BlocklyButton } from './utils';\nexport class SelectGenerator extends BlocklyButton {\n    constructor(props) {\n        super(props);\n        this.handleChange = (event) => {\n            this._manager.selectKernel(event.target.value);\n            this.update();\n        };\n        this._manager = props.manager;\n        this._manager.changed.connect(this.update, this);\n    }\n    dispose() {\n        super.dispose();\n        this._manager.changed.disconnect(this.update, this);\n    }\n    render() {\n        const kernels = this._manager.listKernels();\n        if (this._manager.kernel === 'No kernel') {\n            kernels.push({ label: 'No kernel', value: 'No kernel' });\n        }\n        return (React.createElement(HTMLSelect, { onChange: this.handleChange, value: this._manager.kernel, options: kernels }));\n    }\n}\n//# sourceMappingURL=generator.js.map",
-        "import { DocumentWidget } from '@jupyterlab/docregistry';\nimport { runIcon } from '@jupyterlab/ui-components';\nimport { SplitPanel } from '@lumino/widgets';\nimport { Signal } from '@lumino/signaling';\nimport { BlocklyLayout } from './layout';\nimport { BlocklyButton, SelectGenerator, SelectToolbox, Spacer } from './toolbar';\n/**\n * DocumentWidget: widget that represents the view or editor for a file type.\n */\nexport class BlocklyEditor extends DocumentWidget {\n    constructor(options) {\n        super(options);\n        // Loading the ITranslator\n        // const trans = this.translator.load('jupyterlab');\n        // Create and add a button to the toolbar to execute\n        // the code.\n        const button = new BlocklyButton({\n            label: '',\n            icon: runIcon,\n            className: 'jp-blockly-runButton',\n            onClick: () => this.content.layout.run(),\n            tooltip: 'Run Code'\n        });\n        this.toolbar.addItem('run', button);\n        this.toolbar.addItem('spacer', new Spacer());\n        this.toolbar.addItem('toolbox', new SelectToolbox({\n            label: 'Toolbox',\n            tooltip: 'Select tollbox',\n            manager: options.manager\n        }));\n        this.toolbar.addItem('generator', new SelectGenerator({\n            label: 'Kernel',\n            tooltip: 'Select kernel',\n            manager: options.manager\n        }));\n    }\n    /**\n     * Dispose of the resources held by the widget.\n     */\n    dispose() {\n        this.content.dispose();\n        super.dispose();\n    }\n}\n/**\n * Widget that contains the main view of the DocumentWidget.\n */\nexport class BlocklyPanel extends SplitPanel {\n    /**\n     * Construct a `BlocklyPanel`.\n     *\n     * @param context - The documents context.\n     */\n    constructor(context, manager, rendermime) {\n        super({\n            layout: new BlocklyLayout(manager, context.sessionContext, rendermime)\n        });\n        this.addClass('jp-BlocklyPanel');\n        this._context = context;\n        // Load the content of the file when the context is ready\n        this._context.ready.then(() => this._load());\n        // Connect to the save signal\n        this._context.saveState.connect(this._onSave, this);\n    }\n    /**\n     * Dispose of the resources held by the widget.\n     */\n    dispose() {\n        if (this.isDisposed) {\n            return;\n        }\n        Signal.clearData(this);\n        super.dispose();\n    }\n    _load() {\n        // Loading the content of the document into the workspace\n        const content = this._context.model.toJSON();\n        this.layout.workspace = content;\n    }\n    _onSave(sender, state) {\n        if (state === 'started') {\n            const workspace = this.layout.workspace;\n            this._context.model.fromJSON(workspace);\n        }\n    }\n}\n//# sourceMappingURL=widget.js.map",
+        "import { DocumentWidget } from '@jupyterlab/docregistry';\nimport { runIcon } from '@jupyterlab/ui-components';\nimport { SplitPanel } from '@lumino/widgets';\nimport { Signal } from '@lumino/signaling';\nimport { BlocklyLayout } from './layout';\nimport { BlocklyButton, SelectGenerator, SelectToolbox, Spacer } from './toolbar';\n/**\n * DocumentWidget: widget that represents the view or editor for a file type.\n */\nexport class BlocklyEditor extends DocumentWidget {\n    constructor(options) {\n        super(options);\n        // Loading the ITranslator\n        // const trans = this.translator.load('jupyterlab');\n        // Create and add a button to the toolbar to execute\n        // the code.\n        const button = new BlocklyButton({\n            label: '',\n            icon: runIcon,\n            className: 'jp-blockly-runButton',\n            onClick: () => this.content.layout.run(),\n            tooltip: 'Run Code'\n        });\n        this.toolbar.addItem('run', button);\n        this.toolbar.addItem('spacer', new Spacer());\n        this.toolbar.addItem('toolbox', new SelectToolbox({\n            label: 'Toolbox',\n            tooltip: 'Select tollbox',\n            manager: options.manager\n        }));\n        this.toolbar.addItem('generator', new SelectGenerator({\n            label: 'Kernel',\n            tooltip: 'Select kernel',\n            manager: options.manager\n        }));\n    }\n    /**\n     * Dispose of the resources held by the widget.\n     */\n    dispose() {\n        this.content.dispose();\n        super.dispose();\n    }\n}\n/**\n * Widget that contains the main view of the DocumentWidget.\n */\nexport class BlocklyPanel extends SplitPanel {\n    /**\n     * Construct a `BlocklyPanel`.\n     *\n     * @param context - The documents context.\n     */\n    constructor(context, manager, rendermime) {\n        super({\n            layout: new BlocklyLayout(manager, context.sessionContext, rendermime)\n        });\n        this.addClass('jp-BlocklyPanel');\n        this._context = context;\n        this._rendermime = rendermime;\n        // Load the content of the file when the context is ready\n        this._context.ready.then(() => this._load());\n        // Connect to the save signal\n        this._context.saveState.connect(this._onSave, this);\n    }\n    /*\n     * The code cell.\n     */\n    get cell() {\n        return this.layout.cell;\n    }\n    /*\n     * The rendermime instance used in the code cell.\n     */\n    get rendermime() {\n        return this._rendermime;\n    }\n    /**\n     * Dispose of the resources held by the widget.\n     */\n    dispose() {\n        if (this.isDisposed) {\n            return;\n        }\n        Signal.clearData(this);\n        super.dispose();\n    }\n    _load() {\n        // Loading the content of the document into the workspace\n        const content = this._context.model.toJSON();\n        this.layout.workspace = content;\n    }\n    _onSave(sender, state) {\n        if (state === 'started') {\n            const workspace = this.layout.workspace;\n            this._context.model.fromJSON(workspace);\n        }\n    }\n}\n//# sourceMappingURL=widget.js.map",
         "import * as Blockly from 'blockly';\nimport { pythonGenerator } from 'blockly/python';\nimport { javascriptGenerator } from 'blockly/javascript';\nimport { luaGenerator } from 'blockly/lua';\nimport En from 'blockly/msg/en';\nimport { TOOLBOX } from './utils';\n/**\n * BlocklyRegistry is the class that JupyterLab-Blockly exposes\n * to other plugins. This registry allows other plugins to register\n * new Toolboxes, Blocks and Generators that users can use in the\n * Blockly editor.\n */\nexport class BlocklyRegistry {\n    /**\n     * Constructor of BlocklyRegistry.\n     */\n    constructor() {\n        this._toolboxes = new Map();\n        this._toolboxes.set('default', TOOLBOX);\n        this._generators = new Map();\n        this._generators.set('python', pythonGenerator);\n        this._generators.set('javascript', javascriptGenerator);\n        this._generators.set('lua', luaGenerator);\n    }\n    /**\n     * Returns a map with all the toolboxes.\n     */\n    get toolboxes() {\n        return this._toolboxes;\n    }\n    /**\n     * Returns a map with all the generators.\n     */\n    get generators() {\n        return this._generators;\n    }\n    /**\n     * Register a toolbox for the editor.\n     *\n     * @argument name Name of the toolbox.\n     *\n     * @argument value Toolbox to register.\n     */\n    registerToolbox(name, value) {\n        this._toolboxes.set(name, value);\n    }\n    /**\n     * Register new blocks.\n     *\n     * @argument blocks Blocks to register.\n     */\n    registerBlocks(blocks) {\n        Blockly.defineBlocksWithJsonArray(blocks);\n    }\n    /**\n     * Register new generators.\n     *\n     * @argument name Name of the generator.\n     *\n     * @argument generator Generator to register.\n     *\n     * #### Notes\n     * When registering a generator, the name should correspond to the language\n     * used by a kernel.\n     *\n     * If you register a generator for an existing language this will be overwritten.\n     */\n    registerGenerator(name, generator) {\n        this._generators.set(name, generator);\n    }\n    setlanguage(language) {\n        Private.importLanguageModule(language);\n    }\n}\nvar Private;\n(function (Private) {\n    // Dynamically importing the language modules needed for each respective\n    // user, in order to change the Blockly language in accordance to the\n    // JL one.\n    async function importLanguageModule(language) {\n        let module;\n        switch (language) {\n            case 'En':\n                module = import('blockly/msg/en');\n                break;\n            case 'Es':\n                module = import('blockly/msg/es');\n                break;\n            case 'Fr':\n                module = import('blockly/msg/fr');\n                break;\n            case 'Sa' || 'Ar':\n                module = import('blockly/msg/ar');\n                break;\n            case 'Cz':\n                module = import('blockly/msg/cs');\n                break;\n            case 'Dk':\n                module = import('blockly/msg/da');\n                break;\n            case 'De':\n                module = import('blockly/msg/de');\n                break;\n            case 'Gr':\n                module = import('blockly/msg/el');\n                break;\n            case 'Ee':\n                module = import('blockly/msg/et');\n                break;\n            case 'Fi':\n                module = import('blockly/msg/fi');\n                break;\n            case 'Il':\n                module = import('blockly/msg/he');\n                break;\n            case 'Hu':\n                module = import('blockly/msg/hu');\n                break;\n            case 'Am':\n                module = import('blockly/msg/hy');\n                break;\n            case 'Id':\n                module = import('blockly/msg/id');\n                break;\n            case 'It':\n                module = import('blockly/msg/it');\n                break;\n            case 'Jp':\n                module = import('blockly/msg/ja');\n                break;\n            case 'Kr':\n                module = import('blockly/msg/ko');\n                break;\n            case 'Lt':\n                module = import('blockly/msg/lt');\n                break;\n            case 'Nl':\n                module = import('blockly/msg/nl');\n                break;\n            case 'Pl':\n                module = import('blockly/msg/pl');\n                break;\n            case 'Br':\n                module = import('blockly/msg/pt');\n                break;\n            case 'Ro':\n                module = import('blockly/msg/ro');\n                break;\n            case 'Ru':\n                module = import('blockly/msg/ru');\n                break;\n            case 'Lk':\n                module = import('blockly/msg/si');\n                break;\n            case 'Tr':\n                module = import('blockly/msg/tr');\n                break;\n            case 'Ua':\n                module = import('blockly/msg/uk');\n                break;\n            case 'Vn':\n                module = import('blockly/msg/vi');\n                break;\n            case 'Tw':\n                module = import('blockly/msg/zh-hant');\n                break;\n            case 'Cn':\n                module = import('blockly/msg/zh-hans');\n                break;\n            default:\n                // Complete with all the cases taken from: (last updates June 2022)\n                // List of languages in blockly: https://github.com/google/blockly/tree/master/msg/js\n                // List of languages in Lab: https://github.com/jupyterlab/language-packs/tree/master/language-packs\n                console.warn('Language not found. Loading english');\n                module = Promise.resolve(En);\n                break;\n        }\n        // Setting the current language in Blockly.\n        module.then(lang => {\n            // eslint-disable-next-line @typescript-eslint/ban-ts-comment\n            // @ts-ignore\n            Blockly.setLocale(lang);\n        });\n    }\n    Private.importLanguageModule = importLanguageModule;\n})(Private || (Private = {}));\n//# sourceMappingURL=registry.js.map",
         "import { Signal } from '@lumino/signaling';\n/**\n * BlocklyManager the manager for each document\n * to select the toolbox and the generator that the\n * user wants to use on a specific document.\n */\nexport class BlocklyManager {\n    /**\n     * Constructor of BlocklyManager.\n     */\n    constructor(registry, sessionContext, mimetypeService) {\n        this._registry = registry;\n        this._sessionContext = sessionContext;\n        this._mimetypeService = mimetypeService;\n        this._toolbox = 'default';\n        this._generator = this._registry.generators.get('python');\n        this._changed = new Signal(this);\n        this._sessionContext.kernelChanged.connect(this._onKernelChanged, this);\n    }\n    /**\n     * Returns the selected toolbox.\n     */\n    get toolbox() {\n        return this._registry.toolboxes.get(this._toolbox);\n    }\n    /**\n     * Returns the mimeType for the selected kernel.\n     *\n     * Note: We need the mimeType for the syntax highlighting\n     * when rendering the code.\n     */\n    get mimeType() {\n        if (this._selectedKernel) {\n            return this._mimetypeService.getMimeTypeByLanguage({\n                name: this._selectedKernel.language\n            });\n        }\n        else {\n            return 'text/plain';\n        }\n    }\n    /**\n     * Returns the name of the selected kernel.\n     */\n    get kernel() {\n        var _a;\n        return ((_a = this._selectedKernel) === null || _a === void 0 ? void 0 : _a.name) || 'No kernel';\n    }\n    /**\n     * Returns the selected generator.\n     */\n    get generator() {\n        return this._generator;\n    }\n    /**\n     * Signal triggered when the manager changes.\n     */\n    get changed() {\n        return this._changed;\n    }\n    /**\n     * Dispose.\n     */\n    dispose() {\n        this._sessionContext.kernelChanged.disconnect(this._onKernelChanged, this);\n    }\n    /**\n     * Get the selected toolbox's name.\n     *\n     * @returns The name of the toolbox.\n     */\n    getToolbox() {\n        return this._toolbox;\n    }\n    /**\n     * Set the selected toolbox.\n     *\n     * @argument name The name of the toolbox.\n     */\n    setToolbox(name) {\n        if (this._toolbox !== name) {\n            const toolbox = this._registry.toolboxes.get(name);\n            this._toolbox = toolbox ? name : 'default';\n            this._changed.emit('toolbox');\n        }\n    }\n    /**\n     * List the available toolboxes.\n     *\n     * @returns the list of available toolboxes for Blockly\n     */\n    listToolboxes() {\n        const list = [];\n        this._registry.toolboxes.forEach((toolbox, name) => {\n            list.push({ label: name, value: name });\n        });\n        return list;\n    }\n    /**\n     * Set the selected kernel.\n     *\n     * @argument name The name of the kernel.\n     */\n    selectKernel(name) {\n        this._sessionContext.changeKernel({ name });\n    }\n    /**\n     * List the available kernels.\n     *\n     * @returns the list of available kernels for Blockly\n     */\n    listKernels() {\n        const specs = this._sessionContext.specsManager.specs.kernelspecs;\n        const list = [];\n        Object.keys(specs).forEach(key => {\n            const language = specs[key].language;\n            if (this._registry.generators.has(language)) {\n                list.push({ label: specs[key].display_name, value: specs[key].name });\n            }\n        });\n        return list;\n    }\n    _onKernelChanged(sender, args) {\n        const specs = this._sessionContext.specsManager.specs.kernelspecs;\n        if (args.newValue && specs[args.newValue.name] !== undefined) {\n            this._selectedKernel = specs[args.newValue.name];\n            const language = specs[args.newValue.name].language;\n            this._generator = this._registry.generators.get(language);\n            this._changed.emit('kernel');\n        }\n    }\n}\n//# sourceMappingURL=manager.js.map",
-        "import { ABCWidgetFactory } from '@jupyterlab/docregistry';\nimport { BlocklyEditor, BlocklyPanel } from './widget';\nimport { BlocklyRegistry } from './registry';\nimport { BlocklyManager } from './manager';\n/**\n * A widget factory to create new instances of BlocklyEditor.\n */\nexport class BlocklyEditorFactory extends ABCWidgetFactory {\n    /**\n     * Constructor of BlocklyEditorFactory.\n     *\n     * @param options Constructor options\n     */\n    constructor(options) {\n        super(options);\n        this._registry = new BlocklyRegistry();\n        this._rendermime = options.rendermime;\n        this._mimetypeService = options.mimetypeService;\n    }\n    get registry() {\n        return this._registry;\n    }\n    /**\n     * Create a new widget given a context.\n     *\n     * @param context Contains the information of the file\n     * @returns The widget\n     */\n    createNewWidget(context) {\n        const manager = new BlocklyManager(this._registry, context.sessionContext, this._mimetypeService);\n        const content = new BlocklyPanel(context, manager, this._rendermime);\n        return new BlocklyEditor({ context, content, manager });\n    }\n}\n//# sourceMappingURL=factory.js.map",
+        "import { ABCWidgetFactory } from '@jupyterlab/docregistry';\nimport { BlocklyEditor, BlocklyPanel } from './widget';\nimport { BlocklyRegistry } from './registry';\nimport { BlocklyManager } from './manager';\n/**\n * A widget factory to create new instances of BlocklyEditor.\n */\nexport class BlocklyEditorFactory extends ABCWidgetFactory {\n    /**\n     * Constructor of BlocklyEditorFactory.\n     *\n     * @param options Constructor options\n     */\n    constructor(options) {\n        super(options);\n        this._registry = new BlocklyRegistry();\n        this._rendermime = options.rendermime;\n        this._mimetypeService = options.mimetypeService;\n    }\n    get registry() {\n        return this._registry;\n    }\n    /**\n     * Create a new widget given a context.\n     *\n     * @param context Contains the information of the file\n     * @returns The widget\n     */\n    createNewWidget(context) {\n        // Set a map to the model. The widgets manager expects a Notebook model\n        // but the only notebook property it uses is the metadata.\n        context.model['metadata'] = new Map();\n        const manager = new BlocklyManager(this._registry, context.sessionContext, this._mimetypeService);\n        const content = new BlocklyPanel(context, manager, this._rendermime);\n        return new BlocklyEditor({ context, content, manager });\n    }\n}\n//# sourceMappingURL=factory.js.map",
         "import { Token } from '@lumino/coreutils';\n/**\n * The registry token.\n */\nexport const IBlocklyRegistry = new Token('jupyterlab-blockly/registry');\n//# sourceMappingURL=token.js.map"
     ],
     "version": 3
 }
```

### Comparing `jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/839.c46366b4bade6ade8403.js` & `jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/839.c46366b4bade6ade8403.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/839.c46366b4bade6ade8403.js.map` & `jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/839.c46366b4bade6ade8403.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/929.d864f042fdaf411ba52b.js` & `jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/929.d864f042fdaf411ba52b.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/929.d864f042fdaf411ba52b.js.map` & `jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/929.d864f042fdaf411ba52b.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/939.973bc21fa6263dbabd09.js` & `jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/939.973bc21fa6263dbabd09.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/939.973bc21fa6263dbabd09.js.map` & `jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/939.973bc21fa6263dbabd09.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/974.5f4a862a240a7368a2b5.js` & `jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/974.5f4a862a240a7368a2b5.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/974.5f4a862a240a7368a2b5.js.map` & `jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/974.5f4a862a240a7368a2b5.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/remoteEntry.64321718d51bd0ccabe6.js` & `jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/remoteEntry.fd0c0fecc472143c1077.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -1,31 +1,31 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, a, n, o, f, c, d, l, i, b, u, s, p, h, y, v, m, g, j, w, k, P, x = {
+    var e, r, t, a, n, f, o, c, d, l, i, u, b, s, p, h, y, v, m, g, j, w, k, P, x = {
             1707: (e, r, t) => {
                 var a = {
-                        "./index": () => Promise.all([t.e(153), t.e(216)]).then((() => () => t(4216))),
-                        "./extension": () => Promise.all([t.e(153), t.e(216)]).then((() => () => t(4216))),
+                        "./index": () => Promise.all([t.e(955), t.e(216)]).then((() => () => t(4216))),
+                        "./extension": () => Promise.all([t.e(955), t.e(216)]).then((() => () => t(4216))),
                         "./style": () => t.e(643).then((() => () => t(6643)))
                     },
                     n = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
-                    o = (e, r) => {
+                    f = (e, r) => {
                         if (t.S) {
                             var a = "default",
                                 n = t.S[a];
                             if (n && n !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
                             return t.S[a] = e, t.I(a, r)
                         }
                     };
                 t.d(r, {
                     get: () => n,
-                    init: () => o
+                    init: () => f
                 })
             }
         },
         O = {};
 
     function S(e) {
         var r = O[e];
@@ -45,34 +45,33 @@
         if (1 & a && (t = this(t)), 8 & a) return t;
         if ("object" == typeof t && t) {
             if (4 & a && t.__esModule) return t;
             if (16 & a && "function" == typeof t.then) return t
         }
         var n = Object.create(null);
         S.r(n);
-        var o = {};
+        var f = {};
         e = e || [null, r({}), r([]), r(r)];
-        for (var f = 2 & a && t;
-            "object" == typeof f && !~e.indexOf(f); f = r(f)) Object.getOwnPropertyNames(f).forEach((e => o[e] = () => t[e]));
-        return o.default = () => t, S.d(n, o), n
+        for (var o = 2 & a && t;
+            "object" == typeof o && !~e.indexOf(o); o = r(o)) Object.getOwnPropertyNames(o).forEach((e => f[e] = () => t[e]));
+        return f.default = () => t, S.d(n, f), n
     }, S.d = (e, r) => {
         for (var t in r) S.o(r, t) && !S.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, S.f = {}, S.e = e => Promise.all(Object.keys(S.f).reduce(((r, t) => (S.f[t](e, r), r)), [])), S.u = e => e + "." + {
         31: "418331b4a22dffe518b4",
         109: "624848fd57458c5dd4f0",
-        153: "6a8fe9147a69d0d5e1ff",
         157: "921bbfb16083689ff62a",
         168: "8383bc2d0a83f2b959fd",
         173: "df5a30c1440df850aa82",
         210: "35c06ed0583039490182",
         215: "82ec42ef5a24d2ff187f",
-        216: "011d737685936c4c8e1a",
+        216: "751d5114e75a3795211f",
         232: "d5cb8a2dcc0d34fabd8a",
         268: "4eaefedf266ea50fd6df",
         326: "f8d1ef211f999b0b3dca",
         382: "0016faf875cb665ac9b2",
         410: "941cb48faa5e2d568b13",
         428: "cb1cafd5e6ba8a81b05a",
         513: "5646d474a0e4d9613886",
@@ -86,29 +85,29 @@
         643: "34f4f43b70e246a962a8",
         647: "d729bd3d64d38278f913",
         655: "13bd86e04776bccddcee",
         671: "5cc50d235d821a731440",
         693: "91ee036f7a5bf0e5a1b0",
         698: "48373f0b62bef71acebe",
         704: "cf482c52df64c1afcb10",
-        835: "cbd12870eccd44d69cf0",
+        835: "6f7e7b701fee67a1ec53",
         839: "c46366b4bade6ade8403",
         929: "d864f042fdaf411ba52b",
         939: "973bc21fa6263dbabd09",
+        955: "324ee5220abd1dc68556",
         974: "5f4a862a240a7368a2b5"
     } [e] + ".js?v=" + {
         31: "418331b4a22dffe518b4",
         109: "624848fd57458c5dd4f0",
-        153: "6a8fe9147a69d0d5e1ff",
         157: "921bbfb16083689ff62a",
         168: "8383bc2d0a83f2b959fd",
         173: "df5a30c1440df850aa82",
         210: "35c06ed0583039490182",
         215: "82ec42ef5a24d2ff187f",
-        216: "011d737685936c4c8e1a",
+        216: "751d5114e75a3795211f",
         232: "d5cb8a2dcc0d34fabd8a",
         268: "4eaefedf266ea50fd6df",
         326: "f8d1ef211f999b0b3dca",
         382: "0016faf875cb665ac9b2",
         410: "941cb48faa5e2d568b13",
         428: "cb1cafd5e6ba8a81b05a",
         513: "5646d474a0e4d9613886",
@@ -122,49 +121,50 @@
         643: "34f4f43b70e246a962a8",
         647: "d729bd3d64d38278f913",
         655: "13bd86e04776bccddcee",
         671: "5cc50d235d821a731440",
         693: "91ee036f7a5bf0e5a1b0",
         698: "48373f0b62bef71acebe",
         704: "cf482c52df64c1afcb10",
-        835: "cbd12870eccd44d69cf0",
+        835: "6f7e7b701fee67a1ec53",
         839: "c46366b4bade6ade8403",
         929: "d864f042fdaf411ba52b",
         939: "973bc21fa6263dbabd09",
+        955: "324ee5220abd1dc68556",
         974: "5f4a862a240a7368a2b5"
     } [e], S.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), S.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), t = {}, a = "jupyterlab-blockly-extension:", S.l = (e, r, n, o) => {
+    }(), S.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), t = {}, a = "jupyterlab-blockly-extension:", S.l = (e, r, n, f) => {
         if (t[e]) t[e].push(r);
         else {
-            var f, c;
+            var o, c;
             if (void 0 !== n)
                 for (var d = document.getElementsByTagName("script"), l = 0; l < d.length; l++) {
                     var i = d[l];
                     if (i.getAttribute("src") == e || i.getAttribute("data-webpack") == a + n) {
-                        f = i;
+                        o = i;
                         break
                     }
                 }
-            f || (c = !0, (f = document.createElement("script")).charset = "utf-8", f.timeout = 120, S.nc && f.setAttribute("nonce", S.nc), f.setAttribute("data-webpack", a + n), f.src = e), t[e] = [r];
-            var b = (r, a) => {
-                    f.onerror = f.onload = null, clearTimeout(u);
+            o || (c = !0, (o = document.createElement("script")).charset = "utf-8", o.timeout = 120, S.nc && o.setAttribute("nonce", S.nc), o.setAttribute("data-webpack", a + n), o.src = e), t[e] = [r];
+            var u = (r, a) => {
+                    o.onerror = o.onload = null, clearTimeout(b);
                     var n = t[e];
-                    if (delete t[e], f.parentNode && f.parentNode.removeChild(f), n && n.forEach((e => e(a))), r) return r(a)
+                    if (delete t[e], o.parentNode && o.parentNode.removeChild(o), n && n.forEach((e => e(a))), r) return r(a)
                 },
-                u = setTimeout(b.bind(null, void 0, {
+                b = setTimeout(u.bind(null, void 0, {
                     type: "timeout",
-                    target: f
+                    target: o
                 }), 12e4);
-            f.onerror = b.bind(null, f.onerror), f.onload = b.bind(null, f.onload), c && document.head.appendChild(f)
+            o.onerror = u.bind(null, o.onerror), o.onload = u.bind(null, o.onload), c && document.head.appendChild(o)
         }
     }, S.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -174,27 +174,27 @@
             r = {};
         S.I = (t, a) => {
             a || (a = []);
             var n = r[t];
             if (n || (n = r[t] = {}), !(a.indexOf(n) >= 0)) {
                 if (a.push(n), e[t]) return e[t];
                 S.o(S.S, t) || (S.S[t] = {});
-                var o = S.S[t],
-                    f = "jupyterlab-blockly-extension",
+                var f = S.S[t],
+                    o = "jupyterlab-blockly-extension",
                     c = (e, r, t, a) => {
-                        var n = o[e] = o[e] || {},
+                        var n = f[e] = f[e] || {},
                             c = n[r];
-                        (!c || !c.loaded && (!a != !c.eager ? a : f > c.from)) && (n[r] = {
+                        (!c || !c.loaded && (!a != !c.eager ? a : o > c.from)) && (n[r] = {
                             get: t,
-                            from: f,
+                            from: o,
                             eager: !!a
                         })
                     },
                     d = [];
-                return "default" === t && (c("blockly", "9.2.1", (() => Promise.all([S.e(215), S.e(593)]).then((() => () => S(593))))), c("jupyterlab-blockly-extension", "0.3.0-alpha.0", (() => Promise.all([S.e(153), S.e(216)]).then((() => () => S(4216))))), c("jupyterlab-blockly", "0.3.0-alpha.0", (() => Promise.all([S.e(215), S.e(839), S.e(835), S.e(153)]).then((() => () => S(2835)))))), e[t] = d.length ? Promise.all(d).then((() => e[t] = 1)) : 1
+                return "default" === t && (c("blockly", "9.2.1", (() => Promise.all([S.e(215), S.e(593)]).then((() => () => S(593))))), c("jupyterlab-blockly-extension", "0.3.0-alpha.1", (() => Promise.all([S.e(955), S.e(216)]).then((() => () => S(4216))))), c("jupyterlab-blockly", "0.3.0-alpha.1", (() => Promise.all([S.e(215), S.e(839), S.e(835), S.e(955)]).then((() => () => S(2835)))))), e[t] = d.length ? Promise.all(d).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         S.g.importScripts && (e = S.g.location + "");
         var r = S.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -204,129 +204,131 @@
         if (!e) throw new Error("Automatic publicPath is not supported in this browser");
         e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), S.p = e
     })(), n = e => {
         var r = e => e.split(".").map((e => +e == e ? +e : e)),
             t = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
             a = t[1] ? r(t[1]) : [];
         return t[2] && (a.length++, a.push.apply(a, r(t[2]))), t[3] && (a.push([]), a.push.apply(a, r(t[3]))), a
-    }, o = (e, r) => {
+    }, f = (e, r) => {
         e = n(e), r = n(r);
         for (var t = 0;;) {
             if (t >= e.length) return t < r.length && "u" != (typeof r[t])[0];
             var a = e[t],
-                o = (typeof a)[0];
-            if (t >= r.length) return "u" == o;
-            var f = r[t],
-                c = (typeof f)[0];
-            if (o != c) return "o" == o && "n" == c || "s" == c || "u" == o;
-            if ("o" != o && "u" != o && a != f) return a < f;
+                f = (typeof a)[0];
+            if (t >= r.length) return "u" == f;
+            var o = r[t],
+                c = (typeof o)[0];
+            if (f != c) return "o" == f && "n" == c || "s" == c || "u" == f;
+            if ("o" != f && "u" != f && a != o) return a < o;
             t++
         }
-    }, f = e => {
+    }, o = e => {
         var r = e[0],
             t = "";
         if (1 === e.length) return "*";
         if (r + .5) {
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
             for (var a = 1, n = 1; n < e.length; n++) a--, t += "u" == (typeof(c = e[n]))[0] ? "-" : (a > 0 ? "." : "") + (a = 2, c);
             return t
         }
-        var o = [];
+        var f = [];
         for (n = 1; n < e.length; n++) {
             var c = e[n];
-            o.push(0 === c ? "not(" + d() + ")" : 1 === c ? "(" + d() + " || " + d() + ")" : 2 === c ? o.pop() + " " + o.pop() : f(c))
+            f.push(0 === c ? "not(" + d() + ")" : 1 === c ? "(" + d() + " || " + d() + ")" : 2 === c ? f.pop() + " " + f.pop() : o(c))
         }
         return d();
 
         function d() {
-            return o.pop().replace(/^\((.+)\)$/, "$1")
+            return f.pop().replace(/^\((.+)\)$/, "$1")
         }
     }, c = (e, r) => {
         if (0 in e) {
             r = n(r);
             var t = e[0],
                 a = t < 0;
             a && (t = -t - 1);
-            for (var o = 0, f = 1, d = !0;; f++, o++) {
-                var l, i, b = f < e.length ? (typeof e[f])[0] : "";
-                if (o >= r.length || "o" == (i = (typeof(l = r[o]))[0])) return !d || ("u" == b ? f > t && !a : "" == b != a);
+            for (var f = 0, o = 1, d = !0;; o++, f++) {
+                var l, i, u = o < e.length ? (typeof e[o])[0] : "";
+                if (f >= r.length || "o" == (i = (typeof(l = r[f]))[0])) return !d || ("u" == u ? o > t && !a : "" == u != a);
                 if ("u" == i) {
-                    if (!d || "u" != b) return !1
+                    if (!d || "u" != u) return !1
                 } else if (d)
-                    if (b == i)
-                        if (f <= t) {
-                            if (l != e[f]) return !1
+                    if (u == i)
+                        if (o <= t) {
+                            if (l != e[o]) return !1
                         } else {
-                            if (a ? l > e[f] : l < e[f]) return !1;
-                            l != e[f] && (d = !1)
+                            if (a ? l > e[o] : l < e[o]) return !1;
+                            l != e[o] && (d = !1)
                         }
-                else if ("s" != b && "n" != b) {
-                    if (a || f <= t) return !1;
-                    d = !1, f--
+                else if ("s" != u && "n" != u) {
+                    if (a || o <= t) return !1;
+                    d = !1, o--
                 } else {
-                    if (f <= t || i < b != a) return !1;
+                    if (o <= t || i < u != a) return !1;
                     d = !1
-                } else "s" != b && "n" != b && (d = !1, f--)
+                } else "s" != u && "n" != u && (d = !1, o--)
             }
         }
-        var u = [],
-            s = u.pop.bind(u);
-        for (o = 1; o < e.length; o++) {
-            var p = e[o];
-            u.push(1 == p ? s() | s() : 2 == p ? s() & s() : p ? c(p, r) : !s())
+        var b = [],
+            s = b.pop.bind(b);
+        for (f = 1; f < e.length; f++) {
+            var p = e[f];
+            b.push(1 == p ? s() | s() : 2 == p ? s() & s() : p ? c(p, r) : !s())
         }
         return !!s()
     }, d = (e, r) => {
         var t = S.S[e];
         if (!t || !S.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, l = (e, r) => {
         var t = e[r];
-        return (r = Object.keys(t).reduce(((e, r) => !e || o(e, r) ? r : e), 0)) && t[r]
+        return (r = Object.keys(t).reduce(((e, r) => !e || f(e, r) ? r : e), 0)) && t[r]
     }, i = (e, r) => {
         var t = e[r];
-        return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && o(e, r) ? r : e), 0)
-    }, b = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + f(a) + ")", u = (e, r, t, a) => {
+        return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && f(e, r) ? r : e), 0)
+    }, u = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(a) + ")", b = (e, r, t, a) => {
         var n = i(e, t);
-        return c(a, n) || "undefined" != typeof console && console.warn && console.warn(b(e, t, n, a)), y(e[t][n])
+        return c(a, n) || "undefined" != typeof console && console.warn && console.warn(u(e, t, n, a)), y(e[t][n])
     }, s = (e, r, t) => {
         var a = e[r];
-        return (r = Object.keys(a).reduce(((e, r) => !c(t, r) || e && !o(e, r) ? e : r), 0)) && a[r]
+        return (r = Object.keys(a).reduce(((e, r) => !c(t, r) || e && !f(e, r) ? e : r), 0)) && a[r]
     }, p = (e, r, t, a) => {
         var n = e[t];
-        return "No satisfying version (" + f(a) + ") of shared module " + t + " found in shared scope " + r + ".\nAvailable versions: " + Object.keys(n).map((e => e + " from " + n[e].from)).join(", ")
+        return "No satisfying version (" + o(a) + ") of shared module " + t + " found in shared scope " + r + ".\nAvailable versions: " + Object.keys(n).map((e => e + " from " + n[e].from)).join(", ")
     }, h = (e, r, t, a) => {
         "undefined" != typeof console && console.warn && console.warn(p(e, r, t, a))
     }, y = e => (e.loaded = 1, e.get()), m = (v = e => function(r, t, a, n) {
-        var o = S.I(r);
-        return o && o.then ? o.then(e.bind(e, r, S.S[r], t, a, n)) : e(r, S.S[r], t, a, n)
-    })(((e, r, t, a) => (d(e, t), y(s(r, t, a) || h(r, e, t, a) || l(r, t))))), g = v(((e, r, t, a) => (d(e, t), u(r, 0, t, a)))), j = v(((e, r, t, a, n) => r && S.o(r, t) ? u(r, 0, t, a) : n())), w = {}, k = {
-        5510: () => g("default", "@jupyterlab/apputils", [1, 3, 6, 1]),
-        6591: () => g("default", "@jupyterlab/ui-components", [1, 3, 6, 1]),
-        841: () => g("default", "@jupyterlab/rendermime", [1, 3, 6, 1]),
-        1279: () => g("default", "@jupyterlab/launcher", [1, 3, 6, 1]),
-        1598: () => g("default", "@jupyterlab/settingregistry", [1, 3, 6, 1]),
-        3535: () => g("default", "@jupyterlab/filebrowser", [1, 3, 6, 1]),
-        3591: () => j("default", "jupyterlab-blockly", [2, 0, 3, 0, , "alpha", 0], (() => Promise.all([S.e(215), S.e(839), S.e(835)]).then((() => () => S(2835))))),
-        3606: () => g("default", "@jupyterlab/codeeditor", [1, 3, 6, 1]),
-        5442: () => g("default", "@jupyterlab/translation", [1, 3, 6, 1]),
-        5705: () => g("default", "@jupyterlab/mainmenu", [1, 3, 6, 1]),
-        6866: () => g("default", "@jupyterlab/application", [1, 3, 6, 1]),
+        var f = S.I(r);
+        return f && f.then ? f.then(e.bind(e, r, S.S[r], t, a, n)) : e(r, S.S[r], t, a, n)
+    })(((e, r, t, a) => (d(e, t), y(s(r, t, a) || h(r, e, t, a) || l(r, t))))), g = v(((e, r, t, a) => (d(e, t), b(r, 0, t, a)))), j = v(((e, r, t, a, n) => r && S.o(r, t) ? b(r, 0, t, a) : n())), w = {}, k = {
+        2502: () => g("default", "@jupyterlab/ui-components", [1, 3, 6, 3]),
+        3033: () => g("default", "@jupyterlab/apputils", [1, 3, 6, 3]),
+        1467: () => g("default", "@jupyterlab/launcher", [1, 3, 6, 3]),
+        2086: () => g("default", "@jupyterlab/rendermime", [1, 3, 6, 3]),
+        2486: () => g("default", "@jupyterlab/codeeditor", [1, 3, 6, 3]),
+        2673: () => g("default", "@jupyter-widgets/base", [1, 6, 0, 4]),
+        3169: () => g("default", "@jupyterlab/translation", [1, 3, 6, 3]),
+        4038: () => g("default", "@jupyterlab/settingregistry", [1, 3, 6, 3]),
+        5344: () => g("default", "@jupyterlab/mainmenu", [1, 3, 6, 3]),
+        5687: () => g("default", "@jupyterlab/application", [1, 3, 6, 3]),
+        7280: () => g("default", "@jupyterlab/filebrowser", [1, 3, 6, 3]),
+        8916: () => j("default", "jupyterlab-blockly", [2, 0, 3, 0, , "alpha", 1], (() => Promise.all([S.e(215), S.e(839), S.e(835)]).then((() => () => S(2835))))),
+        9814: () => g("default", "@jupyter-widgets/jupyterlab-manager", [1, 5, 0, 7]),
+        819: () => m("default", "@jupyterlab/docregistry", [1, 3, 6, 3]),
         1041: () => j("default", "blockly", [1, 9, 2, 1], (() => S.e(593).then((() => () => S(593))))),
-        1431: () => g("default", "@lumino/widgets", [1, 1, 37, 1]),
         1526: () => g("default", "@lumino/coreutils", [1, 1, 11, 0]),
         1840: () => g("default", "@lumino/signaling", [1, 1, 10, 0]),
-        1952: () => m("default", "@jupyterlab/cells", [1, 3, 6, 1]),
-        4379: () => m("default", "@jupyterlab/docregistry", [1, 3, 6, 1]),
+        2191: () => m("default", "@jupyterlab/cells", [1, 3, 6, 3]),
         6271: () => g("default", "react", [1, 17, 0, 1]),
+        8832: () => g("default", "@lumino/widgets", [1, 1, 37, 2]),
         8918: () => g("default", "@lumino/algorithm", [1, 1, 9, 0])
     }, P = {
-        153: [5510, 6591],
-        216: [841, 1279, 1598, 3535, 3591, 3606, 5442, 5705, 6866],
-        835: [1041, 1431, 1526, 1840, 1952, 4379, 6271, 8918]
+        216: [1467, 2086, 2486, 2673, 3169, 4038, 5344, 5687, 7280, 8916, 9814],
+        835: [819, 1041, 1526, 1840, 2191, 6271, 8832, 8918],
+        955: [2502, 3033]
     }, S.f.consumes = (e, r) => {
         S.o(P, e) && P[e].forEach((e => {
             if (S.o(w, e)) return r.push(w[e]);
             var t = r => {
                     w[e] = 0, S.m[e] = t => {
                         delete S.c[e], t.exports = r()
                     }
@@ -347,37 +349,37 @@
         var e = {
             380: 0
         };
         S.f.j = (r, t) => {
             var a = S.o(e, r) ? e[r] : void 0;
             if (0 !== a)
                 if (a) t.push(a[2]);
-                else if (153 != r) {
+                else if (955 != r) {
                 var n = new Promise(((t, n) => a = e[r] = [t, n]));
                 t.push(a[2] = n);
-                var o = S.p + S.u(r),
-                    f = new Error;
-                S.l(o, (t => {
+                var f = S.p + S.u(r),
+                    o = new Error;
+                S.l(f, (t => {
                     if (S.o(e, r) && (0 !== (a = e[r]) && (e[r] = void 0), a)) {
                         var n = t && ("load" === t.type ? "missing" : t.type),
-                            o = t && t.target && t.target.src;
-                        f.message = "Loading chunk " + r + " failed.\n(" + n + ": " + o + ")", f.name = "ChunkLoadError", f.type = n, f.request = o, a[1](f)
+                            f = t && t.target && t.target.src;
+                        o.message = "Loading chunk " + r + " failed.\n(" + n + ": " + f + ")", o.name = "ChunkLoadError", o.type = n, o.request = f, a[1](o)
                     }
                 }), "chunk-" + r, r)
             } else e[r] = 0
         };
         var r = (r, t) => {
-                var a, n, [o, f, c] = t,
+                var a, n, [f, o, c] = t,
                     d = 0;
-                if (o.some((r => 0 !== e[r]))) {
-                    for (a in f) S.o(f, a) && (S.m[a] = f[a]);
+                if (f.some((r => 0 !== e[r]))) {
+                    for (a in o) S.o(o, a) && (S.m[a] = o[a]);
                     c && c(S)
                 }
-                for (r && r(t); d < o.length; d++) n = o[d], S.o(e, n) && e[n] && e[n][0](), e[n] = 0
+                for (r && r(t); d < f.length; d++) n = f[d], S.o(e, n) && e[n] && e[n][0](), e[n] = 0
             },
             t = self.webpackChunkjupyterlab_blockly_extension = self.webpackChunkjupyterlab_blockly_extension || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), S.nc = void 0;
     var _ = S(1707);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["jupyterlab-blockly-extension"] = _
 })();
-//# sourceMappingURL=remoteEntry.64321718d51bd0ccabe6.js.map
+//# sourceMappingURL=remoteEntry.fd0c0fecc472143c1077.js.map
```

### Comparing `jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/remoteEntry.64321718d51bd0ccabe6.js.map` & `jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/remoteEntry.fd0c0fecc472143c1077.js.map`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8246753246753247%*

 * *Differences: {"'file'": "'remoteEntry.fd0c0fecc472143c1077.js'",*

 * * "'mappings'": "'uCACIA,EADAC,ECAAC,EACAC,ECDAC,EAIAC,EAIAC,EAIAC,EAIAC,EAKAC,EAOAC,EAMAC,EAOAC,EAUAC,EAQAC,EAYAC,EAGAC,EAIAC,EAaAC,EAQAC,EAoBAC,EAYAC,EACAC,EAwBAC,E,kBC5JJ,IAAIC,EAAY,CACf,UAAW,IACHC,QAAQC,IAAI,CAACC,EAAoBC,EAAE,KAAMD,EAAoBC,EAAE,OAAOC,MAAK,IAAM,IAASF,EAAoB,QAEtH,cAAe,IACPF,QAAQC,IAAI,CAACC,EAAoBC,EAAE,KAAMD,EAAoBC,EAAE,OAAOC,MAAK,IAAM,IAASF,EAAoB,QAEtH,UAAW,IACHA,EAAoBC,EAAE,KAAKC,MAAK,IAAM,IAASF,EAAoB,SAGxEX,EAAM,CAACc,EAAQC,KAClBJ,EAAoB […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "remoteEntry.64321718d51bd0ccabe6.js",
-    "mappings": "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",
+    "file": "remoteEntry.fd0c0fecc472143c1077.js",
+    "mappings": "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",
     "names": [
         "leafPrototypes",
         "getProto",
         "inProgress",
         "dataWebpackPrefix",
         "parseVersion",
         "versionLt",
@@ -205,25 +205,25 @@
         "webpack://jupyterlab-blockly-extension/webpack/runtime/jsonp chunk loading",
         "webpack://jupyterlab-blockly-extension/webpack/runtime/nonce",
         "webpack://jupyterlab-blockly-extension/webpack/startup"
     ],
     "sourcesContent": [
         "var getProto = Object.getPrototypeOf ? (obj) => (Object.getPrototypeOf(obj)) : (obj) => (obj.__proto__);\nvar leafPrototypes;\n// create a fake namespace object\n// mode & 1: value is a module id, require it\n// mode & 2: merge all properties of value into the ns\n// mode & 4: return value when already ns object\n// mode & 16: return value when it's Promise-like\n// mode & 8|1: behave like require\n__webpack_require__.t = function(value, mode) {\n\tif(mode & 1) value = this(value);\n\tif(mode & 8) return value;\n\tif(typeof value === 'object' && value) {\n\t\tif((mode & 4) && value.__esModule) return value;\n\t\tif((mode & 16) && typeof value.then === 'function') return value;\n\t}\n\tvar ns = Object.create(null);\n\t__webpack_require__.r(ns);\n\tvar def = {};\n\tleafPrototypes = leafPrototypes || [null, getProto({}), getProto([]), getProto(getProto)];\n\tfor(var current = mode & 2 && value; typeof current == 'object' && !~leafPrototypes.indexOf(current); current = getProto(current)) {\n\t\tObject.getOwnPropertyNames(current).forEach((key) => (def[key] = () => (value[key])));\n\t}\n\tdef['default'] = () => (value);\n\t__webpack_require__.d(ns, def);\n\treturn ns;\n};",
         "var inProgress = {};\nvar dataWebpackPrefix = \"jupyterlab-blockly-extension:\";\n// loadScript function to load a script via script tag\n__webpack_require__.l = (url, done, key, chunkId) => {\n\tif(inProgress[url]) { inProgress[url].push(done); return; }\n\tvar script, needAttach;\n\tif(key !== undefined) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tfor(var i = 0; i < scripts.length; i++) {\n\t\t\tvar s = scripts[i];\n\t\t\tif(s.getAttribute(\"src\") == url || s.getAttribute(\"data-webpack\") == dataWebpackPrefix + key) { script = s; break; }\n\t\t}\n\t}\n\tif(!script) {\n\t\tneedAttach = true;\n\t\tscript = document.createElement('script');\n\n\t\tscript.charset = 'utf-8';\n\t\tscript.timeout = 120;\n\t\tif (__webpack_require__.nc) {\n\t\t\tscript.setAttribute(\"nonce\", __webpack_require__.nc);\n\t\t}\n\t\tscript.setAttribute(\"data-webpack\", dataWebpackPrefix + key);\n\t\tscript.src = url;\n\t}\n\tinProgress[url] = [done];\n\tvar onScriptComplete = (prev, event) => {\n\t\t// avoid mem leaks in IE.\n\t\tscript.onerror = script.onload = null;\n\t\tclearTimeout(timeout);\n\t\tvar doneFns = inProgress[url];\n\t\tdelete inProgress[url];\n\t\tscript.parentNode && script.parentNode.removeChild(script);\n\t\tdoneFns && doneFns.forEach((fn) => (fn(event)));\n\t\tif(prev) return prev(event);\n\t};\n\tvar timeout = setTimeout(onScriptComplete.bind(null, undefined, { type: 'timeout', target: script }), 120000);\n\tscript.onerror = onScriptComplete.bind(null, script.onerror);\n\tscript.onload = onScriptComplete.bind(null, script.onload);\n\tneedAttach && document.head.appendChild(script);\n};",
-        "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) typeof console !== \"undefined\" && console.warn && console.warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\ttypeof console !== \"undefined\" && console.warn && console.warn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t5510: () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/apputils\", [1,3,6,1])),\n\t6591: () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/ui-components\", [1,3,6,1])),\n\t841: () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/rendermime\", [1,3,6,1])),\n\t1279: () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/launcher\", [1,3,6,1])),\n\t1598: () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/settingregistry\", [1,3,6,1])),\n\t3535: () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/filebrowser\", [1,3,6,1])),\n\t3591: () => (loadSingletonVersionCheckFallback(\"default\", \"jupyterlab-blockly\", [2,0,3,0,,\"alpha\",0], () => (Promise.all([__webpack_require__.e(215), __webpack_require__.e(839), __webpack_require__.e(835)]).then(() => (() => (__webpack_require__(2835))))))),\n\t3606: () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/codeeditor\", [1,3,6,1])),\n\t5442: () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/translation\", [1,3,6,1])),\n\t5705: () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/mainmenu\", [1,3,6,1])),\n\t6866: () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/application\", [1,3,6,1])),\n\t1041: () => (loadSingletonVersionCheckFallback(\"default\", \"blockly\", [1,9,2,1], () => (__webpack_require__.e(593).then(() => (() => (__webpack_require__(593))))))),\n\t1431: () => (loadSingletonVersionCheck(\"default\", \"@lumino/widgets\", [1,1,37,1])),\n\t1526: () => (loadSingletonVersionCheck(\"default\", \"@lumino/coreutils\", [1,1,11,0])),\n\t1840: () => (loadSingletonVersionCheck(\"default\", \"@lumino/signaling\", [1,1,10,0])),\n\t1952: () => (loadVersionCheck(\"default\", \"@jupyterlab/cells\", [1,3,6,1])),\n\t4379: () => (loadVersionCheck(\"default\", \"@jupyterlab/docregistry\", [1,3,6,1])),\n\t6271: () => (loadSingletonVersionCheck(\"default\", \"react\", [1,17,0,1])),\n\t8918: () => (loadSingletonVersionCheck(\"default\", \"@lumino/algorithm\", [1,1,9,0]))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"153\": [\n\t\t5510,\n\t\t6591\n\t],\n\t\"216\": [\n\t\t841,\n\t\t1279,\n\t\t1598,\n\t\t3535,\n\t\t3591,\n\t\t3606,\n\t\t5442,\n\t\t5705,\n\t\t6866\n\t],\n\t\"835\": [\n\t\t1041,\n\t\t1431,\n\t\t1526,\n\t\t1840,\n\t\t1952,\n\t\t4379,\n\t\t6271,\n\t\t8918\n\t]\n};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t});\n\t}\n}",
-        "var moduleMap = {\n\t\"./index\": () => {\n\t\treturn Promise.all([__webpack_require__.e(153), __webpack_require__.e(216)]).then(() => (() => ((__webpack_require__(4216)))));\n\t},\n\t\"./extension\": () => {\n\t\treturn Promise.all([__webpack_require__.e(153), __webpack_require__.e(216)]).then(() => (() => ((__webpack_require__(4216)))));\n\t},\n\t\"./style\": () => {\n\t\treturn __webpack_require__.e(643).then(() => (() => ((__webpack_require__(6643)))));\n\t}\n};\nvar get = (module, getScope) => {\n\t__webpack_require__.R = getScope;\n\tgetScope = (\n\t\t__webpack_require__.o(moduleMap, module)\n\t\t\t? moduleMap[module]()\n\t\t\t: Promise.resolve().then(() => {\n\t\t\t\tthrow new Error('Module \"' + module + '\" does not exist in container.');\n\t\t\t})\n\t);\n\t__webpack_require__.R = undefined;\n\treturn getScope;\n};\nvar init = (shareScope, initScope) => {\n\tif (!__webpack_require__.S) return;\n\tvar name = \"default\"\n\tvar oldScope = __webpack_require__.S[name];\n\tif(oldScope && oldScope !== shareScope) throw new Error(\"Container initialization failed as it has already been initialized with a different share scope\");\n\t__webpack_require__.S[name] = shareScope;\n\treturn __webpack_require__.I(name, initScope);\n};\n\n// This exports getters to disallow modifications\n__webpack_require__.d(exports, {\n\tget: () => (get),\n\tinit: () => (init)\n});",
+        "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) typeof console !== \"undefined\" && console.warn && console.warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\ttypeof console !== \"undefined\" && console.warn && console.warn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t2502: () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/ui-components\", [1,3,6,3])),\n\t3033: () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/apputils\", [1,3,6,3])),\n\t1467: () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/launcher\", [1,3,6,3])),\n\t2086: () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/rendermime\", [1,3,6,3])),\n\t2486: () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/codeeditor\", [1,3,6,3])),\n\t2673: () => (loadSingletonVersionCheck(\"default\", \"@jupyter-widgets/base\", [1,6,0,4])),\n\t3169: () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/translation\", [1,3,6,3])),\n\t4038: () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/settingregistry\", [1,3,6,3])),\n\t5344: () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/mainmenu\", [1,3,6,3])),\n\t5687: () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/application\", [1,3,6,3])),\n\t7280: () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/filebrowser\", [1,3,6,3])),\n\t8916: () => (loadSingletonVersionCheckFallback(\"default\", \"jupyterlab-blockly\", [2,0,3,0,,\"alpha\",1], () => (Promise.all([__webpack_require__.e(215), __webpack_require__.e(839), __webpack_require__.e(835)]).then(() => (() => (__webpack_require__(2835))))))),\n\t9814: () => (loadSingletonVersionCheck(\"default\", \"@jupyter-widgets/jupyterlab-manager\", [1,5,0,7])),\n\t819: () => (loadVersionCheck(\"default\", \"@jupyterlab/docregistry\", [1,3,6,3])),\n\t1041: () => (loadSingletonVersionCheckFallback(\"default\", \"blockly\", [1,9,2,1], () => (__webpack_require__.e(593).then(() => (() => (__webpack_require__(593))))))),\n\t1526: () => (loadSingletonVersionCheck(\"default\", \"@lumino/coreutils\", [1,1,11,0])),\n\t1840: () => (loadSingletonVersionCheck(\"default\", \"@lumino/signaling\", [1,1,10,0])),\n\t2191: () => (loadVersionCheck(\"default\", \"@jupyterlab/cells\", [1,3,6,3])),\n\t6271: () => (loadSingletonVersionCheck(\"default\", \"react\", [1,17,0,1])),\n\t8832: () => (loadSingletonVersionCheck(\"default\", \"@lumino/widgets\", [1,1,37,2])),\n\t8918: () => (loadSingletonVersionCheck(\"default\", \"@lumino/algorithm\", [1,1,9,0]))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"216\": [\n\t\t1467,\n\t\t2086,\n\t\t2486,\n\t\t2673,\n\t\t3169,\n\t\t4038,\n\t\t5344,\n\t\t5687,\n\t\t7280,\n\t\t8916,\n\t\t9814\n\t],\n\t\"835\": [\n\t\t819,\n\t\t1041,\n\t\t1526,\n\t\t1840,\n\t\t2191,\n\t\t6271,\n\t\t8832,\n\t\t8918\n\t],\n\t\"955\": [\n\t\t2502,\n\t\t3033\n\t]\n};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t});\n\t}\n}",
+        "var moduleMap = {\n\t\"./index\": () => {\n\t\treturn Promise.all([__webpack_require__.e(955), __webpack_require__.e(216)]).then(() => (() => ((__webpack_require__(4216)))));\n\t},\n\t\"./extension\": () => {\n\t\treturn Promise.all([__webpack_require__.e(955), __webpack_require__.e(216)]).then(() => (() => ((__webpack_require__(4216)))));\n\t},\n\t\"./style\": () => {\n\t\treturn __webpack_require__.e(643).then(() => (() => ((__webpack_require__(6643)))));\n\t}\n};\nvar get = (module, getScope) => {\n\t__webpack_require__.R = getScope;\n\tgetScope = (\n\t\t__webpack_require__.o(moduleMap, module)\n\t\t\t? moduleMap[module]()\n\t\t\t: Promise.resolve().then(() => {\n\t\t\t\tthrow new Error('Module \"' + module + '\" does not exist in container.');\n\t\t\t})\n\t);\n\t__webpack_require__.R = undefined;\n\treturn getScope;\n};\nvar init = (shareScope, initScope) => {\n\tif (!__webpack_require__.S) return;\n\tvar name = \"default\"\n\tvar oldScope = __webpack_require__.S[name];\n\tif(oldScope && oldScope !== shareScope) throw new Error(\"Container initialization failed as it has already been initialized with a different share scope\");\n\t__webpack_require__.S[name] = shareScope;\n\treturn __webpack_require__.I(name, initScope);\n};\n\n// This exports getters to disallow modifications\n__webpack_require__.d(exports, {\n\tget: () => (get),\n\tinit: () => (init)\n});",
         "// The module cache\nvar __webpack_module_cache__ = {};\n\n// The require function\nfunction __webpack_require__(moduleId) {\n\t// Check if module is in cache\n\tvar cachedModule = __webpack_module_cache__[moduleId];\n\tif (cachedModule !== undefined) {\n\t\treturn cachedModule.exports;\n\t}\n\t// Create a new module (and put it into the cache)\n\tvar module = __webpack_module_cache__[moduleId] = {\n\t\tid: moduleId,\n\t\t// no module.loaded needed\n\t\texports: {}\n\t};\n\n\t// Execute the module function\n\t__webpack_modules__[moduleId].call(module.exports, module, module.exports, __webpack_require__);\n\n\t// Return the exports of the module\n\treturn module.exports;\n}\n\n// expose the modules object (__webpack_modules__)\n__webpack_require__.m = __webpack_modules__;\n\n// expose the module cache\n__webpack_require__.c = __webpack_module_cache__;\n\n",
         "// getDefaultExport function for compatibility with non-harmony modules\n__webpack_require__.n = (module) => {\n\tvar getter = module && module.__esModule ?\n\t\t() => (module['default']) :\n\t\t() => (module);\n\t__webpack_require__.d(getter, { a: getter });\n\treturn getter;\n};",
         "// define getter functions for harmony exports\n__webpack_require__.d = (exports, definition) => {\n\tfor(var key in definition) {\n\t\tif(__webpack_require__.o(definition, key) && !__webpack_require__.o(exports, key)) {\n\t\t\tObject.defineProperty(exports, key, { enumerable: true, get: definition[key] });\n\t\t}\n\t}\n};",
         "__webpack_require__.f = {};\n// This file contains only the entry chunk.\n// The chunk loading function for additional chunks\n__webpack_require__.e = (chunkId) => {\n\treturn Promise.all(Object.keys(__webpack_require__.f).reduce((promises, key) => {\n\t\t__webpack_require__.f[key](chunkId, promises);\n\t\treturn promises;\n\t}, []));\n};",
-        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"31\":\"418331b4a22dffe518b4\",\"109\":\"624848fd57458c5dd4f0\",\"153\":\"6a8fe9147a69d0d5e1ff\",\"157\":\"921bbfb16083689ff62a\",\"168\":\"8383bc2d0a83f2b959fd\",\"173\":\"df5a30c1440df850aa82\",\"210\":\"35c06ed0583039490182\",\"215\":\"82ec42ef5a24d2ff187f\",\"216\":\"011d737685936c4c8e1a\",\"232\":\"d5cb8a2dcc0d34fabd8a\",\"268\":\"4eaefedf266ea50fd6df\",\"326\":\"f8d1ef211f999b0b3dca\",\"382\":\"0016faf875cb665ac9b2\",\"410\":\"941cb48faa5e2d568b13\",\"428\":\"cb1cafd5e6ba8a81b05a\",\"513\":\"5646d474a0e4d9613886\",\"533\":\"606434cc067b99350123\",\"549\":\"dbfa5147d8fec7e5a76f\",\"588\":\"3e52218ff8bfd1512578\",\"593\":\"526fcc348e87fac11681\",\"617\":\"c198d75d062c9be68fef\",\"619\":\"84aef6ceee0a82ac27ee\",\"627\":\"5da93440391d7167f88d\",\"643\":\"34f4f43b70e246a962a8\",\"647\":\"d729bd3d64d38278f913\",\"655\":\"13bd86e04776bccddcee\",\"671\":\"5cc50d235d821a731440\",\"693\":\"91ee036f7a5bf0e5a1b0\",\"698\":\"48373f0b62bef71acebe\",\"704\":\"cf482c52df64c1afcb10\",\"835\":\"cbd12870eccd44d69cf0\",\"839\":\"c46366b4bade6ade8403\",\"929\":\"d864f042fdaf411ba52b\",\"939\":\"973bc21fa6263dbabd09\",\"974\":\"5f4a862a240a7368a2b5\"}[chunkId] + \".js?v=\" + {\"31\":\"418331b4a22dffe518b4\",\"109\":\"624848fd57458c5dd4f0\",\"153\":\"6a8fe9147a69d0d5e1ff\",\"157\":\"921bbfb16083689ff62a\",\"168\":\"8383bc2d0a83f2b959fd\",\"173\":\"df5a30c1440df850aa82\",\"210\":\"35c06ed0583039490182\",\"215\":\"82ec42ef5a24d2ff187f\",\"216\":\"011d737685936c4c8e1a\",\"232\":\"d5cb8a2dcc0d34fabd8a\",\"268\":\"4eaefedf266ea50fd6df\",\"326\":\"f8d1ef211f999b0b3dca\",\"382\":\"0016faf875cb665ac9b2\",\"410\":\"941cb48faa5e2d568b13\",\"428\":\"cb1cafd5e6ba8a81b05a\",\"513\":\"5646d474a0e4d9613886\",\"533\":\"606434cc067b99350123\",\"549\":\"dbfa5147d8fec7e5a76f\",\"588\":\"3e52218ff8bfd1512578\",\"593\":\"526fcc348e87fac11681\",\"617\":\"c198d75d062c9be68fef\",\"619\":\"84aef6ceee0a82ac27ee\",\"627\":\"5da93440391d7167f88d\",\"643\":\"34f4f43b70e246a962a8\",\"647\":\"d729bd3d64d38278f913\",\"655\":\"13bd86e04776bccddcee\",\"671\":\"5cc50d235d821a731440\",\"693\":\"91ee036f7a5bf0e5a1b0\",\"698\":\"48373f0b62bef71acebe\",\"704\":\"cf482c52df64c1afcb10\",\"835\":\"cbd12870eccd44d69cf0\",\"839\":\"c46366b4bade6ade8403\",\"929\":\"d864f042fdaf411ba52b\",\"939\":\"973bc21fa6263dbabd09\",\"974\":\"5f4a862a240a7368a2b5\"}[chunkId] + \"\";\n};",
+        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"31\":\"418331b4a22dffe518b4\",\"109\":\"624848fd57458c5dd4f0\",\"157\":\"921bbfb16083689ff62a\",\"168\":\"8383bc2d0a83f2b959fd\",\"173\":\"df5a30c1440df850aa82\",\"210\":\"35c06ed0583039490182\",\"215\":\"82ec42ef5a24d2ff187f\",\"216\":\"751d5114e75a3795211f\",\"232\":\"d5cb8a2dcc0d34fabd8a\",\"268\":\"4eaefedf266ea50fd6df\",\"326\":\"f8d1ef211f999b0b3dca\",\"382\":\"0016faf875cb665ac9b2\",\"410\":\"941cb48faa5e2d568b13\",\"428\":\"cb1cafd5e6ba8a81b05a\",\"513\":\"5646d474a0e4d9613886\",\"533\":\"606434cc067b99350123\",\"549\":\"dbfa5147d8fec7e5a76f\",\"588\":\"3e52218ff8bfd1512578\",\"593\":\"526fcc348e87fac11681\",\"617\":\"c198d75d062c9be68fef\",\"619\":\"84aef6ceee0a82ac27ee\",\"627\":\"5da93440391d7167f88d\",\"643\":\"34f4f43b70e246a962a8\",\"647\":\"d729bd3d64d38278f913\",\"655\":\"13bd86e04776bccddcee\",\"671\":\"5cc50d235d821a731440\",\"693\":\"91ee036f7a5bf0e5a1b0\",\"698\":\"48373f0b62bef71acebe\",\"704\":\"cf482c52df64c1afcb10\",\"835\":\"6f7e7b701fee67a1ec53\",\"839\":\"c46366b4bade6ade8403\",\"929\":\"d864f042fdaf411ba52b\",\"939\":\"973bc21fa6263dbabd09\",\"955\":\"324ee5220abd1dc68556\",\"974\":\"5f4a862a240a7368a2b5\"}[chunkId] + \".js?v=\" + {\"31\":\"418331b4a22dffe518b4\",\"109\":\"624848fd57458c5dd4f0\",\"157\":\"921bbfb16083689ff62a\",\"168\":\"8383bc2d0a83f2b959fd\",\"173\":\"df5a30c1440df850aa82\",\"210\":\"35c06ed0583039490182\",\"215\":\"82ec42ef5a24d2ff187f\",\"216\":\"751d5114e75a3795211f\",\"232\":\"d5cb8a2dcc0d34fabd8a\",\"268\":\"4eaefedf266ea50fd6df\",\"326\":\"f8d1ef211f999b0b3dca\",\"382\":\"0016faf875cb665ac9b2\",\"410\":\"941cb48faa5e2d568b13\",\"428\":\"cb1cafd5e6ba8a81b05a\",\"513\":\"5646d474a0e4d9613886\",\"533\":\"606434cc067b99350123\",\"549\":\"dbfa5147d8fec7e5a76f\",\"588\":\"3e52218ff8bfd1512578\",\"593\":\"526fcc348e87fac11681\",\"617\":\"c198d75d062c9be68fef\",\"619\":\"84aef6ceee0a82ac27ee\",\"627\":\"5da93440391d7167f88d\",\"643\":\"34f4f43b70e246a962a8\",\"647\":\"d729bd3d64d38278f913\",\"655\":\"13bd86e04776bccddcee\",\"671\":\"5cc50d235d821a731440\",\"693\":\"91ee036f7a5bf0e5a1b0\",\"698\":\"48373f0b62bef71acebe\",\"704\":\"cf482c52df64c1afcb10\",\"835\":\"6f7e7b701fee67a1ec53\",\"839\":\"c46366b4bade6ade8403\",\"929\":\"d864f042fdaf411ba52b\",\"939\":\"973bc21fa6263dbabd09\",\"955\":\"324ee5220abd1dc68556\",\"974\":\"5f4a862a240a7368a2b5\"}[chunkId] + \"\";\n};",
         "__webpack_require__.g = (function() {\n\tif (typeof globalThis === 'object') return globalThis;\n\ttry {\n\t\treturn this || new Function('return this')();\n\t} catch (e) {\n\t\tif (typeof window === 'object') return window;\n\t}\n})();",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
         "// define __esModule on exports\n__webpack_require__.r = (exports) => {\n\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n\t}\n\tObject.defineProperty(exports, '__esModule', { value: true });\n};",
-        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => (typeof console !== \"undefined\" && console.warn && console.warn(msg));\n\tvar uniqueName = \"jupyterlab-blockly-extension\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"blockly\", \"9.2.1\", () => (Promise.all([__webpack_require__.e(215), __webpack_require__.e(593)]).then(() => (() => (__webpack_require__(593))))));\n\t\t\tregister(\"jupyterlab-blockly-extension\", \"0.3.0-alpha.0\", () => (Promise.all([__webpack_require__.e(153), __webpack_require__.e(216)]).then(() => (() => (__webpack_require__(4216))))));\n\t\t\tregister(\"jupyterlab-blockly\", \"0.3.0-alpha.0\", () => (Promise.all([__webpack_require__.e(215), __webpack_require__.e(839), __webpack_require__.e(835), __webpack_require__.e(153)]).then(() => (() => (__webpack_require__(2835))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
+        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => (typeof console !== \"undefined\" && console.warn && console.warn(msg));\n\tvar uniqueName = \"jupyterlab-blockly-extension\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"blockly\", \"9.2.1\", () => (Promise.all([__webpack_require__.e(215), __webpack_require__.e(593)]).then(() => (() => (__webpack_require__(593))))));\n\t\t\tregister(\"jupyterlab-blockly-extension\", \"0.3.0-alpha.1\", () => (Promise.all([__webpack_require__.e(955), __webpack_require__.e(216)]).then(() => (() => (__webpack_require__(4216))))));\n\t\t\tregister(\"jupyterlab-blockly\", \"0.3.0-alpha.1\", () => (Promise.all([__webpack_require__.e(215), __webpack_require__.e(839), __webpack_require__.e(835), __webpack_require__.e(955)]).then(() => (() => (__webpack_require__(2835))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
         "var scriptUrl;\nif (__webpack_require__.g.importScripts) scriptUrl = __webpack_require__.g.location + \"\";\nvar document = __webpack_require__.g.document;\nif (!scriptUrl && document) {\n\tif (document.currentScript)\n\t\tscriptUrl = document.currentScript.src\n\tif (!scriptUrl) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tif(scripts.length) scriptUrl = scripts[scripts.length - 1].src\n\t}\n}\n// When supporting browsers where an automatic publicPath is not supported you must specify an output.publicPath manually via configuration\n// or pass an empty string (\"\") and set the __webpack_public_path__ variable from your code to use your own logic.\nif (!scriptUrl) throw new Error(\"Automatic publicPath is not supported in this browser\");\nscriptUrl = scriptUrl.replace(/#.*$/, \"\").replace(/\\?.*$/, \"\").replace(/\\/[^\\/]+$/, \"/\");\n__webpack_require__.p = scriptUrl;",
-        "// no baseURI\n\n// object to store loaded and loading chunks\n// undefined = chunk not loaded, null = chunk preloaded/prefetched\n// [resolve, reject, Promise] = chunk loading, 0 = chunk loaded\nvar installedChunks = {\n\t380: 0\n};\n\n__webpack_require__.f.j = (chunkId, promises) => {\n\t\t// JSONP chunk loading for javascript\n\t\tvar installedChunkData = __webpack_require__.o(installedChunks, chunkId) ? installedChunks[chunkId] : undefined;\n\t\tif(installedChunkData !== 0) { // 0 means \"already installed\".\n\n\t\t\t// a Promise means \"currently loading\".\n\t\t\tif(installedChunkData) {\n\t\t\t\tpromises.push(installedChunkData[2]);\n\t\t\t} else {\n\t\t\t\tif(153 != chunkId) {\n\t\t\t\t\t// setup Promise in chunk cache\n\t\t\t\t\tvar promise = new Promise((resolve, reject) => (installedChunkData = installedChunks[chunkId] = [resolve, reject]));\n\t\t\t\t\tpromises.push(installedChunkData[2] = promise);\n\n\t\t\t\t\t// start chunk loading\n\t\t\t\t\tvar url = __webpack_require__.p + __webpack_require__.u(chunkId);\n\t\t\t\t\t// create error before stack unwound to get useful stacktrace later\n\t\t\t\t\tvar error = new Error();\n\t\t\t\t\tvar loadingEnded = (event) => {\n\t\t\t\t\t\tif(__webpack_require__.o(installedChunks, chunkId)) {\n\t\t\t\t\t\t\tinstalledChunkData = installedChunks[chunkId];\n\t\t\t\t\t\t\tif(installedChunkData !== 0) installedChunks[chunkId] = undefined;\n\t\t\t\t\t\t\tif(installedChunkData) {\n\t\t\t\t\t\t\t\tvar errorType = event && (event.type === 'load' ? 'missing' : event.type);\n\t\t\t\t\t\t\t\tvar realSrc = event && event.target && event.target.src;\n\t\t\t\t\t\t\t\terror.message = 'Loading chunk ' + chunkId + ' failed.\\n(' + errorType + ': ' + realSrc + ')';\n\t\t\t\t\t\t\t\terror.name = 'ChunkLoadError';\n\t\t\t\t\t\t\t\terror.type = errorType;\n\t\t\t\t\t\t\t\terror.request = realSrc;\n\t\t\t\t\t\t\t\tinstalledChunkData[1](error);\n\t\t\t\t\t\t\t}\n\t\t\t\t\t\t}\n\t\t\t\t\t};\n\t\t\t\t\t__webpack_require__.l(url, loadingEnded, \"chunk-\" + chunkId, chunkId);\n\t\t\t\t} else installedChunks[chunkId] = 0;\n\t\t\t}\n\t\t}\n};\n\n// no prefetching\n\n// no preloaded\n\n// no HMR\n\n// no HMR manifest\n\n// no on chunks loaded\n\n// install a JSONP callback for chunk loading\nvar webpackJsonpCallback = (parentChunkLoadingFunction, data) => {\n\tvar [chunkIds, moreModules, runtime] = data;\n\t// add \"moreModules\" to the modules object,\n\t// then flag all \"chunkIds\" as loaded and fire callback\n\tvar moduleId, chunkId, i = 0;\n\tif(chunkIds.some((id) => (installedChunks[id] !== 0))) {\n\t\tfor(moduleId in moreModules) {\n\t\t\tif(__webpack_require__.o(moreModules, moduleId)) {\n\t\t\t\t__webpack_require__.m[moduleId] = moreModules[moduleId];\n\t\t\t}\n\t\t}\n\t\tif(runtime) var result = runtime(__webpack_require__);\n\t}\n\tif(parentChunkLoadingFunction) parentChunkLoadingFunction(data);\n\tfor(;i < chunkIds.length; i++) {\n\t\tchunkId = chunkIds[i];\n\t\tif(__webpack_require__.o(installedChunks, chunkId) && installedChunks[chunkId]) {\n\t\t\tinstalledChunks[chunkId][0]();\n\t\t}\n\t\tinstalledChunks[chunkId] = 0;\n\t}\n\n}\n\nvar chunkLoadingGlobal = self[\"webpackChunkjupyterlab_blockly_extension\"] = self[\"webpackChunkjupyterlab_blockly_extension\"] || [];\nchunkLoadingGlobal.forEach(webpackJsonpCallback.bind(null, 0));\nchunkLoadingGlobal.push = webpackJsonpCallback.bind(null, chunkLoadingGlobal.push.bind(chunkLoadingGlobal));",
+        "// no baseURI\n\n// object to store loaded and loading chunks\n// undefined = chunk not loaded, null = chunk preloaded/prefetched\n// [resolve, reject, Promise] = chunk loading, 0 = chunk loaded\nvar installedChunks = {\n\t380: 0\n};\n\n__webpack_require__.f.j = (chunkId, promises) => {\n\t\t// JSONP chunk loading for javascript\n\t\tvar installedChunkData = __webpack_require__.o(installedChunks, chunkId) ? installedChunks[chunkId] : undefined;\n\t\tif(installedChunkData !== 0) { // 0 means \"already installed\".\n\n\t\t\t// a Promise means \"currently loading\".\n\t\t\tif(installedChunkData) {\n\t\t\t\tpromises.push(installedChunkData[2]);\n\t\t\t} else {\n\t\t\t\tif(955 != chunkId) {\n\t\t\t\t\t// setup Promise in chunk cache\n\t\t\t\t\tvar promise = new Promise((resolve, reject) => (installedChunkData = installedChunks[chunkId] = [resolve, reject]));\n\t\t\t\t\tpromises.push(installedChunkData[2] = promise);\n\n\t\t\t\t\t// start chunk loading\n\t\t\t\t\tvar url = __webpack_require__.p + __webpack_require__.u(chunkId);\n\t\t\t\t\t// create error before stack unwound to get useful stacktrace later\n\t\t\t\t\tvar error = new Error();\n\t\t\t\t\tvar loadingEnded = (event) => {\n\t\t\t\t\t\tif(__webpack_require__.o(installedChunks, chunkId)) {\n\t\t\t\t\t\t\tinstalledChunkData = installedChunks[chunkId];\n\t\t\t\t\t\t\tif(installedChunkData !== 0) installedChunks[chunkId] = undefined;\n\t\t\t\t\t\t\tif(installedChunkData) {\n\t\t\t\t\t\t\t\tvar errorType = event && (event.type === 'load' ? 'missing' : event.type);\n\t\t\t\t\t\t\t\tvar realSrc = event && event.target && event.target.src;\n\t\t\t\t\t\t\t\terror.message = 'Loading chunk ' + chunkId + ' failed.\\n(' + errorType + ': ' + realSrc + ')';\n\t\t\t\t\t\t\t\terror.name = 'ChunkLoadError';\n\t\t\t\t\t\t\t\terror.type = errorType;\n\t\t\t\t\t\t\t\terror.request = realSrc;\n\t\t\t\t\t\t\t\tinstalledChunkData[1](error);\n\t\t\t\t\t\t\t}\n\t\t\t\t\t\t}\n\t\t\t\t\t};\n\t\t\t\t\t__webpack_require__.l(url, loadingEnded, \"chunk-\" + chunkId, chunkId);\n\t\t\t\t} else installedChunks[chunkId] = 0;\n\t\t\t}\n\t\t}\n};\n\n// no prefetching\n\n// no preloaded\n\n// no HMR\n\n// no HMR manifest\n\n// no on chunks loaded\n\n// install a JSONP callback for chunk loading\nvar webpackJsonpCallback = (parentChunkLoadingFunction, data) => {\n\tvar [chunkIds, moreModules, runtime] = data;\n\t// add \"moreModules\" to the modules object,\n\t// then flag all \"chunkIds\" as loaded and fire callback\n\tvar moduleId, chunkId, i = 0;\n\tif(chunkIds.some((id) => (installedChunks[id] !== 0))) {\n\t\tfor(moduleId in moreModules) {\n\t\t\tif(__webpack_require__.o(moreModules, moduleId)) {\n\t\t\t\t__webpack_require__.m[moduleId] = moreModules[moduleId];\n\t\t\t}\n\t\t}\n\t\tif(runtime) var result = runtime(__webpack_require__);\n\t}\n\tif(parentChunkLoadingFunction) parentChunkLoadingFunction(data);\n\tfor(;i < chunkIds.length; i++) {\n\t\tchunkId = chunkIds[i];\n\t\tif(__webpack_require__.o(installedChunks, chunkId) && installedChunks[chunkId]) {\n\t\t\tinstalledChunks[chunkId][0]();\n\t\t}\n\t\tinstalledChunks[chunkId] = 0;\n\t}\n\n}\n\nvar chunkLoadingGlobal = self[\"webpackChunkjupyterlab_blockly_extension\"] = self[\"webpackChunkjupyterlab_blockly_extension\"] || [];\nchunkLoadingGlobal.forEach(webpackJsonpCallback.bind(null, 0));\nchunkLoadingGlobal.push = webpackJsonpCallback.bind(null, chunkLoadingGlobal.push.bind(chunkLoadingGlobal));",
         "__webpack_require__.nc = undefined;",
         "// module cache are used so entry inlining is disabled\n// startup\n// Load entry module and return exports\nvar __webpack_exports__ = __webpack_require__(1707);\n"
     ],
     "version": 3
 }
```

### Comparing `jupyterlab_blockly-0.3.0a0/jupyterlab_blockly/labextension/static/third-party-licenses.json` & `jupyterlab_blockly-0.3.0a1/jupyterlab_blockly/labextension/static/third-party-licenses.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.984375%*

 * *Differences: {"'packages'": "{2: {'versionInfo': '0.3.0-alpha.1'}}"}*

```diff
@@ -12,15 +12,15 @@
             "name": "css-loader",
             "versionInfo": "5.2.7"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "jupyterlab-blockly",
-            "versionInfo": "0.3.0-alpha.0"
+            "versionInfo": "0.3.0-alpha.1"
         },
         {
             "extractedText": "Copyright JS Foundation and other contributors\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n'Software'), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY\nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,\nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE\nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "style-loader",
             "versionInfo": "2.0.0"
         }
```

### Comparing `jupyterlab_blockly-0.3.0a0/patches/@jupyterlab+codeeditor+3.6.1.patch` & `jupyterlab_blockly-0.3.0a1/patches/@jupyterlab+codeeditor+3.6.3.patch`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/scripts/bump-version.py` & `jupyterlab_blockly-0.3.0a1/scripts/bump-version.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/package.json` & `jupyterlab_blockly-0.3.0a1/packages/blockly/package.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9736842105263158%*

 * *Differences: {"'version'": "'0.3.0-alpha.1'"}*

```diff
@@ -61,9 +61,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.3.0-alpha.0"
+    "version": "0.3.0-alpha.1"
 }
```

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/brace-expansion/LICENSE` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/brace-expansion/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/brace-expansion/README.md` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/brace-expansion/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/brace-expansion/index.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/brace-expansion/index.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/brace-expansion/package.json` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/brace-expansion/package.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/LICENSE` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/README.md` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/package.json` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/package.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/cjs/glob.d.ts` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/cjs/glob.d.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/cjs/glob.d.ts.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/cjs/glob.d.ts.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/cjs/glob.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/cjs/glob.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/cjs/glob.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/cjs/glob.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/cjs/has-magic.d.ts` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/cjs/has-magic.d.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/cjs/has-magic.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/cjs/has-magic.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/cjs/ignore.d.ts` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/cjs/ignore.d.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/cjs/ignore.d.ts.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/cjs/ignore.d.ts.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/cjs/ignore.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/cjs/ignore.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/cjs/ignore.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/cjs/ignore.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/cjs/index-cjs.d.ts` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/cjs/index-cjs.d.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/cjs/index.d.ts` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/cjs/index.d.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/cjs/index.d.ts.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/cjs/index.d.ts.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/cjs/index.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/cjs/index.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/cjs/index.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/cjs/index.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/cjs/pattern.d.ts` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/cjs/pattern.d.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/cjs/pattern.d.ts.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/cjs/pattern.d.ts.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/cjs/pattern.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/cjs/pattern.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/cjs/pattern.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/cjs/pattern.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/cjs/processor.d.ts` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/cjs/processor.d.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/cjs/processor.d.ts.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/cjs/processor.d.ts.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/cjs/processor.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/cjs/processor.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/cjs/processor.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/cjs/processor.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/cjs/walker.d.ts` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/cjs/walker.d.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/cjs/walker.d.ts.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/cjs/walker.d.ts.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/cjs/walker.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/cjs/walker.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/cjs/walker.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/cjs/walker.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/mjs/glob.d.ts` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/mjs/glob.d.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/mjs/glob.d.ts.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/mjs/glob.d.ts.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/mjs/glob.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/mjs/glob.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/mjs/glob.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/mjs/glob.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/mjs/has-magic.d.ts` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/mjs/has-magic.d.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/mjs/has-magic.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/mjs/has-magic.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/mjs/ignore.d.ts` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/mjs/ignore.d.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/mjs/ignore.d.ts.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/mjs/ignore.d.ts.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/mjs/ignore.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/mjs/ignore.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/mjs/ignore.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/mjs/ignore.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/mjs/index.d.ts` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/mjs/index.d.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/mjs/index.d.ts.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/mjs/index.d.ts.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/mjs/index.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/mjs/index.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/mjs/index.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/mjs/index.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/mjs/pattern.d.ts` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/mjs/pattern.d.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/mjs/pattern.d.ts.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/mjs/pattern.d.ts.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/mjs/pattern.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/mjs/pattern.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/mjs/pattern.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/mjs/pattern.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/mjs/processor.d.ts` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/mjs/processor.d.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/mjs/processor.d.ts.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/mjs/processor.d.ts.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/mjs/processor.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/mjs/processor.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/mjs/processor.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/mjs/processor.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/mjs/walker.d.ts` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/mjs/walker.d.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/mjs/walker.d.ts.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/mjs/walker.d.ts.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/mjs/walker.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/mjs/walker.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/glob/dist/mjs/walker.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/glob/dist/mjs/walker.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minimatch/LICENSE` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minimatch/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minimatch/README.md` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minimatch/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minimatch/package.json` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minimatch/package.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minimatch/dist/cjs/brace-expressions.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minimatch/dist/cjs/brace-expressions.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minimatch/dist/cjs/brace-expressions.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minimatch/dist/cjs/brace-expressions.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minimatch/dist/cjs/escape.d.ts` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minimatch/dist/cjs/escape.d.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minimatch/dist/cjs/escape.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minimatch/dist/cjs/escape.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minimatch/dist/cjs/index-cjs.d.ts` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minimatch/dist/cjs/index-cjs.d.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minimatch/dist/cjs/index.d.ts` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minimatch/dist/cjs/index.d.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minimatch/dist/cjs/index.d.ts.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minimatch/dist/cjs/index.d.ts.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minimatch/dist/cjs/index.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minimatch/dist/cjs/index.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minimatch/dist/cjs/index.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minimatch/dist/cjs/index.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minimatch/dist/cjs/unescape.d.ts` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minimatch/dist/cjs/unescape.d.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minimatch/dist/cjs/unescape.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minimatch/dist/cjs/unescape.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minimatch/dist/mjs/brace-expressions.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minimatch/dist/mjs/brace-expressions.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minimatch/dist/mjs/brace-expressions.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minimatch/dist/mjs/brace-expressions.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minimatch/dist/mjs/escape.d.ts` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minimatch/dist/mjs/escape.d.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minimatch/dist/mjs/escape.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minimatch/dist/mjs/escape.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minimatch/dist/mjs/index.d.ts` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minimatch/dist/mjs/index.d.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minimatch/dist/mjs/index.d.ts.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minimatch/dist/mjs/index.d.ts.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minimatch/dist/mjs/index.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minimatch/dist/mjs/index.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minimatch/dist/mjs/index.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minimatch/dist/mjs/index.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minimatch/dist/mjs/unescape.d.ts` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minimatch/dist/mjs/unescape.d.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minimatch/dist/mjs/unescape.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minimatch/dist/mjs/unescape.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minipass/LICENSE` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minipass/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minipass/README.md` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minipass/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minipass/index.d.ts` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minipass/index.d.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minipass/index.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minipass/index.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minipass/index.mjs` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minipass/index.mjs`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/minipass/package.json` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/minipass/package.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/LICENSE` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/README.md` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/package.json` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/package.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/package.json` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/package.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/bin.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/bin.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/bin.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/bin.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/default-tmp.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/default-tmp.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/default-tmp.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/default-tmp.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/fix-eperm.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/fix-eperm.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/fix-eperm.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/fix-eperm.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/fs.d.ts` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/fs.d.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/fs.d.ts.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/fs.d.ts.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/fs.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/fs.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/fs.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/fs.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/ignore-enoent.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/ignore-enoent.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/ignore-enoent.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/ignore-enoent.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/index-cjs.d.ts` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/index-cjs.d.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/index.d.ts` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/index.d.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/index.d.ts.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/index.d.ts.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/index.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/index.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/index.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/index.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/opt-arg.d.ts` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/opt-arg.d.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/opt-arg.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/opt-arg.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/opt-arg.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/opt-arg.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/path-arg.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/path-arg.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/path-arg.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/path-arg.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/readdir-or-error.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/readdir-or-error.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/readdir-or-error.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/readdir-or-error.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/retry-busy.d.ts` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/retry-busy.d.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/retry-busy.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/retry-busy.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/retry-busy.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/retry-busy.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/rimraf-manual.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/rimraf-manual.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/rimraf-move-remove.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/rimraf-move-remove.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/rimraf-move-remove.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/rimraf-move-remove.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/rimraf-native.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/rimraf-native.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/rimraf-native.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/rimraf-native.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/rimraf-posix.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/rimraf-posix.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/rimraf-posix.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/rimraf-posix.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/rimraf-windows.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/rimraf-windows.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/rimraf-windows.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/rimraf-windows.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/use-native.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/use-native.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/cjs/src/use-native.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/cjs/src/use-native.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/default-tmp.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/default-tmp.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/default-tmp.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/default-tmp.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/fix-eperm.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/fix-eperm.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/fix-eperm.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/fix-eperm.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/fs.d.ts` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/fs.d.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/fs.d.ts.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/fs.d.ts.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/fs.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/fs.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/fs.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/fs.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/index.d.ts` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/index.d.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/index.d.ts.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/index.d.ts.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/index.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/index.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/index.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/index.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/opt-arg.d.ts` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/opt-arg.d.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/opt-arg.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/opt-arg.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/opt-arg.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/opt-arg.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/path-arg.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/path-arg.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/path-arg.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/path-arg.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/readdir-or-error.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/readdir-or-error.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/retry-busy.d.ts` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/retry-busy.d.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/retry-busy.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/retry-busy.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/retry-busy.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/retry-busy.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/rimraf-move-remove.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/rimraf-move-remove.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/rimraf-move-remove.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/rimraf-move-remove.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/rimraf-native.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/rimraf-native.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/rimraf-posix.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/rimraf-posix.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/rimraf-posix.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/rimraf-posix.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/rimraf-windows.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/rimraf-windows.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/rimraf-windows.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/rimraf-windows.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/use-native.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/use-native.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/node_modules/rimraf/dist/mjs/use-native.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly/node_modules/rimraf/dist/mjs/use-native.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/src/factory.ts` & `jupyterlab_blockly-0.3.0a1/packages/blockly/src/factory.ts`

 * *Files 19% similar despite different names*

```diff
@@ -42,14 +42,17 @@
    *
    * @param context Contains the information of the file
    * @returns The widget
    */
   protected createNewWidget(
     context: DocumentRegistry.IContext<DocumentModel>
   ): BlocklyEditor {
+    // Set a map to the model. The widgets manager expects a Notebook model
+    // but the only notebook property it uses is the metadata.
+    context.model['metadata'] = new Map();
     const manager = new BlocklyManager(
       this._registry,
       context.sessionContext,
       this._mimetypeService
     );
     const content = new BlocklyPanel(context, manager, this._rendermime);
     return new BlocklyEditor({ context, content, manager });
```

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/src/layout.ts` & `jupyterlab_blockly-0.3.0a1/packages/blockly/src/layout.ts`

 * *Files 2% similar despite different names*

```diff
@@ -53,20 +53,33 @@
     // adding the style to the element as a quick fix
     // we should make it work with the css class
     this._cell.node.style.overflow = 'scroll';
 
     this._manager.changed.connect(this._onManagerChanged, this);
   }
 
+  /*
+   * The code cell.
+   */
+  get cell(): CodeCell {
+    return this._cell;
+  }
+
+  /*
+   * The current workspace.
+   */
   get workspace(): Blockly.Workspace {
     // eslint-disable-next-line @typescript-eslint/ban-ts-comment
     // @ts-ignore
     return Blockly.serialization.workspaces.save(this._workspace);
   }
 
+  /*
+   * Set a new workspace.
+   */
   set workspace(workspace: Blockly.Workspace) {
     const data = workspace === null ? { variables: [] } : workspace;
     // eslint-disable-next-line @typescript-eslint/ban-ts-comment
     // @ts-ignore
     Blockly.serialization.workspaces.load(data, this._workspace);
   }
 
@@ -134,20 +147,24 @@
         finalToplevelInit = finalToplevelInit + string;
       }
     }
     // console.log(finalToplevelInit);
     return finalToplevelInit;
   }
 
+  /*
+   * Generates and runs the code from the current workspace.
+   */
   run(): void {
     // Get extra code from the blocks in the workspace.
     const extra_init = this.getBlocksToplevelInit();
     // Serializing our workspace into the chosen language generator.
     const code =
       extra_init + this._manager.generator.workspaceToCode(this._workspace);
+    //const code = "import ipywidgets as widgets\nwidgets.IntSlider()";
     this._cell.model.sharedModel.setSource(code);
 
     // Execute the code using the kernel, by using a static method from the
     // same class to make an execution request.
     if (this._sessionContext.hasNoKernel) {
       // Check whether there is a kernel
       showErrorMessage(
```

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/src/manager.ts` & `jupyterlab_blockly-0.3.0a1/packages/blockly/src/manager.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/src/registry.ts` & `jupyterlab_blockly-0.3.0a1/packages/blockly/src/registry.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/src/token.ts` & `jupyterlab_blockly-0.3.0a1/packages/blockly/src/token.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/src/utils.ts` & `jupyterlab_blockly-0.3.0a1/packages/blockly/src/utils.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/src/widget.ts` & `jupyterlab_blockly-0.3.0a1/packages/blockly/src/widget.ts`

 * *Files 8% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import { BlocklyManager } from './manager';
 import {
   BlocklyButton,
   SelectGenerator,
   SelectToolbox,
   Spacer
 } from './toolbar';
+import { CodeCell } from '@jupyterlab/cells';
 
 /**
  * DocumentWidget: widget that represents the view or editor for a file type.
  */
 export class BlocklyEditor extends DocumentWidget<BlocklyPanel, DocumentModel> {
   constructor(options: BlocklyEditor.IOptions) {
     super(options);
@@ -76,14 +77,15 @@
 }
 
 /**
  * Widget that contains the main view of the DocumentWidget.
  */
 export class BlocklyPanel extends SplitPanel {
   private _context: DocumentRegistry.IContext<DocumentModel>;
+  private _rendermime: IRenderMimeRegistry;
 
   /**
    * Construct a `BlocklyPanel`.
    *
    * @param context - The documents context.
    */
   constructor(
@@ -92,21 +94,36 @@
     rendermime: IRenderMimeRegistry
   ) {
     super({
       layout: new BlocklyLayout(manager, context.sessionContext, rendermime)
     });
     this.addClass('jp-BlocklyPanel');
     this._context = context;
+    this._rendermime = rendermime;
 
     // Load the content of the file when the context is ready
     this._context.ready.then(() => this._load());
     // Connect to the save signal
     this._context.saveState.connect(this._onSave, this);
   }
 
+  /*
+   * The code cell.
+   */
+  get cell(): CodeCell {
+    return (this.layout as BlocklyLayout).cell;
+  }
+
+  /*
+   * The rendermime instance used in the code cell.
+   */
+  get rendermime(): IRenderMimeRegistry {
+    return this._rendermime;
+  }
+
   /**
    * Dispose of the resources held by the widget.
    */
   dispose(): void {
     if (this.isDisposed) {
       return;
     }
```

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/src/toolbar/generator.tsx` & `jupyterlab_blockly-0.3.0a1/packages/blockly/src/toolbar/generator.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly/src/toolbar/toolbox.tsx` & `jupyterlab_blockly-0.3.0a1/packages/blockly/src/toolbar/toolbox.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/package.json` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/package.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9671875%*

 * *Differences: {"'dependencies'": "{'jupyterlab-blockly': '^0.3.0-alpha.1', '@jupyter-widgets/base': '^6.0.4', "*

 * *                   "'@jupyter-widgets/jupyterlab-manager': '^5.0.7', '@jupyterlab/cells': '^3.6'}",*

 * * "'jupyterlab'": "{'sharedPackages': {'@jupyter-widgets/base': OrderedDict([('bundled', False), "*

 * *                 "('singleton', True)]), '@jupyter-widgets/jupyterlab-manager': "*

 * *                 "OrderedDict([('bundled', False), ('singleton', True)])}}",*

 * * "'version'": "'0.3.0-alpha.1'"}*

```diff
@@ -3,25 +3,28 @@
         "email": "",
         "name": "quantstack"
     },
     "bugs": {
         "url": "https://github.com/quantstack/jupyterlab-blockly/issues"
     },
     "dependencies": {
+        "@jupyter-widgets/base": "^6.0.4",
+        "@jupyter-widgets/jupyterlab-manager": "^5.0.7",
         "@jupyterlab/application": "^3.6",
         "@jupyterlab/apputils": "^3.6",
+        "@jupyterlab/cells": "^3.6",
         "@jupyterlab/codeeditor": "^3.6",
         "@jupyterlab/filebrowser": "^3.6",
         "@jupyterlab/launcher": "^3.6",
         "@jupyterlab/mainmenu": "^3.6",
         "@jupyterlab/rendermime": "^3.6",
         "@jupyterlab/settingregistry": "^3.6",
         "@jupyterlab/translation": "^3.6",
         "@jupyterlab/ui-components": "^3.6",
-        "jupyterlab-blockly": "^0.3.0-alpha.0"
+        "jupyterlab-blockly": "^0.3.0-alpha.1"
     },
     "description": "Blockly extension for JupyterLab.",
     "devDependencies": {
         "@jupyterlab/builder": "^3.6",
         "npm-run-all": "^4.1.5",
         "rimraf": "^4.4.0",
         "source-map-loader": "^4.0.1",
@@ -32,14 +35,22 @@
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/quantstack/jupyterlab-blockly",
     "jupyterlab": {
         "extension": true,
         "outputDir": "../../jupyterlab_blockly/labextension",
         "sharedPackages": {
+            "@jupyter-widgets/base": {
+                "bundled": false,
+                "singleton": true
+            },
+            "@jupyter-widgets/jupyterlab-manager": {
+                "bundled": false,
+                "singleton": true
+            },
             "blockly": {
                 "bundled": true,
                 "singleton": true
             },
             "jupyterlab-blockly": {
                 "bundled": true,
                 "singleton": true
@@ -80,9 +91,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.3.0-alpha.0"
+    "version": "0.3.0-alpha.1"
 }
```

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/brace-expansion/LICENSE` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/brace-expansion/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/brace-expansion/README.md` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/brace-expansion/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/brace-expansion/index.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/brace-expansion/index.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/brace-expansion/package.json` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/brace-expansion/package.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/LICENSE` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/README.md` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/package.json` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/package.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/cjs/glob.d.ts` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/cjs/glob.d.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/cjs/glob.d.ts.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/cjs/glob.d.ts.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/cjs/glob.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/cjs/glob.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/cjs/glob.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/cjs/glob.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/cjs/has-magic.d.ts` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/cjs/has-magic.d.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/cjs/has-magic.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/cjs/has-magic.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/cjs/ignore.d.ts` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/cjs/ignore.d.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/cjs/ignore.d.ts.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/cjs/ignore.d.ts.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/cjs/ignore.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/cjs/ignore.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/cjs/ignore.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/cjs/ignore.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/cjs/index-cjs.d.ts` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/cjs/index-cjs.d.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/cjs/index.d.ts` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/cjs/index.d.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/cjs/index.d.ts.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/cjs/index.d.ts.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/cjs/index.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/cjs/index.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/cjs/index.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/cjs/index.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/cjs/pattern.d.ts` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/cjs/pattern.d.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/cjs/pattern.d.ts.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/cjs/pattern.d.ts.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/cjs/pattern.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/cjs/pattern.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/cjs/pattern.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/cjs/pattern.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/cjs/processor.d.ts` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/cjs/processor.d.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/cjs/processor.d.ts.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/cjs/processor.d.ts.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/cjs/processor.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/cjs/processor.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/cjs/processor.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/cjs/processor.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/cjs/walker.d.ts` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/cjs/walker.d.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/cjs/walker.d.ts.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/cjs/walker.d.ts.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/cjs/walker.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/cjs/walker.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/cjs/walker.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/cjs/walker.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/mjs/glob.d.ts` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/mjs/glob.d.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/mjs/glob.d.ts.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/mjs/glob.d.ts.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/mjs/glob.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/mjs/glob.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/mjs/glob.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/mjs/glob.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/mjs/has-magic.d.ts` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/mjs/has-magic.d.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/mjs/has-magic.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/mjs/has-magic.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/mjs/ignore.d.ts` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/mjs/ignore.d.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/mjs/ignore.d.ts.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/mjs/ignore.d.ts.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/mjs/ignore.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/mjs/ignore.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/mjs/ignore.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/mjs/ignore.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/mjs/index.d.ts` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/mjs/index.d.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/mjs/index.d.ts.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/mjs/index.d.ts.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/mjs/index.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/mjs/index.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/mjs/index.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/mjs/index.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/mjs/pattern.d.ts` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/mjs/pattern.d.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/mjs/pattern.d.ts.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/mjs/pattern.d.ts.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/mjs/pattern.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/mjs/pattern.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/mjs/pattern.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/mjs/pattern.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/mjs/processor.d.ts` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/mjs/processor.d.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/mjs/processor.d.ts.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/mjs/processor.d.ts.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/mjs/processor.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/mjs/processor.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/mjs/processor.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/mjs/processor.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/mjs/walker.d.ts` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/mjs/walker.d.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/mjs/walker.d.ts.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/mjs/walker.d.ts.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/mjs/walker.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/mjs/walker.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/glob/dist/mjs/walker.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/glob/dist/mjs/walker.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minimatch/LICENSE` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minimatch/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minimatch/README.md` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minimatch/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minimatch/package.json` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minimatch/package.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minimatch/dist/cjs/brace-expressions.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minimatch/dist/cjs/brace-expressions.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minimatch/dist/cjs/brace-expressions.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minimatch/dist/cjs/brace-expressions.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minimatch/dist/cjs/escape.d.ts` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minimatch/dist/cjs/escape.d.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minimatch/dist/cjs/escape.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minimatch/dist/cjs/escape.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minimatch/dist/cjs/index-cjs.d.ts` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minimatch/dist/cjs/index-cjs.d.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minimatch/dist/cjs/index.d.ts` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minimatch/dist/cjs/index.d.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minimatch/dist/cjs/index.d.ts.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minimatch/dist/cjs/index.d.ts.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minimatch/dist/cjs/index.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minimatch/dist/cjs/index.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minimatch/dist/cjs/index.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minimatch/dist/cjs/index.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minimatch/dist/cjs/unescape.d.ts` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minimatch/dist/cjs/unescape.d.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minimatch/dist/cjs/unescape.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minimatch/dist/cjs/unescape.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minimatch/dist/mjs/brace-expressions.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minimatch/dist/mjs/brace-expressions.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minimatch/dist/mjs/brace-expressions.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minimatch/dist/mjs/brace-expressions.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minimatch/dist/mjs/escape.d.ts` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minimatch/dist/mjs/escape.d.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minimatch/dist/mjs/escape.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minimatch/dist/mjs/escape.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minimatch/dist/mjs/index.d.ts` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minimatch/dist/mjs/index.d.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minimatch/dist/mjs/index.d.ts.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minimatch/dist/mjs/index.d.ts.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minimatch/dist/mjs/index.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minimatch/dist/mjs/index.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minimatch/dist/mjs/index.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minimatch/dist/mjs/index.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minimatch/dist/mjs/unescape.d.ts` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minimatch/dist/mjs/unescape.d.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minimatch/dist/mjs/unescape.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minimatch/dist/mjs/unescape.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minipass/LICENSE` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minipass/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minipass/README.md` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minipass/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minipass/index.d.ts` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minipass/index.d.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minipass/index.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minipass/index.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minipass/index.mjs` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minipass/index.mjs`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/minipass/package.json` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/minipass/package.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/LICENSE` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/README.md` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/package.json` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/package.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/package.json` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/package.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/bin.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/bin.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/bin.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/bin.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/default-tmp.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/default-tmp.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/default-tmp.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/default-tmp.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/fix-eperm.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/fix-eperm.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/fix-eperm.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/fix-eperm.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/fs.d.ts` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/fs.d.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/fs.d.ts.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/fs.d.ts.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/fs.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/fs.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/fs.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/fs.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/ignore-enoent.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/ignore-enoent.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/ignore-enoent.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/ignore-enoent.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/index-cjs.d.ts` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/index-cjs.d.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/index.d.ts` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/index.d.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/index.d.ts.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/index.d.ts.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/index.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/index.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/index.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/index.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/opt-arg.d.ts` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/opt-arg.d.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/opt-arg.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/opt-arg.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/opt-arg.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/opt-arg.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/path-arg.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/path-arg.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/path-arg.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/path-arg.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/readdir-or-error.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/readdir-or-error.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/readdir-or-error.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/readdir-or-error.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/retry-busy.d.ts` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/retry-busy.d.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/retry-busy.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/retry-busy.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/retry-busy.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/retry-busy.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/rimraf-manual.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/rimraf-manual.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/rimraf-move-remove.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/rimraf-move-remove.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/rimraf-move-remove.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/rimraf-move-remove.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/rimraf-native.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/rimraf-native.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/rimraf-native.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/rimraf-native.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/rimraf-posix.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/rimraf-posix.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/rimraf-posix.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/rimraf-posix.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/rimraf-windows.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/rimraf-windows.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/rimraf-windows.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/rimraf-windows.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/use-native.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/use-native.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/use-native.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/cjs/src/use-native.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/default-tmp.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/default-tmp.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/default-tmp.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/default-tmp.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/fix-eperm.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/fix-eperm.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/fix-eperm.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/fix-eperm.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/fs.d.ts` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/fs.d.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/fs.d.ts.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/fs.d.ts.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/fs.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/fs.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/fs.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/fs.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/index.d.ts` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/index.d.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/index.d.ts.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/index.d.ts.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/index.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/index.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/index.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/index.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/opt-arg.d.ts` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/opt-arg.d.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/opt-arg.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/opt-arg.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/opt-arg.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/opt-arg.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/path-arg.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/path-arg.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/path-arg.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/path-arg.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/readdir-or-error.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/readdir-or-error.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/retry-busy.d.ts` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/retry-busy.d.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/retry-busy.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/retry-busy.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/retry-busy.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/retry-busy.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/rimraf-move-remove.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/rimraf-move-remove.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/rimraf-move-remove.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/rimraf-move-remove.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/rimraf-native.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/rimraf-native.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/rimraf-posix.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/rimraf-posix.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/rimraf-posix.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/rimraf-posix.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/rimraf-windows.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/rimraf-windows.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/rimraf-windows.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/rimraf-windows.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/use-native.js` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/use-native.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/node_modules/rimraf/dist/mjs/use-native.js.map` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/node_modules/rimraf/dist/mjs/use-native.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/src/index.ts` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/src/index.ts`

 * *Files 10% similar despite different names*

```diff
@@ -3,20 +3,28 @@
   JupyterFrontEndPlugin,
   ILayoutRestorer
 } from '@jupyterlab/application';
 import { jsonIcon } from '@jupyterlab/ui-components';
 import { WidgetTracker, ICommandPalette } from '@jupyterlab/apputils';
 import { IRenderMimeRegistry } from '@jupyterlab/rendermime';
 import { IEditorServices } from '@jupyterlab/codeeditor';
+import { CodeCell } from '@jupyterlab/cells';
 import { IFileBrowserFactory } from '@jupyterlab/filebrowser';
 import { ILauncher } from '@jupyterlab/launcher';
 import { ITranslator } from '@jupyterlab/translation';
 import { ISettingRegistry } from '@jupyterlab/settingregistry';
 import { IKernelMenu, IMainMenu } from '@jupyterlab/mainmenu';
 
+import { IJupyterWidgetRegistry } from '@jupyter-widgets/base';
+
+import {
+  WidgetRenderer,
+  registerWidgetManager
+} from '@jupyter-widgets/jupyterlab-manager';
+
 import { BlocklyEditorFactory } from 'jupyterlab-blockly';
 import { IBlocklyRegistry } from 'jupyterlab-blockly';
 import { BlocklyEditor } from 'jupyterlab-blockly';
 
 import { blockly_icon } from './icons';
 
 /**
@@ -45,27 +53,28 @@
     ILayoutRestorer,
     IRenderMimeRegistry,
     IEditorServices,
     IFileBrowserFactory,
     ISettingRegistry,
     ITranslator
   ],
-  optional: [ILauncher, ICommandPalette, IMainMenu],
+  optional: [ILauncher, ICommandPalette, IMainMenu, IJupyterWidgetRegistry],
   provides: IBlocklyRegistry,
   activate: (
     app: JupyterFrontEnd,
     restorer: ILayoutRestorer,
     rendermime: IRenderMimeRegistry,
     editorServices: IEditorServices,
     browserFactory: IFileBrowserFactory,
     settings: ISettingRegistry,
     translator: ITranslator,
     launcher: ILauncher | null,
     palette: ICommandPalette | null,
-    mainMenu: IMainMenu | null
+    mainMenu: IMainMenu | null,
+    widgetRegistry: IJupyterWidgetRegistry | null
   ): IBlocklyRegistry => {
     console.log('JupyterLab extension jupyterlab-blocky is activated!');
 
     // Namespace for the tracker
     const namespace = 'jupyterlab-blocky';
 
     // Creating the tracker for the document
@@ -229,12 +238,38 @@
           }
           return Promise.resolve(void 0);
         },
         shutdownKernel: current => current.context.sessionContext.shutdown()
       } as IKernelMenu.IKernelUser<BlocklyEditor>);
     }
 
+    if (widgetRegistry) {
+      tracker.forEach(panel => {
+        registerWidgetManager(
+          panel.context as any,
+          panel.content.rendermime,
+          widgetRenderers([panel.content.cell])
+        );
+      });
+
+      tracker.widgetAdded.connect((sender, panel) => {
+        registerWidgetManager(
+          panel.context as any,
+          panel.content.rendermime,
+          widgetRenderers([panel.content.cell])
+        );
+      });
+    }
+
     return widgetFactory.registry;
   }
 };
 
+function* widgetRenderers(cells: CodeCell[]): IterableIterator<WidgetRenderer> {
+  for (const w of cells) {
+    if (w instanceof WidgetRenderer) {
+      yield w;
+    }
+  }
+}
+
 export default plugin;
```

### Comparing `jupyterlab_blockly-0.3.0a0/packages/blockly-extension/style/icons/blockly_logo.svg` & `jupyterlab_blockly-0.3.0a1/packages/blockly-extension/style/icons/blockly_logo.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/.gitignore` & `jupyterlab_blockly-0.3.0a1/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/LICENSE` & `jupyterlab_blockly-0.3.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/README.md` & `jupyterlab_blockly-0.3.0a1/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_blockly-0.3.0a0/pyproject.toml` & `jupyterlab_blockly-0.3.0a1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,16 @@
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
-	"jupyterlab~=3.6"
+	"jupyterlab~=3.6",
+    "jupyterlab_widgets~=3.0"
 ]
 dynamic = ["version", "description", "authors", "urls", "keywords"]
 
 [project.optional-dependencies]
 dev = [
     "click",
     "pre-commit",
```

### Comparing `jupyterlab_blockly-0.3.0a0/PKG-INFO` & `jupyterlab_blockly-0.3.0a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab_blockly
-Version: 0.3.0a0
+Version: 0.3.0a1
 Summary: Blockly extension for JupyterLab.
 Project-URL: Homepage, https://github.com/quantstack/jupyterlab-blockly
 Project-URL: Bug Tracker, https://github.com/quantstack/jupyterlab-blockly/issues
 Author: quantstack
 License: BSD 3-Clause License
         
         Copyright (c) 2022, quantstack
@@ -45,14 +45,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
+Requires-Dist: jupyterlab-widgets~=3.0
 Requires-Dist: jupyterlab~=3.6
 Provides-Extra: dev
 Requires-Dist: click; extra == 'dev'
 Requires-Dist: jupyter-releaser; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
 Description-Content-Type: text/markdown
```

