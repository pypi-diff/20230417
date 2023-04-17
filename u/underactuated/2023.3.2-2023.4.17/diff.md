# Comparing `tmp/underactuated-2023.3.2.tar.gz` & `tmp/underactuated-2023.4.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "underactuated-2023.3.2.tar", last modified: Thu Mar  2 13:21:40 2023, max compression
+gzip compressed data, was "underactuated-2023.4.17.tar", last modified: Mon Apr 17 15:18:20 2023, max compression
```

## Comparing `underactuated-2023.3.2.tar` & `underactuated-2023.4.17.tar`

### file list

```diff
@@ -1,117 +1,120 @@
-drwxrwxr-x   0 russt     (1002) russt     (1002)        0 2023-03-02 13:21:40.185962 underactuated-2023.3.2/
--rw-rw-r--   0 russt     (1002) russt     (1002)     1703 2022-03-07 00:40:42.000000 underactuated-2023.3.2/LICENSE.TXT
--rw-rw-r--   0 russt     (1002) russt     (1002)       79 2022-03-07 00:40:42.000000 underactuated-2023.3.2/MANIFEST.in
--rw-rw-r--   0 russt     (1002) russt     (1002)     1064 2023-03-02 13:21:40.185962 underactuated-2023.3.2/PKG-INFO
--rw-rw-r--   0 russt     (1002) russt     (1002)      550 2022-10-02 16:20:06.000000 underactuated-2023.3.2/README.md
--rw-rw-r--   0 russt     (1002) russt     (1002)      103 2022-03-07 00:40:42.000000 underactuated-2023.3.2/pyproject.toml
--rw-rw-r--   0 russt     (1002) russt     (1002)     3169 2023-03-02 13:21:40.185962 underactuated-2023.3.2/setup.cfg
-drwxrwxr-x   0 russt     (1002) russt     (1002)        0 2023-03-02 13:21:40.165962 underactuated-2023.3.2/underactuated/
--rw-rw-r--   0 russt     (1002) russt     (1002)      293 2022-03-07 00:40:42.000000 underactuated-2023.3.2/underactuated/__init__.py
--rw-rw-r--   0 russt     (1002) russt     (1002)     1814 2022-03-07 00:40:42.000000 underactuated-2023.3.2/underactuated/double_integrator.py
-drwxrwxr-x   0 russt     (1002) russt     (1002)        0 2023-03-02 13:21:40.165962 underactuated-2023.3.2/underactuated/exercises/
-drwxrwxr-x   0 russt     (1002) russt     (1002)        0 2023-03-02 13:21:40.165962 underactuated-2023.3.2/underactuated/exercises/acrobot/
--rw-rw-r--   0 russt     (1002) russt     (1002)     9021 2022-08-16 10:06:31.000000 underactuated-2023.3.2/underactuated/exercises/acrobot/test_cartpole_balancing.py
--rw-rw-r--   0 russt     (1002) russt     (1002)    10554 2023-02-25 02:27:36.000000 underactuated-2023.3.2/underactuated/exercises/acrobot/test_cartpoles_urdf.py
-drwxrwxr-x   0 russt     (1002) russt     (1002)        0 2023-03-02 13:21:40.165962 underactuated-2023.3.2/underactuated/exercises/contact/
--rw-rw-r--   0 russt     (1002) russt     (1002)     7786 2023-02-24 02:58:02.000000 underactuated-2023.3.2/underactuated/exercises/contact/test_compass_gait_limit_cycle.py
-drwxrwxr-x   0 russt     (1002) russt     (1002)        0 2023-03-02 13:21:40.165962 underactuated-2023.3.2/underactuated/exercises/dp/
--rw-rw-r--   0 russt     (1002) russt     (1002)     6191 2023-02-24 02:58:02.000000 underactuated-2023.3.2/underactuated/exercises/dp/minimum_time_utils.py
--rw-rw-r--   0 russt     (1002) russt     (1002)      794 2023-02-24 02:58:02.000000 underactuated-2023.3.2/underactuated/exercises/dp/test_lp_dp.py
--rw-rw-r--   0 russt     (1002) russt     (1002)     1168 2023-02-24 02:58:02.000000 underactuated-2023.3.2/underactuated/exercises/dp/test_minimum_time.py
--rw-rw-r--   0 russt     (1002) russt     (1002)     9667 2023-02-06 13:33:57.000000 underactuated-2023.3.2/underactuated/exercises/dp/test_pendulum_cvi.py
--rw-rw-r--   0 russt     (1002) russt     (1002)     4450 2022-03-07 00:40:42.000000 underactuated-2023.3.2/underactuated/exercises/grader.py
-drwxrwxr-x   0 russt     (1002) russt     (1002)        0 2023-03-02 13:21:40.165962 underactuated-2023.3.2/underactuated/exercises/humanoids/
--rw-rw-r--   0 russt     (1002) russt     (1002)     6202 2022-08-16 10:06:31.000000 underactuated-2023.3.2/underactuated/exercises/humanoids/test_footstep_planning.py
-drwxrwxr-x   0 russt     (1002) russt     (1002)        0 2023-03-02 13:21:40.169962 underactuated-2023.3.2/underactuated/exercises/intro/
--rw-rw-r--   0 russt     (1002) russt     (1002)     1763 2023-02-24 02:58:02.000000 underactuated-2023.3.2/underactuated/exercises/intro/test_drake_systems.py
-drwxrwxr-x   0 russt     (1002) russt     (1002)        0 2023-03-02 13:21:40.169962 underactuated-2023.3.2/underactuated/exercises/lqr/
--rw-rw-r--   0 russt     (1002) russt     (1002)     4957 2023-02-24 02:58:02.000000 underactuated-2023.3.2/underactuated/exercises/lqr/test_drake_diagrams.py
-drwxrwxr-x   0 russt     (1002) russt     (1002)        0 2023-03-02 13:21:40.169962 underactuated-2023.3.2/underactuated/exercises/lyapunov/
--rw-rw-r--   0 russt     (1002) russt     (1002)     7744 2022-08-16 10:06:31.000000 underactuated-2023.3.2/underactuated/exercises/lyapunov/test_control.py
--rw-rw-r--   0 russt     (1002) russt     (1002)     4108 2022-08-16 10:06:31.000000 underactuated-2023.3.2/underactuated/exercises/lyapunov/test_van_der_pol.py
-drwxrwxr-x   0 russt     (1002) russt     (1002)        0 2023-03-02 13:21:40.169962 underactuated-2023.3.2/underactuated/exercises/pend/
--rw-rw-r--   0 russt     (1002) russt     (1002)     2610 2022-08-16 10:06:31.000000 underactuated-2023.3.2/underactuated/exercises/pend/test_hopfield_network.py
--rw-rw-r--   0 russt     (1002) russt     (1002)     1125 2022-08-16 10:06:31.000000 underactuated-2023.3.2/underactuated/exercises/pend/test_vibrating_pendulum.py
-drwxrwxr-x   0 russt     (1002) russt     (1002)        0 2023-03-02 13:21:40.169962 underactuated-2023.3.2/underactuated/exercises/planning/
--rw-rw-r--   0 russt     (1002) russt     (1002)     5642 2022-08-16 10:06:31.000000 underactuated-2023.3.2/underactuated/exercises/planning/test_rrt_planning.py
-drwxrwxr-x   0 russt     (1002) russt     (1002)        0 2023-03-02 13:21:40.169962 underactuated-2023.3.2/underactuated/exercises/simple_legs/
--rw-rw-r--   0 russt     (1002) russt     (1002)     5429 2022-08-16 10:06:31.000000 underactuated-2023.3.2/underactuated/exercises/simple_legs/test_one_d_hopper.py
-drwxrwxr-x   0 russt     (1002) russt     (1002)        0 2023-03-02 13:21:40.169962 underactuated-2023.3.2/underactuated/exercises/sysid/
--rw-rw-r--   0 russt     (1002) russt     (1002)     2123 2022-08-16 10:06:31.000000 underactuated-2023.3.2/underactuated/exercises/sysid/test_glider_sysid.py
--rw-rw-r--   0 russt     (1002) russt     (1002)     2282 2022-08-16 10:06:31.000000 underactuated-2023.3.2/underactuated/exercises/sysid/test_linear_sysid.py
-drwxrwxr-x   0 russt     (1002) russt     (1002)        0 2023-03-02 13:21:40.169962 underactuated-2023.3.2/underactuated/exercises/trajopt/
--rw-rw-r--   0 russt     (1002) russt     (1002)    10464 2022-08-16 10:06:31.000000 underactuated-2023.3.2/underactuated/exercises/trajopt/test_ilqr_driving.py
--rw-rw-r--   0 russt     (1002) russt     (1002)     4556 2022-08-16 10:06:31.000000 underactuated-2023.3.2/underactuated/exercises/trajopt/test_orbital_transfer.py
--rw-rw-r--   0 russt     (1002) russt     (1002)     8851 2022-08-16 10:06:31.000000 underactuated-2023.3.2/underactuated/exercises/trajopt/test_shooting_vs_transcription.py
--rw-rw-r--   0 russt     (1002) russt     (1002)     6145 2022-05-02 09:17:40.000000 underactuated-2023.3.2/underactuated/jupyter.py
--rw-rw-r--   0 russt     (1002) russt     (1002)      249 2023-02-15 10:53:50.000000 underactuated-2023.3.2/underactuated/meshcat_cpp_utils.py
--rw-rw-r--   0 russt     (1002) russt     (1002)    23151 2023-02-15 10:53:50.000000 underactuated-2023.3.2/underactuated/meshcat_utils.py
-drwxrwxr-x   0 russt     (1002) russt     (1002)        0 2023-03-02 13:21:40.173962 underactuated-2023.3.2/underactuated/models/
--rw-rw-r--   0 russt     (1002) russt     (1002)     2331 2022-08-16 10:06:31.000000 underactuated-2023.3.2/underactuated/models/cartpole.urdf
--rw-rw-r--   0 russt     (1002) russt     (1002)     2879 2022-03-07 00:40:42.000000 underactuated-2023.3.2/underactuated/models/compass_gait_limit_cycle.urdf
--rw-rw-r--   0 russt     (1002) russt     (1002)     2151 2022-08-16 10:06:31.000000 underactuated-2023.3.2/underactuated/models/double_pendulum.sdf
--rw-rw-r--   0 russt     (1002) russt     (1002)     2417 2022-08-16 10:06:31.000000 underactuated-2023.3.2/underactuated/models/double_pendulum.urdf
-drwxrwxr-x   0 russt     (1002) russt     (1002)        0 2023-03-02 13:21:40.173962 underactuated-2023.3.2/underactuated/models/glider/
--rw-rw-r--   0 russt     (1002) russt     (1002)     5335 2022-03-07 00:40:42.000000 underactuated-2023.3.2/underactuated/models/glider/glider.urdf
-drwxrwxr-x   0 russt     (1002) russt     (1002)        0 2023-03-02 13:21:40.173962 underactuated-2023.3.2/underactuated/models/glider/meshes/
--rw-rw-r--   0 russt     (1002) russt     (1002)     4411 2022-03-07 00:40:42.000000 underactuated-2023.3.2/underactuated/models/glider/meshes/elevator.obj
--rw-rw-r--   0 russt     (1002) russt     (1002)     1192 2022-03-07 00:40:42.000000 underactuated-2023.3.2/underactuated/models/glider/meshes/fuselageh_hstab.obj
--rw-rw-r--   0 russt     (1002) russt     (1002)    17609 2022-03-07 00:40:42.000000 underactuated-2023.3.2/underactuated/models/glider/meshes/fuselageh_main.obj
--rw-rw-r--   0 russt     (1002) russt     (1002)    11270 2022-03-07 00:40:42.000000 underactuated-2023.3.2/underactuated/models/glider/meshes/fuselagev_main.obj
--rw-rw-r--   0 russt     (1002) russt     (1002)     1664 2022-03-07 00:40:42.000000 underactuated-2023.3.2/underactuated/models/glider/meshes/fuselagev_top.obj
--rw-rw-r--   0 russt     (1002) russt     (1002)     2316 2022-03-07 00:40:42.000000 underactuated-2023.3.2/underactuated/models/glider/meshes/fuselagev_vstab.obj
--rw-rw-r--   0 russt     (1002) russt     (1002)     1460 2022-03-07 00:40:42.000000 underactuated-2023.3.2/underactuated/models/glider/meshes/wing_left.obj
--rw-rw-r--   0 russt     (1002) russt     (1002)     1577 2022-03-07 00:40:42.000000 underactuated-2023.3.2/underactuated/models/glider/meshes/wing_right.obj
-drwxrwxr-x   0 russt     (1002) russt     (1002)        0 2023-03-02 13:21:40.173962 underactuated-2023.3.2/underactuated/models/littledog/
--rw-rw-r--   0 russt     (1002) russt     (1002)     1679 2022-03-07 00:40:42.000000 underactuated-2023.3.2/underactuated/models/littledog/LICENSE.txt
--rw-rw-r--   0 russt     (1002) russt     (1002)    12800 2022-08-16 10:06:31.000000 underactuated-2023.3.2/underactuated/models/littledog/LittleDog.urdf
--rw-rw-r--   0 russt     (1002) russt     (1002)      411 2022-03-07 00:40:42.000000 underactuated-2023.3.2/underactuated/models/littledog/README.md
--rw-rw-r--   0 russt     (1002) russt     (1002)      666 2022-03-07 00:40:42.000000 underactuated-2023.3.2/underactuated/models/littledog/ground.urdf
-drwxrwxr-x   0 russt     (1002) russt     (1002)        0 2023-03-02 13:21:40.185962 underactuated-2023.3.2/underactuated/models/littledog/meshes/
--rw-rw-r--   0 russt     (1002) russt     (1002)    50176 2022-03-07 00:40:42.000000 underactuated-2023.3.2/underactuated/models/littledog/meshes/back_left_hip.obj
--rw-rw-r--   0 russt     (1002) russt     (1002)      200 2022-03-07 00:40:42.000000 underactuated-2023.3.2/underactuated/models/littledog/meshes/back_left_hip.obj.mtl
--rw-rw-r--   0 russt     (1002) russt     (1002)   121081 2022-03-07 00:40:42.000000 underactuated-2023.3.2/underactuated/models/littledog/meshes/back_left_lower.obj
--rw-rw-r--   0 russt     (1002) russt     (1002)      528 2022-03-07 00:40:42.000000 underactuated-2023.3.2/underactuated/models/littledog/meshes/back_left_lower.obj.mtl
--rw-rw-r--   0 russt     (1002) russt     (1002)   104694 2022-03-07 00:40:42.000000 underactuated-2023.3.2/underactuated/models/littledog/meshes/back_left_upper.obj
--rw-rw-r--   0 russt     (1002) russt     (1002)      512 2022-03-07 00:40:42.000000 underactuated-2023.3.2/underactuated/models/littledog/meshes/back_left_upper.obj.mtl
--rw-rw-r--   0 russt     (1002) russt     (1002)    51166 2022-03-07 00:40:42.000000 underactuated-2023.3.2/underactuated/models/littledog/meshes/back_right_hip.obj
--rw-rw-r--   0 russt     (1002) russt     (1002)      200 2022-03-07 00:40:42.000000 underactuated-2023.3.2/underactuated/models/littledog/meshes/back_right_hip.obj.mtl
--rw-rw-r--   0 russt     (1002) russt     (1002)   120989 2022-03-07 00:40:42.000000 underactuated-2023.3.2/underactuated/models/littledog/meshes/back_right_lower.obj
--rw-rw-r--   0 russt     (1002) russt     (1002)      528 2022-03-07 00:40:42.000000 underactuated-2023.3.2/underactuated/models/littledog/meshes/back_right_lower.obj.mtl
--rw-rw-r--   0 russt     (1002) russt     (1002)   105531 2022-03-07 00:40:42.000000 underactuated-2023.3.2/underactuated/models/littledog/meshes/back_right_upper.obj
--rw-rw-r--   0 russt     (1002) russt     (1002)      512 2022-03-07 00:40:42.000000 underactuated-2023.3.2/underactuated/models/littledog/meshes/back_right_upper.obj.mtl
--rw-rw-r--   0 russt     (1002) russt     (1002)  1036654 2022-03-07 00:40:42.000000 underactuated-2023.3.2/underactuated/models/littledog/meshes/body.obj
--rw-rw-r--   0 russt     (1002) russt     (1002)      357 2022-03-07 00:40:42.000000 underactuated-2023.3.2/underactuated/models/littledog/meshes/body.obj.mtl
--rw-rw-r--   0 russt     (1002) russt     (1002)    25320 2022-03-07 00:40:42.000000 underactuated-2023.3.2/underactuated/models/littledog/meshes/body2.jpg
--rw-rw-r--   0 russt     (1002) russt     (1002)    11322 2022-03-07 00:40:42.000000 underactuated-2023.3.2/underactuated/models/littledog/meshes/body3.jpg
--rw-rw-r--   0 russt     (1002) russt     (1002)    29266 2022-03-07 00:40:42.000000 underactuated-2023.3.2/underactuated/models/littledog/meshes/foot.jpg
--rw-rw-r--   0 russt     (1002) russt     (1002)    49151 2022-03-07 00:40:42.000000 underactuated-2023.3.2/underactuated/models/littledog/meshes/front_left_hip.obj
--rw-rw-r--   0 russt     (1002) russt     (1002)      200 2022-03-07 00:40:42.000000 underactuated-2023.3.2/underactuated/models/littledog/meshes/front_left_hip.obj.mtl
--rw-rw-r--   0 russt     (1002) russt     (1002)   121747 2022-03-07 00:40:42.000000 underactuated-2023.3.2/underactuated/models/littledog/meshes/front_left_lower.obj
--rw-rw-r--   0 russt     (1002) russt     (1002)      528 2022-03-07 00:40:42.000000 underactuated-2023.3.2/underactuated/models/littledog/meshes/front_left_lower.obj.mtl
--rw-rw-r--   0 russt     (1002) russt     (1002)   104401 2022-03-07 00:40:42.000000 underactuated-2023.3.2/underactuated/models/littledog/meshes/front_left_upper.obj
--rw-rw-r--   0 russt     (1002) russt     (1002)      512 2022-03-07 00:40:42.000000 underactuated-2023.3.2/underactuated/models/littledog/meshes/front_left_upper.obj.mtl
--rw-rw-r--   0 russt     (1002) russt     (1002)    58904 2022-03-07 00:40:42.000000 underactuated-2023.3.2/underactuated/models/littledog/meshes/front_right_hip.obj
--rw-rw-r--   0 russt     (1002) russt     (1002)      200 2022-03-07 00:40:42.000000 underactuated-2023.3.2/underactuated/models/littledog/meshes/front_right_hip.obj.mtl
--rw-rw-r--   0 russt     (1002) russt     (1002)   121685 2022-03-07 00:40:42.000000 underactuated-2023.3.2/underactuated/models/littledog/meshes/front_right_lower.obj
--rw-rw-r--   0 russt     (1002) russt     (1002)      528 2022-03-07 00:40:42.000000 underactuated-2023.3.2/underactuated/models/littledog/meshes/front_right_lower.obj.mtl
--rw-rw-r--   0 russt     (1002) russt     (1002)   104294 2022-03-07 00:40:42.000000 underactuated-2023.3.2/underactuated/models/littledog/meshes/front_right_upper.obj
--rw-rw-r--   0 russt     (1002) russt     (1002)      512 2022-03-07 00:40:42.000000 underactuated-2023.3.2/underactuated/models/littledog/meshes/front_right_upper.obj.mtl
--rw-rw-r--   0 russt     (1002) russt     (1002)    21971 2022-03-07 00:40:42.000000 underactuated-2023.3.2/underactuated/models/littledog/meshes/leg.jpg
--rw-rw-r--   0 russt     (1002) russt     (1002)     2820 2022-03-07 00:40:42.000000 underactuated-2023.3.2/underactuated/models/one_d_hopper.urdf
--rw-rw-r--   0 russt     (1002) russt     (1002)     1723 2022-03-07 00:40:42.000000 underactuated-2023.3.2/underactuated/models/undamped_cartpole.urdf
--rw-rw-r--   0 russt     (1002) russt     (1002)     1444 2022-03-07 00:40:42.000000 underactuated-2023.3.2/underactuated/models/vibrating_pendulum.urdf
--rw-rw-r--   0 russt     (1002) russt     (1002)      843 2022-08-16 10:06:31.000000 underactuated-2023.3.2/underactuated/multibody.py
--rw-rw-r--   0 russt     (1002) russt     (1002)     2368 2022-03-07 00:40:42.000000 underactuated-2023.3.2/underactuated/optimizers.py
--rw-rw-r--   0 russt     (1002) russt     (1002)     2299 2022-03-07 00:40:42.000000 underactuated-2023.3.2/underactuated/pendulum.py
--rw-rw-r--   0 russt     (1002) russt     (1002)     1865 2022-03-07 00:40:42.000000 underactuated-2023.3.2/underactuated/plot_utils.py
--rw-rw-r--   0 russt     (1002) russt     (1002)      959 2022-03-07 00:40:42.000000 underactuated-2023.3.2/underactuated/pyplot_visualizer.py
--rw-rw-r--   0 russt     (1002) russt     (1002)     5074 2022-08-16 10:06:31.000000 underactuated-2023.3.2/underactuated/quadrotor2d.py
--rw-rw-r--   0 russt     (1002) russt     (1002)     3793 2022-08-16 10:06:31.000000 underactuated-2023.3.2/underactuated/scenarios.py
--rw-rw-r--   0 russt     (1002) russt     (1002)     3166 2022-10-02 16:20:06.000000 underactuated-2023.3.2/underactuated/utils.py
-drwxrwxr-x   0 russt     (1002) russt     (1002)        0 2023-03-02 13:21:40.165962 underactuated-2023.3.2/underactuated.egg-info/
--rw-rw-r--   0 russt     (1002) russt     (1002)     1064 2023-03-02 13:21:40.000000 underactuated-2023.3.2/underactuated.egg-info/PKG-INFO
--rw-rw-r--   0 russt     (1002) russt     (1002)     4443 2023-03-02 13:21:40.000000 underactuated-2023.3.2/underactuated.egg-info/SOURCES.txt
--rw-rw-r--   0 russt     (1002) russt     (1002)        1 2023-03-02 13:21:40.000000 underactuated-2023.3.2/underactuated.egg-info/dependency_links.txt
--rw-rw-r--   0 russt     (1002) russt     (1002)       96 2023-03-02 13:21:40.000000 underactuated-2023.3.2/underactuated.egg-info/requires.txt
--rw-rw-r--   0 russt     (1002) russt     (1002)       14 2023-03-02 13:21:40.000000 underactuated-2023.3.2/underactuated.egg-info/top_level.txt
+drwxr-xr-x   0 russt      (504) staff       (20)        0 2023-04-17 15:18:20.027175 underactuated-2023.4.17/
+-rw-r--r--   0 russt      (504) staff       (20)     1703 2021-12-11 10:13:05.000000 underactuated-2023.4.17/LICENSE.TXT
+-rw-r--r--   0 russt      (504) staff       (20)       85 2023-04-16 10:35:33.000000 underactuated-2023.4.17/MANIFEST.in
+-rw-r--r--   0 russt      (504) staff       (20)     1065 2023-04-17 15:18:20.027270 underactuated-2023.4.17/PKG-INFO
+-rw-r--r--   0 russt      (504) staff       (20)      550 2022-10-02 15:34:42.000000 underactuated-2023.4.17/README.md
+-rw-r--r--   0 russt      (504) staff       (20)      609 2023-03-16 10:55:11.000000 underactuated-2023.4.17/pyproject.toml
+-rw-r--r--   0 russt      (504) staff       (20)     3169 2023-04-17 15:18:20.027966 underactuated-2023.4.17/setup.cfg
+drwxr-xr-x   0 russt      (504) staff       (20)        0 2023-04-17 15:18:19.999704 underactuated-2023.4.17/underactuated/
+-rw-r--r--   0 russt      (504) staff       (20)      311 2023-03-16 10:52:43.000000 underactuated-2023.4.17/underactuated/__init__.py
+-rw-r--r--   0 russt      (504) staff       (20)     1692 2023-03-16 10:52:43.000000 underactuated-2023.4.17/underactuated/double_integrator.py
+drwxr-xr-x   0 russt      (504) staff       (20)        0 2023-04-17 15:18:20.000847 underactuated-2023.4.17/underactuated/exercises/
+drwxr-xr-x   0 russt      (504) staff       (20)        0 2023-04-17 15:18:20.001547 underactuated-2023.4.17/underactuated/exercises/acrobot/
+-rw-r--r--   0 russt      (504) staff       (20)    14129 2023-03-16 10:52:43.000000 underactuated-2023.4.17/underactuated/exercises/acrobot/test_cartpole_balancing.py
+-rw-r--r--   0 russt      (504) staff       (20)    12035 2023-03-16 10:52:43.000000 underactuated-2023.4.17/underactuated/exercises/acrobot/test_cartpoles_urdf.py
+drwxr-xr-x   0 russt      (504) staff       (20)        0 2023-04-17 15:18:20.001848 underactuated-2023.4.17/underactuated/exercises/contact/
+-rw-r--r--   0 russt      (504) staff       (20)     7965 2023-03-16 10:52:43.000000 underactuated-2023.4.17/underactuated/exercises/contact/test_compass_gait_limit_cycle.py
+drwxr-xr-x   0 russt      (504) staff       (20)        0 2023-04-17 15:18:20.002848 underactuated-2023.4.17/underactuated/exercises/dp/
+-rw-r--r--   0 russt      (504) staff       (20)     5595 2023-03-12 02:22:59.000000 underactuated-2023.4.17/underactuated/exercises/dp/minimum_time_utils.py
+-rw-r--r--   0 russt      (504) staff       (20)      796 2023-03-16 10:52:43.000000 underactuated-2023.4.17/underactuated/exercises/dp/test_lp_dp.py
+-rw-r--r--   0 russt      (504) staff       (20)     1315 2023-03-16 10:52:43.000000 underactuated-2023.4.17/underactuated/exercises/dp/test_minimum_time.py
+-rw-r--r--   0 russt      (504) staff       (20)     9872 2023-03-16 10:52:43.000000 underactuated-2023.4.17/underactuated/exercises/dp/test_pendulum_cvi.py
+-rw-r--r--   0 russt      (504) staff       (20)     4542 2023-03-16 10:52:43.000000 underactuated-2023.4.17/underactuated/exercises/grader.py
+drwxr-xr-x   0 russt      (504) staff       (20)        0 2023-04-17 15:18:20.003094 underactuated-2023.4.17/underactuated/exercises/humanoids/
+-rw-r--r--   0 russt      (504) staff       (20)     6496 2023-03-16 10:52:43.000000 underactuated-2023.4.17/underactuated/exercises/humanoids/test_footstep_planning.py
+drwxr-xr-x   0 russt      (504) staff       (20)        0 2023-04-17 15:18:20.003311 underactuated-2023.4.17/underactuated/exercises/intro/
+-rw-r--r--   0 russt      (504) staff       (20)     1802 2023-03-16 10:52:43.000000 underactuated-2023.4.17/underactuated/exercises/intro/test_drake_systems.py
+drwxr-xr-x   0 russt      (504) staff       (20)        0 2023-04-17 15:18:20.003549 underactuated-2023.4.17/underactuated/exercises/lqr/
+-rw-r--r--   0 russt      (504) staff       (20)     5253 2023-03-12 02:22:59.000000 underactuated-2023.4.17/underactuated/exercises/lqr/test_drake_diagrams.py
+drwxr-xr-x   0 russt      (504) staff       (20)        0 2023-04-17 15:18:20.004480 underactuated-2023.4.17/underactuated/exercises/lyapunov/
+-rw-r--r--   0 russt      (504) staff       (20)     7516 2023-03-16 10:52:43.000000 underactuated-2023.4.17/underactuated/exercises/lyapunov/test_control.py
+-rw-r--r--   0 russt      (504) staff       (20)     1302 2023-03-23 11:35:19.000000 underactuated-2023.4.17/underactuated/exercises/lyapunov/test_sos_and_psd.py
+-rw-r--r--   0 russt      (504) staff       (20)     5349 2023-03-16 10:52:43.000000 underactuated-2023.4.17/underactuated/exercises/lyapunov/test_van_der_pol.py
+drwxr-xr-x   0 russt      (504) staff       (20)        0 2023-04-17 15:18:20.004849 underactuated-2023.4.17/underactuated/exercises/pend/
+-rw-r--r--   0 russt      (504) staff       (20)     2636 2023-03-16 10:52:43.000000 underactuated-2023.4.17/underactuated/exercises/pend/test_hopfield_network.py
+-rw-r--r--   0 russt      (504) staff       (20)     1127 2023-03-16 10:52:43.000000 underactuated-2023.4.17/underactuated/exercises/pend/test_vibrating_pendulum.py
+drwxr-xr-x   0 russt      (504) staff       (20)        0 2023-04-17 15:18:20.005032 underactuated-2023.4.17/underactuated/exercises/planning/
+-rw-r--r--   0 russt      (504) staff       (20)     5523 2023-03-16 10:52:43.000000 underactuated-2023.4.17/underactuated/exercises/planning/test_rrt_planning.py
+drwxr-xr-x   0 russt      (504) staff       (20)        0 2023-04-17 15:18:20.005197 underactuated-2023.4.17/underactuated/exercises/simple_legs/
+-rw-r--r--   0 russt      (504) staff       (20)     6829 2023-03-16 10:52:43.000000 underactuated-2023.4.17/underactuated/exercises/simple_legs/test_one_d_hopper.py
+drwxr-xr-x   0 russt      (504) staff       (20)        0 2023-04-17 15:18:20.006672 underactuated-2023.4.17/underactuated/exercises/sysid/
+-rw-r--r--   0 russt      (504) staff       (20)     1891 2023-03-16 10:52:43.000000 underactuated-2023.4.17/underactuated/exercises/sysid/test_glider_sysid.py
+-rw-r--r--   0 russt      (504) staff       (20)     2382 2023-03-16 10:52:43.000000 underactuated-2023.4.17/underactuated/exercises/sysid/test_linear_sysid.py
+drwxr-xr-x   0 russt      (504) staff       (20)        0 2023-04-17 15:18:20.007452 underactuated-2023.4.17/underactuated/exercises/trajopt/
+-rw-r--r--   0 russt      (504) staff       (20)    10059 2023-03-16 10:52:43.000000 underactuated-2023.4.17/underactuated/exercises/trajopt/test_ilqr_driving.py
+-rw-r--r--   0 russt      (504) staff       (20)     4662 2023-03-16 10:52:43.000000 underactuated-2023.4.17/underactuated/exercises/trajopt/test_orbital_transfer.py
+-rw-r--r--   0 russt      (504) staff       (20)     9970 2023-03-16 10:52:43.000000 underactuated-2023.4.17/underactuated/exercises/trajopt/test_shooting_vs_transcription.py
+-rw-r--r--   0 russt      (504) staff       (20)     6016 2023-03-16 10:52:43.000000 underactuated-2023.4.17/underactuated/jupyter.py
+-rw-r--r--   0 russt      (504) staff       (20)      259 2023-03-12 02:22:59.000000 underactuated-2023.4.17/underactuated/meshcat_cpp_utils.py
+-rw-r--r--   0 russt      (504) staff       (20)    22418 2023-03-16 10:57:53.000000 underactuated-2023.4.17/underactuated/meshcat_utils.py
+drwxr-xr-x   0 russt      (504) staff       (20)        0 2023-04-17 15:18:20.009859 underactuated-2023.4.17/underactuated/models/
+-rw-r--r--   0 russt      (504) staff       (20)     2331 2022-07-13 01:24:22.000000 underactuated-2023.4.17/underactuated/models/cartpole.urdf
+-rw-r--r--   0 russt      (504) staff       (20)     2879 2021-12-11 10:13:05.000000 underactuated-2023.4.17/underactuated/models/compass_gait_limit_cycle.urdf
+-rw-r--r--   0 russt      (504) staff       (20)     2151 2022-07-13 01:24:22.000000 underactuated-2023.4.17/underactuated/models/double_pendulum.sdf
+-rw-r--r--   0 russt      (504) staff       (20)     2417 2022-07-13 01:24:22.000000 underactuated-2023.4.17/underactuated/models/double_pendulum.urdf
+drwxr-xr-x   0 russt      (504) staff       (20)        0 2023-04-17 15:18:20.010161 underactuated-2023.4.17/underactuated/models/glider/
+-rw-r--r--   0 russt      (504) staff       (20)     5943 2023-03-12 01:00:41.000000 underactuated-2023.4.17/underactuated/models/glider/glider.urdf
+drwxr-xr-x   0 russt      (504) staff       (20)        0 2023-04-17 15:18:20.012122 underactuated-2023.4.17/underactuated/models/glider/meshes/
+-rw-r--r--   0 russt      (504) staff       (20)     4411 2021-12-11 10:13:05.000000 underactuated-2023.4.17/underactuated/models/glider/meshes/elevator.obj
+-rw-r--r--   0 russt      (504) staff       (20)     1192 2021-12-11 10:13:05.000000 underactuated-2023.4.17/underactuated/models/glider/meshes/fuselageh_hstab.obj
+-rw-r--r--   0 russt      (504) staff       (20)    17609 2021-12-11 10:13:05.000000 underactuated-2023.4.17/underactuated/models/glider/meshes/fuselageh_main.obj
+-rw-r--r--   0 russt      (504) staff       (20)    11270 2021-12-11 10:13:05.000000 underactuated-2023.4.17/underactuated/models/glider/meshes/fuselagev_main.obj
+-rw-r--r--   0 russt      (504) staff       (20)     1664 2021-12-11 10:13:05.000000 underactuated-2023.4.17/underactuated/models/glider/meshes/fuselagev_top.obj
+-rw-r--r--   0 russt      (504) staff       (20)     2316 2021-12-11 10:13:05.000000 underactuated-2023.4.17/underactuated/models/glider/meshes/fuselagev_vstab.obj
+-rw-r--r--   0 russt      (504) staff       (20)     1460 2021-12-11 10:13:05.000000 underactuated-2023.4.17/underactuated/models/glider/meshes/wing_left.obj
+-rw-r--r--   0 russt      (504) staff       (20)     1577 2021-12-11 10:13:05.000000 underactuated-2023.4.17/underactuated/models/glider/meshes/wing_right.obj
+-rw-r--r--   0 russt      (504) staff       (20)     5297 2023-04-09 21:56:41.000000 underactuated-2023.4.17/underactuated/models/kneed_compass_gait.urdf
+drwxr-xr-x   0 russt      (504) staff       (20)        0 2023-04-17 15:18:20.013460 underactuated-2023.4.17/underactuated/models/littledog/
+-rw-r--r--   0 russt      (504) staff       (20)     1679 2021-12-11 10:13:05.000000 underactuated-2023.4.17/underactuated/models/littledog/LICENSE.txt
+-rw-r--r--   0 russt      (504) staff       (20)    13333 2023-03-12 01:00:41.000000 underactuated-2023.4.17/underactuated/models/littledog/LittleDog.urdf
+-rw-r--r--   0 russt      (504) staff       (20)      411 2021-12-11 10:13:05.000000 underactuated-2023.4.17/underactuated/models/littledog/README.md
+-rw-r--r--   0 russt      (504) staff       (20)      666 2021-12-11 10:13:05.000000 underactuated-2023.4.17/underactuated/models/littledog/ground.urdf
+drwxr-xr-x   0 russt      (504) staff       (20)        0 2023-04-17 15:18:20.026934 underactuated-2023.4.17/underactuated/models/littledog/meshes/
+-rw-r--r--   0 russt      (504) staff       (20)    50176 2021-12-11 10:13:05.000000 underactuated-2023.4.17/underactuated/models/littledog/meshes/back_left_hip.obj
+-rw-r--r--   0 russt      (504) staff       (20)      200 2022-01-14 11:58:31.000000 underactuated-2023.4.17/underactuated/models/littledog/meshes/back_left_hip.obj.mtl
+-rw-r--r--   0 russt      (504) staff       (20)   121081 2021-12-11 10:13:05.000000 underactuated-2023.4.17/underactuated/models/littledog/meshes/back_left_lower.obj
+-rw-r--r--   0 russt      (504) staff       (20)      528 2022-01-14 11:58:31.000000 underactuated-2023.4.17/underactuated/models/littledog/meshes/back_left_lower.obj.mtl
+-rw-r--r--   0 russt      (504) staff       (20)   104694 2021-12-11 10:13:05.000000 underactuated-2023.4.17/underactuated/models/littledog/meshes/back_left_upper.obj
+-rw-r--r--   0 russt      (504) staff       (20)      512 2022-01-14 11:58:31.000000 underactuated-2023.4.17/underactuated/models/littledog/meshes/back_left_upper.obj.mtl
+-rw-r--r--   0 russt      (504) staff       (20)    51166 2021-12-11 10:13:05.000000 underactuated-2023.4.17/underactuated/models/littledog/meshes/back_right_hip.obj
+-rw-r--r--   0 russt      (504) staff       (20)      200 2022-01-14 11:58:31.000000 underactuated-2023.4.17/underactuated/models/littledog/meshes/back_right_hip.obj.mtl
+-rw-r--r--   0 russt      (504) staff       (20)   120989 2021-12-11 10:13:05.000000 underactuated-2023.4.17/underactuated/models/littledog/meshes/back_right_lower.obj
+-rw-r--r--   0 russt      (504) staff       (20)      528 2022-01-14 11:58:31.000000 underactuated-2023.4.17/underactuated/models/littledog/meshes/back_right_lower.obj.mtl
+-rw-r--r--   0 russt      (504) staff       (20)   105531 2021-12-11 10:13:05.000000 underactuated-2023.4.17/underactuated/models/littledog/meshes/back_right_upper.obj
+-rw-r--r--   0 russt      (504) staff       (20)      512 2022-01-14 11:58:31.000000 underactuated-2023.4.17/underactuated/models/littledog/meshes/back_right_upper.obj.mtl
+-rw-r--r--   0 russt      (504) staff       (20)  1036654 2021-12-11 10:13:05.000000 underactuated-2023.4.17/underactuated/models/littledog/meshes/body.obj
+-rw-r--r--   0 russt      (504) staff       (20)      357 2022-01-14 11:58:31.000000 underactuated-2023.4.17/underactuated/models/littledog/meshes/body.obj.mtl
+-rw-r--r--   0 russt      (504) staff       (20)    25320 2021-12-11 10:13:05.000000 underactuated-2023.4.17/underactuated/models/littledog/meshes/body2.jpg
+-rw-r--r--   0 russt      (504) staff       (20)    11322 2021-12-11 10:13:05.000000 underactuated-2023.4.17/underactuated/models/littledog/meshes/body3.jpg
+-rw-r--r--   0 russt      (504) staff       (20)    29266 2021-12-11 10:13:05.000000 underactuated-2023.4.17/underactuated/models/littledog/meshes/foot.jpg
+-rw-r--r--   0 russt      (504) staff       (20)    49151 2021-12-11 10:13:05.000000 underactuated-2023.4.17/underactuated/models/littledog/meshes/front_left_hip.obj
+-rw-r--r--   0 russt      (504) staff       (20)      200 2022-01-14 11:58:31.000000 underactuated-2023.4.17/underactuated/models/littledog/meshes/front_left_hip.obj.mtl
+-rw-r--r--   0 russt      (504) staff       (20)   121747 2021-12-11 10:13:05.000000 underactuated-2023.4.17/underactuated/models/littledog/meshes/front_left_lower.obj
+-rw-r--r--   0 russt      (504) staff       (20)      528 2022-01-14 11:58:31.000000 underactuated-2023.4.17/underactuated/models/littledog/meshes/front_left_lower.obj.mtl
+-rw-r--r--   0 russt      (504) staff       (20)   104401 2021-12-11 10:13:05.000000 underactuated-2023.4.17/underactuated/models/littledog/meshes/front_left_upper.obj
+-rw-r--r--   0 russt      (504) staff       (20)      512 2022-01-14 11:58:31.000000 underactuated-2023.4.17/underactuated/models/littledog/meshes/front_left_upper.obj.mtl
+-rw-r--r--   0 russt      (504) staff       (20)    58904 2021-12-11 10:13:05.000000 underactuated-2023.4.17/underactuated/models/littledog/meshes/front_right_hip.obj
+-rw-r--r--   0 russt      (504) staff       (20)      200 2022-01-14 11:58:31.000000 underactuated-2023.4.17/underactuated/models/littledog/meshes/front_right_hip.obj.mtl
+-rw-r--r--   0 russt      (504) staff       (20)   121685 2021-12-11 10:13:05.000000 underactuated-2023.4.17/underactuated/models/littledog/meshes/front_right_lower.obj
+-rw-r--r--   0 russt      (504) staff       (20)      528 2022-01-14 11:58:31.000000 underactuated-2023.4.17/underactuated/models/littledog/meshes/front_right_lower.obj.mtl
+-rw-r--r--   0 russt      (504) staff       (20)   104294 2021-12-11 10:13:05.000000 underactuated-2023.4.17/underactuated/models/littledog/meshes/front_right_upper.obj
+-rw-r--r--   0 russt      (504) staff       (20)      512 2022-01-14 11:58:31.000000 underactuated-2023.4.17/underactuated/models/littledog/meshes/front_right_upper.obj.mtl
+-rw-r--r--   0 russt      (504) staff       (20)    21971 2021-12-11 10:13:05.000000 underactuated-2023.4.17/underactuated/models/littledog/meshes/leg.jpg
+-rw-r--r--   0 russt      (504) staff       (20)     2820 2021-12-11 10:13:05.000000 underactuated-2023.4.17/underactuated/models/one_d_hopper.urdf
+-rw-r--r--   0 russt      (504) staff       (20)     1723 2021-12-11 10:13:05.000000 underactuated-2023.4.17/underactuated/models/undamped_cartpole.urdf
+-rw-r--r--   0 russt      (504) staff       (20)     1444 2021-12-11 10:13:05.000000 underactuated-2023.4.17/underactuated/models/vibrating_pendulum.urdf
+-rw-r--r--   0 russt      (504) staff       (20)      687 2023-03-12 02:22:59.000000 underactuated-2023.4.17/underactuated/multibody.py
+-rw-r--r--   0 russt      (504) staff       (20)     2341 2023-03-12 02:22:59.000000 underactuated-2023.4.17/underactuated/optimizers.py
+-rw-r--r--   0 russt      (504) staff       (20)      369 2023-03-12 01:00:41.000000 underactuated-2023.4.17/underactuated/package.xml
+-rw-r--r--   0 russt      (504) staff       (20)     2296 2023-03-16 11:05:00.000000 underactuated-2023.4.17/underactuated/pendulum.py
+-rw-r--r--   0 russt      (504) staff       (20)     1887 2023-03-16 10:52:43.000000 underactuated-2023.4.17/underactuated/plot_utils.py
+-rw-r--r--   0 russt      (504) staff       (20)      957 2023-03-16 10:52:43.000000 underactuated-2023.4.17/underactuated/pyplot_visualizer.py
+-rw-r--r--   0 russt      (504) staff       (20)     5263 2023-03-16 10:52:43.000000 underactuated-2023.4.17/underactuated/quadrotor2d.py
+-rw-r--r--   0 russt      (504) staff       (20)     3971 2023-03-12 02:22:59.000000 underactuated-2023.4.17/underactuated/scenarios.py
+-rw-r--r--   0 russt      (504) staff       (20)     2220 2023-04-14 12:16:55.000000 underactuated-2023.4.17/underactuated/utils.py
+drwxr-xr-x   0 russt      (504) staff       (20)        0 2023-04-17 15:18:20.000677 underactuated-2023.4.17/underactuated.egg-info/
+-rw-r--r--   0 russt      (504) staff       (20)     1065 2023-04-17 15:18:19.000000 underactuated-2023.4.17/underactuated.egg-info/PKG-INFO
+-rw-r--r--   0 russt      (504) staff       (20)     4567 2023-04-17 15:18:19.000000 underactuated-2023.4.17/underactuated.egg-info/SOURCES.txt
+-rw-r--r--   0 russt      (504) staff       (20)        1 2023-04-17 15:18:19.000000 underactuated-2023.4.17/underactuated.egg-info/dependency_links.txt
+-rw-r--r--   0 russt      (504) staff       (20)       96 2023-04-17 15:18:19.000000 underactuated-2023.4.17/underactuated.egg-info/requires.txt
+-rw-r--r--   0 russt      (504) staff       (20)       14 2023-04-17 15:18:19.000000 underactuated-2023.4.17/underactuated.egg-info/top_level.txt
```

### Comparing `underactuated-2023.3.2/LICENSE.TXT` & `underactuated-2023.4.17/LICENSE.TXT`

 * *Files identical despite different names*

### Comparing `underactuated-2023.3.2/PKG-INFO` & `underactuated-2023.4.17/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: underactuated
-Version: 2023.3.2
+Version: 2023.4.17
 Summary: MIT 6.832 - Underactuated Robotics
 Home-page: https://underactuated.csail.mit.edu
 Author: Russ Tedrake
 Author-email: russt@mit.edu
 Project-URL: Bug Tracker, https://github.com/RussTedrake/underactuated/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `underactuated-2023.3.2/README.md` & `underactuated-2023.4.17/README.md`

 * *Files identical despite different names*

### Comparing `underactuated-2023.3.2/setup.cfg` & `underactuated-2023.4.17/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = underactuated
-version = 2023.03.02
+version = 2023.04.17
 author = Russ Tedrake
 author_email = russt@mit.edu
 description = MIT 6.832 - Underactuated Robotics
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://underactuated.csail.mit.edu
 project_urls = 
@@ -16,15 +16,15 @@
 
 [options]
 package_dir = 
 include_package_data = True
 packages = find:
 python_requires = >=3.8
 install_requires = 
-	drake>=1.13.0
+	drake>=1.14.0
 	pandas
 	gradescope-utils>=0.4.0
 	mpld3>=0.5.1
 	pydot>=1.3.0
 	timeout-decorator>=0.4.1
 
 [pycodestyle]
```

### Comparing `underactuated-2023.3.2/underactuated/double_integrator.py` & `underactuated-2023.4.17/underactuated/double_integrator.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,39 @@
-import numpy as np
 import matplotlib.pyplot as plt
-
+import numpy as np
+from pydrake.systems.framework import PortDataType
 from pydrake.systems.pyplot_visualizer import PyPlotVisualizer
-from pydrake.systems.framework import Context, PortDataType
 
 _MIT_RED = "#A31F34"
 
 
 class Brick(object):
-    WIDTH = 3.
-    HEIGHT = 1.
+    WIDTH = 3.0
+    HEIGHT = 1.0
 
     def __init__(self):
-        self.patch = plt.Rectangle((0.0, 0.0),
-                                   self.WIDTH,
-                                   self.HEIGHT,
-                                   fc=_MIT_RED,
-                                   ec="k")
-        self.set_state(0.)
+        self.patch = plt.Rectangle(
+            (0.0, 0.0), self.WIDTH, self.HEIGHT, fc=_MIT_RED, ec="k"
+        )
+        self.set_state(0.0)
 
     def set_state(self, x):
         self.patch.set_x(x - self.WIDTH / 2)  # Center at x
 
     @classmethod
     def add_to_axes(cls, ax):
         brick = cls()
         ax.add_patch(brick.patch)
         return brick
 
 
 class DoubleIntegratorVisualizer(PyPlotVisualizer):
-
     # Limits of view port
-    XLIM = (-15., 15.)
-    YLIM = (-6., 6.)
+    XLIM = (-15.0, 15.0)
+    YLIM = (-6.0, 6.0)
     TICK_DIMS = (0.2, 0.8)
 
     def __init__(self, ax=None, show=None):
         PyPlotVisualizer.__init__(self, ax=ax, show=show)
         self.DeclareInputPort("state", PortDataType.kVectorValued, 2)
 
         self.ax.set_xlim(*self.XLIM)
```

### Comparing `underactuated-2023.3.2/underactuated/exercises/acrobot/test_cartpoles_urdf.py` & `underactuated-2023.4.17/underactuated/exercises/acrobot/test_cartpoles_urdf.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import unittest
+
+import numpy as np
 import timeout_decorator
 from gradescope_utils.autograder_utils.decorators import weight
-import numpy as np
 
 
 class TestCartPolesURDF(unittest.TestCase):
-
     def __init__(self, test_name, notebook_locals):
         super().__init__(test_name)
         self.notebook_locals = notebook_locals
 
     @weight(1)
     @timeout_decorator.timeout(1.0)
     def test_x_star_single_state(self):
@@ -43,232 +43,295 @@
         )
 
     @weight(3)
     @timeout_decorator.timeout(10.0)
     def test_single_pendulum_urdf(self):
         """Test single-pendulum cart-pole dynamics"""
         # note: all prints here go to the output item in the json file
-        obtained_single_pend_urdf = self.notebook_locals["single_pendulum_urdf"]
+        obtained_single_pend_urdf = self.notebook_locals[
+            "single_pendulum_urdf"
+        ]
         cartpole_fn = self.notebook_locals["cartpole_balancing"]
         x_star = np.array([0, np.pi, 0, 0])
         Q = np.diag((10.0, 10.0, 1.0, 1.0))
         R = np.eye(1)
-        state_lst = np.array([
-            [0.05, np.pi * 0.95, -0.01, 0.01 * np.pi],
-            [-0.01, np.pi * 1.1, 0.1, 0.0],
-            [0.2, np.pi * 0.5, 0.01, 0.0],
-            [0.0, np.pi, 0.0, 0.0],
-            [-2, np.pi * 1.2, 0.0, -0.1 * np.pi],
-        ])
+        state_lst = np.array(
+            [
+                [0.05, np.pi * 0.95, -0.01, 0.01 * np.pi],
+                [-0.01, np.pi * 1.1, 0.1, 0.0],
+                [0.2, np.pi * 0.5, 0.01, 0.0],
+                [0.0, np.pi, 0.0, 0.0],
+                [-2, np.pi * 1.2, 0.0, -0.1 * np.pi],
+            ]
+        )
         diagram = cartpole_fn(obtained_single_pend_urdf, x_star, Q, R)
         cartpole = diagram.GetSubsystemByName("cartpole")
         context = cartpole.CreateDefaultContext()
         cartpole.get_actuation_input_port().FixValue(context, [0])
         result_lst = []
         for state in state_lst:
             context.SetContinuousState(state)
             result_lst.append(
-                cartpole.EvalTimeDerivatives(context).CopyToVector())
+                cartpole.EvalTimeDerivatives(context).CopyToVector()
+            )
         result = np.array(result_lst)
-        target_derivatives = np.array([
-            [-1.00000000e-02, 3.14159265e-02, -1.47937117e00, -2.99577976e00],
-            [1.00000000e-01, 0.00000000e00, 2.63177456e00, 5.53442305e00],
-            [1.00000000e-02, 0.00000000e00, 3.00344627e-16, -9.81000000e00],
-            [0.00000000e00, 0.00000000e00, -1.20137851e-15, -2.40275702e-15],
-            [0.00000000e00, -3.14159265e-01, 3.42396821e00, 8.53622180e00],
-        ])
+        target_derivatives = np.array(
+            [
+                [
+                    -1.00000000e-02,
+                    3.14159265e-02,
+                    -1.47937117e00,
+                    -2.99577976e00,
+                ],
+                [1.00000000e-01, 0.00000000e00, 2.63177456e00, 5.53442305e00],
+                [
+                    1.00000000e-02,
+                    0.00000000e00,
+                    3.00344627e-16,
+                    -9.81000000e00,
+                ],
+                [
+                    0.00000000e00,
+                    0.00000000e00,
+                    -1.20137851e-15,
+                    -2.40275702e-15,
+                ],
+                [0.00000000e00, -3.14159265e-01, 3.42396821e00, 8.53622180e00],
+            ]
+        )
         np.testing.assert_array_almost_equal(
             result,
             target_derivatives,
             decimal=6,
             err_msg="the dynamics for the single pendulum do not match",
         )
 
     @weight(3)
     @timeout_decorator.timeout(10.0)
     def test_double_pendulum_urdf(self):
         """Test double-pendulum cart-pole dynamics"""
         # note: all prints here go to the output item in the json file
-        obtained_double_pend_urdf = self.notebook_locals["double_pendulum_urdf"]
+        obtained_double_pend_urdf = self.notebook_locals[
+            "double_pendulum_urdf"
+        ]
         cartpole_fn = self.notebook_locals["cartpole_balancing"]
         x_star = np.array([0, np.pi, np.pi, 0, 0, 0])
         Q = np.diag((10.0, 10.0, 10.0, 1.0, 1.0, 1.0))
         R = np.eye(1)
-        state_lst = np.array([
-            [0.05, np.pi * 0.95, np.pi / 2, -0.01, 0.01 * np.pi, 0.0],
-            [-0.01, np.pi * 1.1, -np.pi * 0.1, 0.1, 0.0, -0.2 * np.pi],
-            [0.2, np.pi * 0.5, np.pi / 8, 0.01, 0.0, 0.0],
-            [0.0, np.pi, np.pi, 0.0, 0.0, 0.0],
-            [-2, np.pi * 1.2, 0.01, 0.2, 0.0, -0.1 * np.pi],
-        ])
+        state_lst = np.array(
+            [
+                [0.05, np.pi * 0.95, np.pi / 2, -0.01, 0.01 * np.pi, 0.0],
+                [-0.01, np.pi * 1.1, -np.pi * 0.1, 0.1, 0.0, -0.2 * np.pi],
+                [0.2, np.pi * 0.5, np.pi / 8, 0.01, 0.0, 0.0],
+                [0.0, np.pi, np.pi, 0.0, 0.0, 0.0],
+                [-2, np.pi * 1.2, 0.01, 0.2, 0.0, -0.1 * np.pi],
+            ]
+        )
         diagram = cartpole_fn(obtained_double_pend_urdf, x_star, Q, R)
         cartpole = diagram.GetSubsystemByName("cartpole")
         context = cartpole.CreateDefaultContext()
         cartpole.get_actuation_input_port().FixValue(context, [0])
         result_lst = []
         for state in state_lst:
             context.SetContinuousState(state)
             result_lst.append(
-                cartpole.EvalTimeDerivatives(context).CopyToVector())
+                cartpole.EvalTimeDerivatives(context).CopyToVector()
+            )
         result = np.array(result_lst)
-        target_derivatives = np.array([
-            [
-                -1.00000000e-02,
-                3.14159265e-02,
-                0.00000000e00,
-                -1.47937117e00,
-                -2.99627324e00,
-                -6.46053778e00,
-            ],
-            [
-                1.00000000e-01,
-                0.00000000e00,
-                -6.28318531e-01,
-                4.57233893e00,
-                9.61528333e00,
-                -5.04294440e00,
-            ],
-            [
-                1.00000000e-02,
-                0.00000000e00,
-                0.00000000e00,
-                1.61809378e-16,
-                -9.81000000e00,
-                9.81000000e00,
-            ],
+        target_derivatives = np.array(
             [
-                0.00000000e00,
-                0.00000000e00,
-                0.00000000e00,
-                -2.40275702e-15,
-                -2.40275702e-15,
-                0.00000000e00,
-            ],
-            [
-                2.00000000e-01,
-                0.00000000e00,
-                -3.14159265e-01,
-                5.55139729e00,
-                1.02096347e01,
-                -1.03040792e01,
-            ],
-        ])
+                [
+                    -1.00000000e-02,
+                    3.14159265e-02,
+                    0.00000000e00,
+                    -1.47937117e00,
+                    -2.99627324e00,
+                    -6.46053778e00,
+                ],
+                [
+                    1.00000000e-01,
+                    0.00000000e00,
+                    -6.28318531e-01,
+                    4.57233893e00,
+                    9.61528333e00,
+                    -5.04294440e00,
+                ],
+                [
+                    1.00000000e-02,
+                    0.00000000e00,
+                    0.00000000e00,
+                    1.61809378e-16,
+                    -9.81000000e00,
+                    9.81000000e00,
+                ],
+                [
+                    0.00000000e00,
+                    0.00000000e00,
+                    0.00000000e00,
+                    -2.40275702e-15,
+                    -2.40275702e-15,
+                    0.00000000e00,
+                ],
+                [
+                    2.00000000e-01,
+                    0.00000000e00,
+                    -3.14159265e-01,
+                    5.55139729e00,
+                    1.02096347e01,
+                    -1.03040792e01,
+                ],
+            ]
+        )
         np.testing.assert_array_almost_equal(
             result,
             target_derivatives,
             decimal=6,
             err_msg="the dynamics for the double pendulum do not match",
         )
 
     @weight(2)
     @timeout_decorator.timeout(10.0)
     def test_single_pendulum_lqr(self):
         """Test single-pendulum cart-pole LQR states"""
         # note: all prints here go to the output item in the json file
-        obtained_single_pend_urdf = self.notebook_locals["single_pendulum_urdf"]
+        obtained_single_pend_urdf = self.notebook_locals[
+            "single_pendulum_urdf"
+        ]
         cartpole_fn = self.notebook_locals["cartpole_balancing"]
         x_star = np.array([0, np.pi, 0, 0])
         Q = np.diag((10.0, 10.0, 1.0, 1.0))
         R = np.eye(1)
-        state_lst = np.array([
-            [0.05, np.pi * 0.95, -0.01, 0.01 * np.pi],
-            [-0.01, np.pi * 1.1, 0.1, 0.0],
-            [0.2, np.pi * 0.5, 0.01, 0.0],
-            [0.0, np.pi, 0.0, 0.0],
-            [-2, np.pi * 1.2, 0.0, -0.1 * np.pi],
-        ])
+        state_lst = np.array(
+            [
+                [0.05, np.pi * 0.95, -0.01, 0.01 * np.pi],
+                [-0.01, np.pi * 1.1, 0.1, 0.0],
+                [0.2, np.pi * 0.5, 0.01, 0.0],
+                [0.0, np.pi, 0.0, 0.0],
+                [-2, np.pi * 1.2, 0.0, -0.1 * np.pi],
+            ]
+        )
         diagram = cartpole_fn(obtained_single_pend_urdf, x_star, Q, R)
         result_lst = []
         context = diagram.CreateDefaultContext()
         for state in state_lst:
             context.SetContinuousState(state)
             result_lst.append(
-                diagram.EvalTimeDerivatives(context).CopyToVector())
+                diagram.EvalTimeDerivatives(context).CopyToVector()
+            )
         result = np.array(result_lst)
-        target_derivatives = np.array([
-            [-1.00000000e-02, 3.14159265e-02, 7.54162904e00, 5.91415697e00],
-            [1.00000000e-01, 0.00000000e00, -1.45222333e01, -1.07800079e01],
-            [1.00000000e-02, 0.00000000e00, 4.85651106e01, -9.81000000e00],
-            [0.00000000e00, 0.00000000e00, -1.20137851e-15, -2.40275702e-15],
-            [0.00000000e00, -3.14159265e-01, -2.61730991e01, -1.54083086e01],
-        ])
+        target_derivatives = np.array(
+            [
+                [
+                    -1.00000000e-02,
+                    3.14159265e-02,
+                    7.54162904e00,
+                    5.91415697e00,
+                ],
+                [
+                    1.00000000e-01,
+                    0.00000000e00,
+                    -1.45222333e01,
+                    -1.07800079e01,
+                ],
+                [1.00000000e-02, 0.00000000e00, 4.85651106e01, -9.81000000e00],
+                [
+                    0.00000000e00,
+                    0.00000000e00,
+                    -1.20137851e-15,
+                    -2.40275702e-15,
+                ],
+                [
+                    0.00000000e00,
+                    -3.14159265e-01,
+                    -2.61730991e01,
+                    -1.54083086e01,
+                ],
+            ]
+        )
         np.testing.assert_array_almost_equal(
             result,
             target_derivatives,
             decimal=4,
             err_msg="the dynamics for the single pendulum LQR do not match",
         )
 
     @weight(2)
     @timeout_decorator.timeout(10.0)
     def test_double_pendulum_lqr(self):
         """Test double-pendulum cart-pole LQR states"""
         # note: all prints here go to the output item in the json file
-        obtained_double_pend_urdf = self.notebook_locals["double_pendulum_urdf"]
+        obtained_double_pend_urdf = self.notebook_locals[
+            "double_pendulum_urdf"
+        ]
         diagram_fn = self.notebook_locals["cartpole_balancing"]
         x_star = np.array([0, np.pi, np.pi, 0, 0, 0])
         Q = np.diag((10.0, 10.0, 10.0, 1.0, 1.0, 1.0))
         R = np.eye(1)
         diagram = diagram_fn(obtained_double_pend_urdf, x_star, Q, R)
         context = diagram.CreateDefaultContext()
-        state_lst = np.array([
-            [0.05, np.pi * 0.95, np.pi / 2, -0.01, 0.01 * np.pi, 0.0],
-            [-0.01, np.pi * 1.1, -np.pi * 0.1, 0.1, 0.0, -0.2 * np.pi],
-            [0.2, np.pi * 0.5, np.pi / 8, 0.01, 0.0, 0.0],
-            [0.0, np.pi, np.pi, 0.0, 0.0, 0.0],
-            [-2, np.pi * 1.2, 0.01, 0.2, 0.0, -0.1 * np.pi],
-        ])
+        state_lst = np.array(
+            [
+                [0.05, np.pi * 0.95, np.pi / 2, -0.01, 0.01 * np.pi, 0.0],
+                [-0.01, np.pi * 1.1, -np.pi * 0.1, 0.1, 0.0, -0.2 * np.pi],
+                [0.2, np.pi * 0.5, np.pi / 8, 0.01, 0.0, 0.0],
+                [0.0, np.pi, np.pi, 0.0, 0.0, 0.0],
+                [-2, np.pi * 1.2, 0.01, 0.2, 0.0, -0.1 * np.pi],
+            ]
+        )
         result_lst = []
         context = diagram.CreateDefaultContext()
         for state in state_lst:
             context.SetContinuousState(state)
             result_lst.append(
-                diagram.EvalTimeDerivatives(context).CopyToVector())
+                diagram.EvalTimeDerivatives(context).CopyToVector()
+            )
         result = np.array(result_lst)
-        target_derivatives = np.array([
-            [
-                -1.00000000e-02,
-                3.14159265e-02,
-                0.00000000e00,
-                -4.68965989e02,
-                -4.64727356e02,
-                5.28401564e02,
-            ],
-            [
-                1.00000000e-01,
-                0.00000000e00,
-                -6.28318531e-01,
-                -9.02354495e02,
-                -7.77737857e02,
-                9.40419695e02,
-            ],
+        target_derivatives = np.array(
             [
-                1.00000000e-02,
-                0.00000000e00,
-                0.00000000e00,
-                -3.32561210e02,
-                9.27487605e01,
-                1.29268844e02,
-            ],
-            [
-                0.00000000e00,
-                0.00000000e00,
-                0.00000000e00,
-                -2.40275702e-15,
-                -2.40275702e-15,
-                0.00000000e00,
-            ],
-            [
-                2.00000000e-01,
-                0.00000000e00,
-                -3.14159265e-01,
-                -5.40431505e02,
-                -4.34708484e02,
-                4.28196374e02,
-            ],
-        ])
+                [
+                    -1.00000000e-02,
+                    3.14159265e-02,
+                    0.00000000e00,
+                    -4.68965989e02,
+                    -4.64727356e02,
+                    5.28401564e02,
+                ],
+                [
+                    1.00000000e-01,
+                    0.00000000e00,
+                    -6.28318531e-01,
+                    -9.02354495e02,
+                    -7.77737857e02,
+                    9.40419695e02,
+                ],
+                [
+                    1.00000000e-02,
+                    0.00000000e00,
+                    0.00000000e00,
+                    -3.32561210e02,
+                    9.27487605e01,
+                    1.29268844e02,
+                ],
+                [
+                    0.00000000e00,
+                    0.00000000e00,
+                    0.00000000e00,
+                    -2.40275702e-15,
+                    -2.40275702e-15,
+                    0.00000000e00,
+                ],
+                [
+                    2.00000000e-01,
+                    0.00000000e00,
+                    -3.14159265e-01,
+                    -5.40431505e02,
+                    -4.34708484e02,
+                    4.28196374e02,
+                ],
+            ]
+        )
         np.testing.assert_array_almost_equal(
             result,
             target_derivatives,
             decimal=4,
             err_msg="the dynamics for the double pendulum LQR do not match",
         )
```

### Comparing `underactuated-2023.3.2/underactuated/exercises/contact/test_compass_gait_limit_cycle.py` & `underactuated-2023.4.17/underactuated/exercises/contact/test_compass_gait_limit_cycle.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,204 +1,223 @@
 import unittest
+
+import numpy as np
 import timeout_decorator
 from gradescope_utils.autograder_utils.decorators import weight
-import numpy as np
 
 
 class TestCompassGaitLimitCycle(unittest.TestCase):
-
     def __init__(self, test_name, notebook_locals):
         super().__init__(test_name)
         self.notebook_locals = notebook_locals
 
     # starts by testing the constraints we already implemented
     # but gives zero points for each test
 
     @weight(0)
-    @timeout_decorator.timeout(3.)
+    @timeout_decorator.timeout(3.0)
     def test_time_intervals(self):
         """Time intervals are within bounds"""
         # retrieve variables from notebook
-        T = self.notebook_locals['T']
-        h_opt = self.notebook_locals['h_opt']
-        h_min = self.notebook_locals['h_min']
-        h_max = self.notebook_locals['h_max']
+        T = self.notebook_locals["T"]
+        h_opt = self.notebook_locals["h_opt"]
+        h_min = self.notebook_locals["h_min"]
+        h_max = self.notebook_locals["h_max"]
 
         # check one per time
         tol = 1e-4
         for t in range(T):
-            self.assertTrue(h_opt[t] >= h_min - tol,
-                            msg=f'Time interval lower bound violated at time '
-                            + f'step {t}.')
-            self.assertTrue(h_opt[t] <= h_max + tol,
-                            msg=f'Time interval upper bound violated at time '
-                            + f'step {t}.')
+            self.assertTrue(
+                h_opt[t] >= h_min - tol,
+                msg=f"Time interval lower bound violated at time "
+                + f"step {t}.",
+            )
+            self.assertTrue(
+                h_opt[t] <= h_max + tol,
+                msg=f"Time interval upper bound violated at time "
+                + f"step {t}.",
+            )
 
     @weight(0)
-    @timeout_decorator.timeout(3.)
+    @timeout_decorator.timeout(3.0)
     def test_dynamic_feasibility(self):
         """Implicit Euler equations are verified"""
         # retrieve variables from notebook
-        T = self.notebook_locals['T']
-        h = self.notebook_locals['h_opt']
-        q = self.notebook_locals['q_opt']
-        qd = self.notebook_locals['qd_opt']
-        qdd = self.notebook_locals['qdd_opt']
-        f = self.notebook_locals['f_opt']
-        manipulator_equations = self.notebook_locals['manipulator_equations']
+        T = self.notebook_locals["T"]
+        h = self.notebook_locals["h_opt"]
+        q = self.notebook_locals["q_opt"]
+        qd = self.notebook_locals["qd_opt"]
+        qdd = self.notebook_locals["qdd_opt"]
+        f = self.notebook_locals["f_opt"]
+        manipulator_equations = self.notebook_locals["manipulator_equations"]
 
         # link configurations, velocities, accelerations using implicit Euler
         for t in range(T):
             np.testing.assert_allclose(
                 q[t + 1],
                 q[t] + h[t] * qd[t + 1],
                 atol=1e-5,
                 rtol=1e-5,
-                err_msg='Configurations q and velocities qd do not verify '
-                + f'the Implicit Euler rule at time step {t}.')
+                err_msg="Configurations q and velocities qd do not verify "
+                + f"the Implicit Euler rule at time step {t}.",
+            )
             np.testing.assert_allclose(
                 qd[t + 1],
                 qd[t] + h[t] * qdd[t],
                 atol=1e-5,
                 rtol=1e-5,
-                err_msg='Velocities qd and accelerations qdd do not verify '
-                + f'the Implicit Euler rule at time step {t}.')
+                err_msg="Velocities qd and accelerations qdd do not verify "
+                + f"the Implicit Euler rule at time step {t}.",
+            )
             vars = np.concatenate((q[t + 1], qd[t + 1], qdd[t], f[t]))
             manipulator_equations_violation = manipulator_equations(vars)
             np.testing.assert_allclose(
                 manipulator_equations_violation,
                 np.zeros(q.shape[1]),
                 atol=1e-5,
                 rtol=1e-5,
-                err_msg='Manipulator equations are not verified at time '
-                + f'step {t}.')
+                err_msg="Manipulator equations are not verified at time "
+                + f"step {t}.",
+            )
 
     @weight(0)
-    @timeout_decorator.timeout(3.)
+    @timeout_decorator.timeout(3.0)
     def test_impulsive_collision(self):
         """Impulsive collision is verified at the heel strike"""
         # retrieve variables from notebook
-        q = self.notebook_locals['q_opt']
-        qd = self.notebook_locals['qd_opt']
-        qd_post = self.notebook_locals['qd_post_opt']
-        imp = self.notebook_locals['imp_opt']
+        q = self.notebook_locals["q_opt"]
+        qd = self.notebook_locals["qd_opt"]
+        qd_post = self.notebook_locals["qd_post_opt"]
+        imp = self.notebook_locals["imp_opt"]
         reset_velocity_heelstrike = self.notebook_locals[
-            'reset_velocity_heelstrike']
+            "reset_velocity_heelstrike"
+        ]
 
         # link pre and post impact velocities
         vars = np.concatenate((q[-1], qd[-1], qd_post, imp))
         reset_velocity_heelstrike_violation = reset_velocity_heelstrike(vars)
         np.testing.assert_allclose(
             reset_velocity_heelstrike_violation,
             np.zeros(q.shape[1] + imp.size),
             atol=1e-5,
             rtol=1e-5,
-            err_msg='Impulsive collision equations are not verified.')
+            err_msg="Impulsive collision equations are not verified.",
+        )
 
     @weight(0)
-    @timeout_decorator.timeout(3.)
+    @timeout_decorator.timeout(3.0)
     def test_periodicity(self):
         """Periodicity of the walking gait"""
         # retrieve variables from notebook
-        q = self.notebook_locals['q_opt']
-        qd = self.notebook_locals['qd_opt']
-        qd_post = self.notebook_locals['qd_post_opt']
+        q = self.notebook_locals["q_opt"]
+        qd = self.notebook_locals["qd_opt"]
+        qd_post = self.notebook_locals["qd_post_opt"]
 
         # periodicity of the configuration
         np.testing.assert_allclose(
             q[0],
             -q[-1],
             atol=1e-5,
             rtol=1e-5,
-            err_msg='Configuration vector q does not verify periodicity '
-            + 'conditions.')
+            err_msg="Configuration vector q does not verify periodicity "
+            + "conditions.",
+        )
 
         # periodicity of the  velocities
         np.testing.assert_allclose(
             qd[0],
             np.array([0, 0, qd_post[2] + qd_post[3], -qd_post[3]]),
             atol=1e-5,
             rtol=1e-5,
-            err_msg='Velocity vector qd does not verify periodicity '
-            + 'conditions.')
+            err_msg="Velocity vector qd does not verify periodicity "
+            + "conditions.",
+        )
 
     # tests constraints implemented by the students
     # does not use the same expressions that must be used in the constraint
     # e.g. checks that a linear constraint is verified by evaluating a nonlinear
     # function
 
     @weight(3)
-    @timeout_decorator.timeout(3.)
+    @timeout_decorator.timeout(3.0)
     def test_stance_foot_on_ground(self):
         """Stance foot on the ground for all times"""
         # retrieve variables from notebook
-        T = self.notebook_locals['T']
-        q = self.notebook_locals['q_opt']
+        T = self.notebook_locals["T"]
+        q = self.notebook_locals["q_opt"]
         for t in range(T + 1):
             self.assertAlmostEqual(
                 np.linalg.norm(q[t, :2]),
                 0,
-                msg=f'Stance foot is not on the ground at time step {t}.')
+                msg=f"Stance foot is not on the ground at time step {t}.",
+            )
 
     @weight(2)
-    @timeout_decorator.timeout(3.)
+    @timeout_decorator.timeout(3.0)
     def test_swing_foot_on_ground(self):
         """Swing foot on the ground at time zero"""
         # retrieve variables from notebook
-        q = self.notebook_locals['q_opt']
-        swing_foot_height = self.notebook_locals['swing_foot_height']
+        q = self.notebook_locals["q_opt"]
+        swing_foot_height = self.notebook_locals["swing_foot_height"]
         self.assertAlmostEqual(
             swing_foot_height(q[0])[0],
             0,
-            msg='Swing foot is not on the ground at time zero.')
+            msg="Swing foot is not on the ground at time zero.",
+        )
 
     @weight(3)
-    @timeout_decorator.timeout(3.)
+    @timeout_decorator.timeout(3.0)
     def test_no_penetration(self):
         """No penetration of the swing foot in the ground for all times"""
         # retrieve variables from notebook
-        T = self.notebook_locals['T']
-        q = self.notebook_locals['q_opt']
-        swing_foot_height = self.notebook_locals['swing_foot_height']
+        T = self.notebook_locals["T"]
+        q = self.notebook_locals["q_opt"]
+        swing_foot_height = self.notebook_locals["swing_foot_height"]
         tol = 1e-4
         for t in range(T + 1):
             self.assertGreater(
                 swing_foot_height(q[t])[0],
                 -tol,
-                msg=f'Swing foot in penetration with ground at time step {t}.')
+                msg=f"Swing foot in penetration with ground at time step {t}.",
+            )
 
     @weight(3)
-    @timeout_decorator.timeout(3.)
+    @timeout_decorator.timeout(3.0)
     def test_stance_foot_friction(self):
         """Stance-foot contact force in friction cone for all times"""
         # retrieve variables from notebook
-        T = self.notebook_locals['T']
-        friction = self.notebook_locals['friction']
-        f = self.notebook_locals['f_opt']
+        T = self.notebook_locals["T"]
+        friction = self.notebook_locals["friction"]
+        f = self.notebook_locals["f_opt"]
         tol = 1e-4
         for t in range(T):
             self.assertGreater(
                 f[t, 1],
                 -tol,
-                msg='Stance-foot normal contact force is negative at time '
-                + f'step {t}.')
+                msg="Stance-foot normal contact force is negative at time "
+                + f"step {t}.",
+            )
             self.assertLess(
                 np.abs(f[t, 0]),
                 friction * f[t, 1] + tol,
-                msg='Stance-foot contact force outside friction cone at time '
-                + f'step {t}.')
+                msg="Stance-foot contact force outside friction cone at time "
+                + f"step {t}.",
+            )
 
     @weight(2)
-    @timeout_decorator.timeout(3.)
+    @timeout_decorator.timeout(3.0)
     def test_swing_foot_friction(self):
         """Swing-foot impulse in friction cone"""
         # retrieve variables from notebook
-        friction = self.notebook_locals['friction']
-        imp = self.notebook_locals['imp_opt']
+        friction = self.notebook_locals["friction"]
+        imp = self.notebook_locals["imp_opt"]
         tol = 1e-4
         self.assertGreater(
             imp[1],
             -tol,
-            msg='Normal heel-strike impulse is negative at time step {t}.')
-        self.assertLess(np.abs(imp[0]),
-                        friction * imp[1] + tol,
-                        msg='Heel-strike impulse outside friction cone')
+            msg="Normal heel-strike impulse is negative at time step {t}.",
+        )
+        self.assertLess(
+            np.abs(imp[0]),
+            friction * imp[1] + tol,
+            msg="Heel-strike impulse outside friction cone",
+        )
```

### Comparing `underactuated-2023.3.2/underactuated/exercises/dp/minimum_time_utils.py` & `underactuated-2023.4.17/underactuated/exercises/dp/minimum_time_utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,190 +1,181 @@
 import matplotlib.animation as ani
 import matplotlib.pyplot as plt
 import numpy as np
-from IPython.display import HTML
 from matplotlib import cm
-from mpl_toolkits.mplot3d import Axes3D
+
 # pydrake imports
-from pydrake.all import (DiagramBuilder, DynamicProgrammingOptions,
-                         FittedValueIteration, LinearSystem, LogVectorOutput,
-                         Simulator, VectorSystem)
 
 
 def create_animation(J_grid, pi_grid, mesh):
     # initialize figure for animation plus misc settings
     fig, ax = plt.subplots(1, 2, figsize=(12, 5))
     plt.tight_layout()
-    ax[0].axis('off')
-    ax[1].axis('off')
+    ax[0].axis("off")
+    ax[1].axis("off")
 
     # cost-to-go plot and policy plots
     # overwrites the subplots axes
-    ax[0] = fig.add_subplot(121, projection='3d')
-    ax[1] = fig.add_subplot(122, projection='3d')
-    ax[0].set_title(r'Optimal cost to go   $J^*(\mathbf{x})$')
-    ax[1].set_title(r'Optimal policy   $\pi^*(\mathbf{x})$')
+    ax[0] = fig.add_subplot(121, projection="3d")
+    ax[1] = fig.add_subplot(122, projection="3d")
+    ax[0].set_title(r"Optimal cost to go   $J^*(\mathbf{x})$")
+    ax[1].set_title(r"Optimal policy   $\pi^*(\mathbf{x})$")
     for axi in ax:
-        axi.set_xlabel(r'$q$')
-        axi.set_ylabel(r'$\dot q$')
+        axi.set_xlabel(r"$q$")
+        axi.set_ylabel(r"$\dot q$")
 
     # helper function for the surface plot
-    Q, Qdot = np.meshgrid(mesh['q_grid'], mesh['qdot_grid'])
+    Q, Qdot = np.meshgrid(mesh["q_grid"], mesh["qdot_grid"])
 
     def plot_surf(ax, Z):
         return ax.plot_surface(Q, Qdot, Z.T, rstride=1, cstride=1, cmap=cm.jet)
 
     # first frame of the animation
     J_surf = [plot_surf(ax[0], J_grid[:, :, 0])]
     pi_surf = [plot_surf(ax[1], pi_grid[:, :, 0])]
 
     # video parameters
     frames = 40  # total number of frames
     duration = 10  # seconds
     interval = duration / (frames - 1) * 1000  # milliseconds
 
     # initialize title to be modified in the callback
-    title = fig.text(.5,
-                     .95,
-                     "",
-                     fontsize='x-large',
-                     bbox={'facecolor': 'w'},
-                     ha='center')
+    title = fig.text(
+        0.5, 0.95, "", fontsize="x-large", bbox={"facecolor": "w"}, ha="center"
+    )
 
     # callback function for the animation
     def update_surf(frame, J_grid, J_surf, pi_grid, pi_surf):
-
         # iteration to plot, - 1 for base zero
         iters = J_grid.shape[2]
         i = int(frame * (iters - 1) / (frames - 1))
 
         # update cost-to-go and policy
         J_surf[0].remove()
         pi_surf[0].remove()
         J_surf[0] = plot_surf(ax[0], J_grid[:, :, i])
         pi_surf[0] = plot_surf(ax[1], pi_grid[:, :, i])
 
         # update title with current iteration
         # use base 1 as above
-        title.set_text(f'Value iteration {i+1}')
+        title.set_text(f"Value iteration {i+1}")
 
     # create animation
-    animate = ani.FuncAnimation(fig,
-                                update_surf,
-                                frames=frames,
-                                interval=interval,
-                                fargs=(J_grid, J_surf, pi_grid, pi_surf))
+    animate = ani.FuncAnimation(
+        fig,
+        update_surf,
+        frames=frames,
+        interval=interval,
+        fargs=(J_grid, J_surf, pi_grid, pi_surf),
+    )
 
     # play video
     plt.close()  # close any open figure
     return animate
 
 
 # function that plots the trajectory of the
 # double integrator in state space (q_sim vs qdot_sim)
 def plot_state_trajectory(q_sim, qdot_sim):
-
     # draw a white dot for the initial conditions
-    plt.scatter(q_sim[0],
-                qdot_sim[0],
-                s=100,
-                edgecolor='k',
-                c='w',
-                zorder=3,
-                label=r'$\mathbf{x}(0)$')
+    plt.scatter(
+        q_sim[0],
+        qdot_sim[0],
+        s=100,
+        edgecolor="k",
+        c="w",
+        zorder=3,
+        label=r"$\mathbf{x}(0)$",
+    )
 
     # black line for the trajectory in time
-    plt.plot(q_sim, qdot_sim, color='k', linewidth=2, label=r'$\mathbf{x}(t)$')
+    plt.plot(q_sim, qdot_sim, color="k", linewidth=2, label=r"$\mathbf{x}(t)$")
 
     # misc
-    plt.xlabel(r'$q$')
-    plt.ylabel(r'$\dot q$')
+    plt.xlabel(r"$q$")
+    plt.ylabel(r"$\dot q$")
     plt.legend()
 
 
 # helper function for plot_policy that evaluates
 # the controller output at a given state
 def evaluate_controller(controller, q, qdot):
-
     # get context and set system output (= system state)
     context = controller.CreateDefaultContext()
     controller.get_input_port(0).FixValue(context, (q, qdot))
 
     # compute input for the double integrator
     u = controller.get_output_port(0).Eval(context)[0]
 
     return u
 
 
 # function that produces a level plot
 # the policy generated by the passed controller
 # it used the grid defined by q_grid and qdot_grid
 def plot_policy(q_grid, qdot_grid, controller):
-
     # evaluate the policy on the grid
     Pi_grid = np.array(
-        [[evaluate_controller(controller, q, qdot)
-          for qdot in qdot_grid]
-         for q in q_grid])
+        [
+            [evaluate_controller(controller, q, qdot) for qdot in qdot_grid]
+            for q in q_grid
+        ]
+    )
 
     # level plot the level function
     # note the transpose to align the policy to the grid
     plt.contourf(*np.meshgrid(q_grid, qdot_grid), Pi_grid.T, cmap=cm.jet)
 
     # add a bar with the color scale on the right
-    plt.colorbar(label=r'$\pi^*(\mathbf{x})$')
+    plt.colorbar(label=r"$\pi^*(\mathbf{x})$")
 
 
 # function that plots the control signal
 # u_sim as a function of the time vector t
 def plot_input(u_sim, t_sim, u_lim):
-
     # plot the bounds for the control signal
-    plt.plot(t_sim, [u_lim[0]] * len(t_sim),
-             c='r',
-             linestyle='--',
-             label='Input limits')
-    plt.plot(t_sim, [u_lim[1]] * len(t_sim), c='r', linestyle='--')
+    plt.plot(
+        t_sim,
+        [u_lim[0]] * len(t_sim),
+        c="r",
+        linestyle="--",
+        label="Input limits",
+    )
+    plt.plot(t_sim, [u_lim[1]] * len(t_sim), c="r", linestyle="--")
 
     # plot the control signal
-    plt.plot(t_sim, u_sim, label='Input from simulation')
+    plt.plot(t_sim, u_sim, label="Input from simulation")
 
     # misc
-    plt.xlabel(r'$t$')
-    plt.ylabel(r'$u$')
+    plt.xlabel(r"$t$")
+    plt.ylabel(r"$u$")
     plt.xlim(min(t_sim), max(t_sim))
     plt.grid(True)
     plt.legend(loc=1)
 
 
 # overall plot function for the state trajectory,
 # controller policy, and input signal
-def simulate_and_plot(q0,
-                      qdot0,
-                      sim_time,
-                      controller,
-                      u_lim,
-                      nq=201,
-                      nqdot=201,
-                      simulate=None):
-
+def simulate_and_plot(
+    q0, qdot0, sim_time, controller, u_lim, nq=201, nqdot=201, simulate=None
+):
     # get trajectories
     q_sim, qdot_sim, u_sim, t_sim = simulate(q0, qdot0, sim_time, controller)
 
     # state figure
     plt.figure()
     plot_state_trajectory(q_sim, qdot_sim)
 
     # plot policy only in a square region that
     # contains tightly the trajectory
 
     # helper function that computes upper and
     # lower bounds, with a small frame, for the
     # passed signal s
-    def frame_signal(s, frame=.1):
+    def frame_signal(s, frame=0.1):
         ds = (max(s) - min(s)) * frame
         return [min(s) - ds, max(s) + ds]
 
     # regrid state space for policy plot
     # this grid must be much finer than the
     # one used for value iteration
     q_grid = np.linspace(*frame_signal(q_sim), nq)
```

### Comparing `underactuated-2023.3.2/underactuated/exercises/dp/test_lp_dp.py` & `underactuated-2023.4.17/underactuated/exercises/dp/test_lp_dp.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 import unittest
+
 import numpy as np
 import timeout_decorator
 from gradescope_utils.autograder_utils.decorators import weight
+
 from underactuated import FindResource
 
 
 class Testlpdp(unittest.TestCase):
-
     def __init__(self, test_name, notebook_locals):
         super().__init__(test_name)
         self.notebook_locals = notebook_locals
 
     @weight(6)
-    @timeout_decorator.timeout(1.)
+    @timeout_decorator.timeout(1.0)
     def test_J_from_lp(self):
         """Test optimal cost-to-go from Linear Program"""
         # note: all prints here go to the output item in the json file
-        J_value = self.notebook_locals['J_value']
+        J_value = self.notebook_locals["J_value"]
 
         J = np.load(FindResource("exercises/dp/J.npy"))
 
         diff = np.abs(J - J_value)
 
         self.assertTrue(
             (diff <= 1e-6).all(),
-            msg='|J - J*| > 1e-6',
+            msg="|J - J*| > 1e-6",
         )
```

### Comparing `underactuated-2023.3.2/underactuated/exercises/dp/test_pendulum_cvi.py` & `underactuated-2023.4.17/underactuated/exercises/dp/test_pendulum_cvi.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,190 +1,253 @@
 import unittest
+
+import numpy as np
 import timeout_decorator
 from gradescope_utils.autograder_utils.decorators import weight
-import numpy as np
-from pydrake.all import (DiagramBuilder, SceneGraph, Simulator, LeafSystem,
-                         DiagramBuilder, SceneGraph, ZeroOrderHold)
+from pydrake.all import (
+    DiagramBuilder,
+    LeafSystem,
+    SceneGraph,
+    Simulator,
+    ZeroOrderHold,
+)
 from pydrake.examples import PendulumGeometry, PendulumPlant
 
 
 class TestPendulumCVI(unittest.TestCase):
-
     def __init__(self, test_name, notebook_locals):
         super().__init__(test_name)
         self.notebook_locals = notebook_locals
 
     @weight(2)
-    @timeout_decorator.timeout(20.)
+    @timeout_decorator.timeout(20.0)
     def test_state_cost(self):
         """Test compute state cost"""
         # note: all prints here go to the output item in the json file
 
         # the loss must be close to the correct value
-        compute_state_cost = self.notebook_locals['compute_state_cost']
+        compute_state_cost = self.notebook_locals["compute_state_cost"]
         tol = 1e-8
 
         # intentionally different values than for cartpole
         target_state = np.array([0, np.pi]).reshape(-1, 1)
-        Q = np.diag([1., 20.])
+        Q = np.diag([1.0, 20.0])
 
         self.assertLessEqual(
             compute_state_cost(Q, target_state, target_state),
             tol,
-            msg=('target state cost is '
-                 f'{compute_state_cost(Q, target_state, target_state)}'
-                 ' which is more than tolerance {tol}'))
-
-        cost = compute_state_cost(Q, target_state,
-                                  np.array([0, 0]).reshape(-1, 1))
-        target = np.pi**2 * 20.
-        self.assertLessEqual(np.abs(cost - target),
-                             tol,
-                             msg='Cost at state = 0 is incorrect')
+            msg=(
+                "target state cost is "
+                f"{compute_state_cost(Q, target_state, target_state)}"
+                " which is more than tolerance {tol}"
+            ),
+        )
+
+        cost = compute_state_cost(
+            Q, target_state, np.array([0, 0]).reshape(-1, 1)
+        )
+        target = np.pi**2 * 20.0
+        self.assertLessEqual(
+            np.abs(cost - target), tol, msg="Cost at state = 0 is incorrect"
+        )
 
         state1 = [
-            5.89375203, 5.72132364, 2.07924145, -25.58778621, 4.84281921,
-            -19.20542969, -2.35612669
+            5.89375203,
+            5.72132364,
+            2.07924145,
+            -25.58778621,
+            4.84281921,
+            -19.20542969,
+            -2.35612669,
         ]
         state2 = [
-            -35.69553553, 24.11618679, -0.85857409, 3.61505439, -3.28412933,
-            26.96593774, -0.81457745
+            -35.69553553,
+            24.11618679,
+            -0.85857409,
+            3.61505439,
+            -3.28412933,
+            26.96593774,
+            -0.81457745,
         ]
         test_states = np.array([state1, state2])
-        result_true = np.array([
-            30201.18682396, 8831.40552794, 324.34992454, 659.21812345,
-            849.25095811, 11720.8369055, 318.57697075
-        ])
+        result_true = np.array(
+            [
+                30201.18682396,
+                8831.40552794,
+                324.34992454,
+                659.21812345,
+                849.25095811,
+                11720.8369055,
+                318.57697075,
+            ]
+        )
         result_tested = compute_state_cost(Q, target_state, test_states)
         for i in range(result_true.shape[0]):
-            self.assertLessEqual(np.abs(result_true[i] - result_tested[i]), tol,
-                                 f"failed on random state number {i}")
+            self.assertLessEqual(
+                np.abs(result_true[i] - result_tested[i]),
+                tol,
+                f"failed on random state number {i}",
+            )
 
     @weight(2)
-    @timeout_decorator.timeout(20.)
+    @timeout_decorator.timeout(20.0)
     def test_compute_u_star(self):
         """Test compute u_star"""
         # note: all prints here go to the output item in the json file
-        compute_u_star = self.notebook_locals['compute_u_star']
+        compute_u_star = self.notebook_locals["compute_u_star"]
 
         R_diag = np.array([1.5])
 
         dJdX = np.array(
-            [[8.455e+00, -2.330e+00, 1.650e-01, 2.040e+00, -3.945e+00],
-             [1.000e-02, -5.000e-03, -8.775e+00, 5.090e+00, 3.000e+00]])
-        dstate_dynamics_du = np.array([[[-0.785, 3.86, -6.79, 3.51, 5.265]],
-                                       [[1.35, -4.855, 5.24, 6.095, -0.26]]])
+            [
+                [8.455e00, -2.330e00, 1.650e-01, 2.040e00, -3.945e00],
+                [1.000e-02, -5.000e-03, -8.775e00, 5.090e00, 3.000e00],
+            ]
+        )
+        dstate_dynamics_du = np.array(
+            [
+                [[-0.785, 3.86, -6.79, 3.51, 5.265]],
+                [[1.35, -4.855, 5.24, 6.095, -0.26]],
+            ]
+        )
         u_star_true = np.array(
-            [[2.20789167, 2.98984167, 15.70045, -12.72798333, 7.183475]])
+            [[2.20789167, 2.98984167, 15.70045, -12.72798333, 7.183475]]
+        )
         u_star_test = compute_u_star(R_diag, dJdX, dstate_dynamics_du)
-        self.assertTrue(u_star_true.shape == u_star_test.shape,
-                        (f"output of compute_u_star is incorrect. Expected "
-                         f"{u_star_true.shape} got {u_star_test.shape}"))
+        self.assertTrue(
+            u_star_true.shape == u_star_test.shape,
+            (
+                f"output of compute_u_star is incorrect. Expected "
+                f"{u_star_true.shape} got {u_star_test.shape}"
+            ),
+        )
 
         for i in range(u_star_test.shape[0]):
             for j in range(u_star_test.shape[1]):
                 self.assertLessEqual(
-                    np.abs(u_star_test[i, j] - u_star_true[i, j]), 1e-8,
-                    f"incorrect u_star at index {i} for test state {j}")
+                    np.abs(u_star_test[i, j] - u_star_true[i, j]),
+                    1e-8,
+                    f"incorrect u_star at index {i} for test state {j}",
+                )
 
     @weight(6)
-    @timeout_decorator.timeout(600.)
+    @timeout_decorator.timeout(600.0)
     def test_policy(self):
         """Test policy"""
-        value_mlp = self.notebook_locals['value_mlp']
-        input_limits = self.notebook_locals['input_limits']
-        value_mlp_context = self.notebook_locals['value_mlp_context']
-        R_diag = self.notebook_locals['R_diag']
-        compute_u_star = self.notebook_locals['compute_u_star']
-        simulator = self.build_pendulum_simulator(value_mlp,
-                                                  value_mlp_context,
-                                                  R_diag,
-                                                  compute_u_star,
-                                                  input_limits=input_limits)
+        value_mlp = self.notebook_locals["value_mlp"]
+        input_limits = self.notebook_locals["input_limits"]
+        value_mlp_context = self.notebook_locals["value_mlp_context"]
+        R_diag = self.notebook_locals["R_diag"]
+        compute_u_star = self.notebook_locals["compute_u_star"]
+        simulator = self.build_pendulum_simulator(
+            value_mlp,
+            value_mlp_context,
+            R_diag,
+            compute_u_star,
+            input_limits=input_limits,
+        )
         simulator_context = simulator.get_mutable_context()
-        simulator.set_target_realtime_rate(0.)
+        simulator.set_target_realtime_rate(0.0)
         num_sim = 20
         np.random.seed(14)
         errors = []
         for i in range(num_sim):
             duration = 5.0
-            simulator_context.SetTime(0.)
+            simulator_context.SetTime(0.0)
             simulator_context.SetContinuousState(
-                np.array([2 * np.pi * np.random.rand(), 0]))
+                np.array([2 * np.pi * np.random.rand(), 0])
+            )
             simulator.Initialize()
             simulator.AdvanceTo(duration)
-            final_state_vector = simulator_context.get_continuous_state(
-            ).get_vector().CopyToVector()
+            final_state_vector = (
+                simulator_context.get_continuous_state()
+                .get_vector()
+                .CopyToVector()
+            )
             theta_wrapped = np.arccos(np.cos(final_state_vector[0]))
             errors.append(np.abs(theta_wrapped - np.pi))
 
         num_passed = 0
         for e in errors:
             # check if theta is close to pi
             if np.abs(e) <= 1e-1:
                 num_passed += 1
         frac = 0.7
         threshold = int(frac * num_sim)
         self.assertGreaterEqual(
-            num_passed, threshold,
-            (f"Only passed {num_passed/num_sim * 100}% of initial"
-             f" configurations. Need to pass {frac*100}%"))
+            num_passed,
+            threshold,
+            (
+                f"Only passed {num_passed/num_sim * 100}% of initial"
+                f" configurations. Need to pass {frac*100}%"
+            ),
+        )
 
     # initialize controller and plant
-    def build_pendulum_simulator(self,
-                                 value_mlp,
-                                 value_mlp_context,
-                                 R_diag,
-                                 compute_u_star,
-                                 input_limits=None):
+    def build_pendulum_simulator(
+        self,
+        value_mlp,
+        value_mlp_context,
+        R_diag,
+        compute_u_star,
+        input_limits=None,
+    ):
         time_step = 0.01
         closed_loop_builder = DiagramBuilder()
         plant_cl, scene_graph_cl = closed_loop_builder.AddSystem(
-            PendulumPlant()), closed_loop_builder.AddSystem(SceneGraph())
+            PendulumPlant()
+        ), closed_loop_builder.AddSystem(SceneGraph())
 
         controller_sys = ContinuousFittedValueIterationPolicyComputeUStar(
             plant_cl,
             value_mlp,
             value_mlp_context,
             R_diag,
             compute_u_star,
-            input_limits=input_limits)
+            input_limits=input_limits,
+        )
 
-        PendulumGeometry.AddToBuilder(closed_loop_builder,
-                                      plant_cl.get_state_output_port(),
-                                      scene_graph_cl)
+        PendulumGeometry.AddToBuilder(
+            closed_loop_builder,
+            plant_cl.get_state_output_port(),
+            scene_graph_cl,
+        )
 
         controller = closed_loop_builder.AddSystem(controller_sys)
         # we assume a zero-order hold between time steps
         zoh = closed_loop_builder.AddSystem(ZeroOrderHold(time_step, 1))
 
         # wire all the systems together
-        closed_loop_builder.Connect(plant_cl.get_output_port(),
-                                    controller.get_input_port())
-        closed_loop_builder.Connect(controller.get_output_port(),
-                                    zoh.get_input_port())
-        closed_loop_builder.Connect(zoh.get_output_port(),
-                                    plant_cl.get_input_port())
+        closed_loop_builder.Connect(
+            plant_cl.get_output_port(), controller.get_input_port()
+        )
+        closed_loop_builder.Connect(
+            controller.get_output_port(), zoh.get_input_port()
+        )
+        closed_loop_builder.Connect(
+            zoh.get_output_port(), plant_cl.get_input_port()
+        )
 
         diagram_closed_loop = closed_loop_builder.Build()
 
         simulator = Simulator(diagram_closed_loop)
         return simulator
 
 
 class ContinuousFittedValueIterationPolicyComputeUStar(LeafSystem):
-
-    def __init__(self,
-                 plant,
-                 value_mlp,
-                 value_mlp_context,
-                 R_diag,
-                 compute_u_star,
-                 input_port_index=0,
-                 input_limits=None):
+    def __init__(
+        self,
+        plant,
+        value_mlp,
+        value_mlp_context,
+        R_diag,
+        compute_u_star,
+        input_port_index=0,
+        input_limits=None,
+    ):
         LeafSystem.__init__(self)
 
         self.num_plant_states = value_mlp.get_input_port().size()
         self._plant = plant
         self._plant_context = plant.CreateDefaultContext()
 
         self.value_mlp = value_mlp
@@ -195,39 +258,50 @@
         self.compute_u_star = compute_u_star
 
         self.Rinv = 1 / R_diag
         self.R_diag = R_diag
         self.input_limits = input_limits
         self.DeclareVectorInputPort("plant_state", self.num_plant_states)
         self._plant_input_port = self._plant.get_input_port(input_port_index)
-        self.DeclareVectorOutputPort("output", self._plant_input_port.size(),
-                                     self.CalcOutput)
+        self.DeclareVectorOutputPort(
+            "output", self._plant_input_port.size(), self.CalcOutput
+        )
 
     def CalcOutput(self, context, output):
         num_inputs = self._plant_input_port.size()
         u = np.zeros(num_inputs)
         plant_state = self.get_input_port().Eval(context)
 
-        self.value_mlp.BatchOutput(self.value_mlp_context,
-                                   np.atleast_2d(plant_state).T, self.J,
-                                   self.dJdX)
+        self.value_mlp.BatchOutput(
+            self.value_mlp_context,
+            np.atleast_2d(plant_state).T,
+            self.J,
+            self.dJdX,
+        )
 
         self._plant_context.SetContinuousState(plant_state)
         self._plant_input_port.FixValue(self._plant_context, u)
         state_dynamics_x = self._plant.EvalTimeDerivatives(
-            self._plant_context).CopyToVector()
+            self._plant_context
+        ).CopyToVector()
 
         dstate_dynamics_du = np.empty((self.num_plant_states, num_inputs, 1))
         for i in range(num_inputs):
             u[i] = 1
             self._plant_input_port.FixValue(self._plant_context, u)
-            dstate_dynamics_du[:, :, i] = (self._plant.EvalTimeDerivatives(
-                self._plant_context).CopyToVector() - state_dynamics_x).reshape(
-                    -1, 1)
+            dstate_dynamics_du[:, :, i] = (
+                self._plant.EvalTimeDerivatives(
+                    self._plant_context
+                ).CopyToVector()
+                - state_dynamics_x
+            ).reshape(-1, 1)
             u[i] = 0
 
-        u_star = self.compute_u_star(self.R_diag, self.dJdX,
-                                     dstate_dynamics_du)[:, 0]
+        u_star = self.compute_u_star(
+            self.R_diag, self.dJdX, dstate_dynamics_du
+        )[:, 0]
         if self.input_limits is not None:
-            u_star = np.clip(u_star, self.input_limits[0], self.input_limits[1])
+            u_star = np.clip(
+                u_star, self.input_limits[0], self.input_limits[1]
+            )
         for i in range(num_inputs):
             output.SetAtIndex(i, u_star[i])
```

### Comparing `underactuated-2023.3.2/underactuated/exercises/grader.py` & `underactuated-2023.4.17/underactuated/exercises/grader.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,123 +1,140 @@
-import unittest
-from gradescope_utils.autograder_utils.json_test_runner import JSONTestRunner
 import json
+import os
+import unittest
 from runpy import run_path
+
 import nbformat
+from gradescope_utils.autograder_utils.json_test_runner import JSONTestRunner
 from nbconvert import PythonExporter
-import os
 
 grader_throws = False
 
 
 def set_grader_throws(val):
     global grader_throws
     grader_throws = val
 
 
 class Grader:
-
     def __init__(self):
         pass
 
     @staticmethod
-    def grade_from_notebooks(test_cases_list, notebook_ipynb_list,
-                             results_json):
+    def grade_from_notebooks(
+        test_cases_list, notebook_ipynb_list, results_json
+    ):
         """
         Running notebooks in notebook_ipynb_list and evaluating
         them on test_cases_list. Result is written into results_json
         """
         try:
             notebook_locals_list = []
             for notebook_ipynb in notebook_ipynb_list:
                 notebook_locals_list.append(
-                    Grader.locals_from_notebook(notebook_ipynb))
+                    Grader.locals_from_notebook(notebook_ipynb)
+                )
         except Exception as e:
             Grader.global_fail_with_error_message(
-                "Exception when running file: " + notebook_ipynb + ', '
-                + str(e), results_json)
+                "Exception when running file: "
+                + notebook_ipynb
+                + ", "
+                + str(e),
+                results_json,
+            )
             raise
 
         # Grade notebook_locals_list on test_cases_list
-        Grader.grade_output(test_cases_list, notebook_locals_list, results_json)
+        Grader.grade_output(
+            test_cases_list, notebook_locals_list, results_json
+        )
 
     @staticmethod
     def grade_output(test_case_list, notebook_locals_list, results_json):
         """Grading the notebook_locals with the provided test_cases"""
         # setup test suite for gradescope
         suite = unittest.TestSuite()
-        for test_case, notebook_locals in zip(test_case_list,
-                                              notebook_locals_list):
+        for test_case, notebook_locals in zip(
+            test_case_list, notebook_locals_list
+        ):
             test_case_names = unittest.defaultTestLoader.getTestCaseNames(
-                test_case)
+                test_case
+            )
             for test_case_name in test_case_names:
                 suite.addTest(test_case(test_case_name, notebook_locals))
 
         # run all the tests in the suite
-        with open(results_json, 'w') as fh:
+        with open(results_json, "w") as fh:
             JSONTestRunner(stream=fh).run(suite)
 
     @staticmethod
     def locals_from_notebook(notebook_ipynb):
         """Read, run, return locals of notebook"""
-        banned_commands = ['HTML']
+        banned_commands = ["HTML"]
 
         ipynb = json.load(open(notebook_ipynb))
 
-        for cell in ipynb['cells']:
+        for cell in ipynb["cells"]:
             # erase test cells, this is optional and useful for debugging
             # to avoid recursions when developing
-            if any('## TEST ##' in line for line in cell['source']):
-                cell['source'] = []
+            if any("## TEST ##" in line for line in cell["source"]):
+                cell["source"] = []
             # filter out all the lines with banned commands
             if banned_commands is not None:
-                cell['source'] = [
-                    line for line in cell['source']
+                cell["source"] = [
+                    line
+                    for line in cell["source"]
                     if not any(command in line for command in banned_commands)
                 ]
 
         exporter = PythonExporter()
         source, meta = exporter.from_notebook_node(
-            nbformat.reads(json.dumps(ipynb), nbformat.NO_CONVERT))
-        with open('./cleaned_notebook.py', 'w') as fh:
+            nbformat.reads(json.dumps(ipynb), nbformat.NO_CONVERT)
+        )
+        with open("./cleaned_notebook.py", "w") as fh:
             fh.write(source)
 
-        notebook_locals = run_path('cleaned_notebook.py')
-        os.system('rm cleaned_notebook.py')
+        notebook_locals = run_path("cleaned_notebook.py")
+        os.system("rm cleaned_notebook.py")
         return notebook_locals
 
     @staticmethod
     def global_fail_with_error_message(msg, results_json):
         """Error message if no specific"""
         results = {"score": 0.0, "output": msg}
 
-        with open(results_json, 'w') as f:
+        with open(results_json, "w") as f:
             f.write(
-                json.dumps(results,
-                           indent=4,
-                           sort_keys=True,
-                           separators=(',', ': '),
-                           ensure_ascii=True))
+                json.dumps(
+                    results,
+                    indent=4,
+                    sort_keys=True,
+                    separators=(",", ": "),
+                    ensure_ascii=True,
+                )
+            )
 
     @staticmethod
     def print_test_results(results_json):
         """Printing the results.json"""
         # open the json file for reading
-        with open(results_json, 'r') as fh:
+        with open(results_json, "r") as fh:
             result = json.load(fh)
 
         # print total score
-        max_score = sum(test['max_score'] for test in result['tests'])
-        print('Total score is {}/{}.'.format(int(result['score']), max_score))
+        max_score = sum(test["max_score"] for test in result["tests"])
+        print("Total score is {}/{}.".format(int(result["score"]), max_score))
 
-        if grader_throws and int(result['score']) != max_score:
+        if grader_throws and int(result["score"]) != max_score:
             raise RuntimeError("Grader did not award full points.")
 
         # print partial scores
-        for test in result['tests']:
-            print('\nScore for {} is {}/{}.'.format(test['name'],
-                                                    int(test['score']),
-                                                    test['max_score']))
+        for test in result["tests"]:
+            print(
+                "\nScore for {} is {}/{}.".format(
+                    test["name"], int(test["score"]), test["max_score"]
+                )
+            )
 
             # print error message if any
-            if 'output' in test:
-                print('- ' + test['output'])
+            if "output" in test:
+                print("- " + test["output"])
```

### Comparing `underactuated-2023.3.2/underactuated/exercises/humanoids/test_footstep_planning.py` & `underactuated-2023.4.17/underactuated/exercises/humanoids/test_footstep_planning.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,142 +1,160 @@
 import unittest
+
+import numpy as np
 import timeout_decorator
 from gradescope_utils.autograder_utils.decorators import weight
-import numpy as np
 
 
 class TestFootstepPlanning(unittest.TestCase):
-
     def __init__(self, test_name, notebook_locals):
         """
         Since the planner raises an error if the problem is infeasible, it is
         better to solve the optimizations inside each method rather than here in
         the __init__ method. This way if the plan is infeasible, students get
         zero points instead of an error from the test file. Note also that each
         time a test (method of this class) fails a new class is instantiated,
         hence we must re-solve the plans for each test.
         """
         super().__init__(test_name)
 
         # get locals
         self.notebook_locals = notebook_locals
-        Terrain = self.notebook_locals['Terrain']
-        self.footstep_planner = self.notebook_locals['footstep_planner']
+        Terrain = self.notebook_locals["Terrain"]
+        self.footstep_planner = self.notebook_locals["footstep_planner"]
 
         # empty solution of the benchmark problems
-        self.terrains = {'A': Terrain([1, 1, 1, 1]), 'B': Terrain([1, 1, 1, 0])}
+        self.terrains = {
+            "A": Terrain([1, 1, 1, 1]),
+            "B": Terrain([1, 1, 1, 0]),
+        }
         self.n_steps = 8
-        self.step_span = .8
-        self.plans = {'A': {}, 'B': {}}
+        self.step_span = 0.8
+        self.plans = {"A": {}, "B": {}}
 
     def _solve_benchmarks(self):
         """Solves the benchmark problems."""
-        for plan in ['A', 'B']:
-            self.plans[plan]['vars'], self.plans[plan][
-                'cost'] = self.footstep_planner(self.terrains[plan],
-                                                self.n_steps, self.step_span)
+        for plan in ["A", "B"]:
+            (
+                self.plans[plan]["vars"],
+                self.plans[plan]["cost"],
+            ) = self.footstep_planner(
+                self.terrains[plan], self.n_steps, self.step_span
+            )
 
     @weight(4)
-    @timeout_decorator.timeout(30.)
+    @timeout_decorator.timeout(30.0)
     def test_relative_position_limits(self):
         """Tests the constraints on the relative position of the feet"""
         self._solve_benchmarks()
 
         # center to corner vector for the square with side step_span
         # (plus tolerance for the checks)
         tol = 1e-2
         c2c = np.ones(2) * self.step_span / 2 + tol
 
         # check constraint for both terrains
-        for plan in ['A', 'B']:
-            position_left, position_right = self.plans[plan]['vars'][:2]
+        for plan in ["A", "B"]:
+            position_left, position_right = self.plans[plan]["vars"][:2]
             relative_position = position_left - position_right
             for t in range(self.n_steps + 1):
-                msg = f'Error at foot step {t} when solving the problem ' + \
-                    f'for terrain_{plan}: one foot is not contained in a ' + \
-                    f'square of side {self.step_span} centered at the ' + \
-                    'other foot.'
+                msg = (
+                    f"Error at foot step {t} when solving the problem "
+                    + f"for terrain_{plan}: one foot is not contained in a "
+                    + f"square of side {self.step_span} centered at the "
+                    + "other foot."
+                )
                 np.testing.assert_array_less(relative_position[t], c2c, msg)
                 np.testing.assert_array_less(-relative_position[t], c2c, msg)
 
     @weight(3)
-    @timeout_decorator.timeout(30.)
+    @timeout_decorator.timeout(30.0)
     def test_one_stone_per_foot(self):
         """Tests that a foot is assigned to a single stepping stone"""
         self._solve_benchmarks()
 
         # check constraint for both terrains
-        for plan in ['A', 'B']:
-            stone_left, stone_right = self.plans[plan]['vars'][2:4]
+        for plan in ["A", "B"]:
+            stone_left, stone_right = self.plans[plan]["vars"][2:4]
             for t in range(self.n_steps + 1):
-                msg = f'Error at foot step {t} when solving the problem ' + \
-                    f'for terrain_{plan}: '
+                msg = (
+                    f"Error at foot step {t} when solving the problem "
+                    + f"for terrain_{plan}: "
+                )
                 self.assertAlmostEqual(
                     sum(stone_left[t]),
                     1,
                     places=4,
-                    msg=msg + f'stone_left[{t}] do not sum up to one.')
+                    msg=msg + f"stone_left[{t}] do not sum up to one.",
+                )
                 self.assertAlmostEqual(
                     sum(stone_right[t]),
                     1,
                     places=4,
-                    msg=msg + f'stone_right[{t}] do not sum up to one.')
+                    msg=msg + f"stone_right[{t}] do not sum up to one.",
+                )
 
     @weight(5)
-    @timeout_decorator.timeout(30.)
+    @timeout_decorator.timeout(30.0)
     def test_foot_in_stepping_stone(self):
         """Tests that binaries imply correctly the positioning of the feet"""
         self._solve_benchmarks()
         tol = 1e-2
 
         # check constraint for both terrains
-        for plan in ['A', 'B']:
-            position_left, position_right, \
-                stone_left, stone_right = self.plans[plan]['vars'][:4]
+        for plan in ["A", "B"]:
+            (
+                position_left,
+                position_right,
+                stone_left,
+                stone_right,
+            ) = self.plans[plan]["vars"][:4]
             for t in range(self.n_steps + 1):
-
                 # left foot
                 i = np.where(np.isclose(stone_left[t], 1, atol=tol))[0][0]
                 stone = self.terrains[plan].stepping_stones[i]
                 np.testing.assert_array_less(
-                    stone.A.dot(position_left[t]), stone.b + tol,
-                    f'Solving the problem for terrain_{plan}, the binary '
-                    + f'variable stone_left[{t}, {i}] is one but the left foot '
-                    + f'is not in stone {i} at time {t}.')
+                    stone.A.dot(position_left[t]),
+                    stone.b + tol,
+                    f"Solving the problem for terrain_{plan}, the binary "
+                    + f"variable stone_left[{t}, {i}] is one but the left foot "
+                    + f"is not in stone {i} at time {t}.",
+                )
 
                 # right foot
                 i = np.where(np.isclose(stone_right[t], 1, atol=tol))[0][0]
                 stone = self.terrains[plan].stepping_stones[i]
                 np.testing.assert_array_less(
-                    stone.A.dot(position_right[t]), stone.b + tol,
-                    f'Solving the problem for terrain_{plan}, the binary '
-                    + f'variable stone_right[{t}, {i}] is one but the right '
-                    + f'foot is not in stone {i} at time {t}.')
+                    stone.A.dot(position_right[t]),
+                    stone.b + tol,
+                    f"Solving the problem for terrain_{plan}, the binary "
+                    + f"variable stone_right[{t}, {i}] is one but the right "
+                    + f"foot is not in stone {i} at time {t}.",
+                )
 
     @weight(4)
-    @timeout_decorator.timeout(30.)
+    @timeout_decorator.timeout(30.0)
     def test_minimize_step_length(self):
         """
         Tests that the positioning of the feet minimized the sum of the
         square of the two norm of the step lengths.
         """
         self._solve_benchmarks()
-        tol = 1e-2
 
         # check constraint for both terrains
-        target_cost = {'A': 4.1592510194, 'B': 5.6478552756}
-        for plan in ['A', 'B']:
-
+        target_cost = {"A": 4.1592510194, "B": 5.6478552756}
+        for plan in ["A", "B"]:
             # same convergence check as in
             # https://github.com/RobotLocomotion/drake/blob/88c93118df507777eb3f99628d1aa7c808f81f49/solvers/branch_and_bound.cc#L711
             # with double the tolerances from
             # https://github.com/RobotLocomotion/drake/blob/4ee674e7931527df838bd33e79cf2f4dad57bd20/solvers/branch_and_bound.h#L674
             atol = 2e-2
             rtol = 2e-2
-            gap = self.plans[plan]['cost'] - target_cost[plan]
+            gap = self.plans[plan]["cost"] - target_cost[plan]
             atol_convergence = gap <= atol
             rtol_convergence = gap / target_cost[plan] <= rtol
             self.assertTrue(
                 atol_convergence or rtol_convergence,
-                f'Target cost of {target_cost[plan]} is not achieved for '
-                + f'terrain_{plan}, with absolute tolerance {atol} and '
-                + f'relative tolerance {rtol}.')
+                f"Target cost of {target_cost[plan]} is not achieved for "
+                + f"terrain_{plan}, with absolute tolerance {atol} and "
+                + f"relative tolerance {rtol}.",
+            )
```

### Comparing `underactuated-2023.3.2/underactuated/exercises/intro/test_drake_systems.py` & `underactuated-2023.4.17/underactuated/exercises/intro/test_drake_systems.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,49 +1,51 @@
-import numpy as np
 import unittest
+
+import numpy as np
 import timeout_decorator
 from gradescope_utils.autograder_utils.decorators import weight
-
 from pydrake.all import System
 
 
 class TestDrakeSystems(unittest.TestCase):
-
     def __init__(self, test_name, notebook_locals):
         super().__init__(test_name)
         self.notebook_locals = notebook_locals
 
     @weight(1)
-    @timeout_decorator.timeout(5.)
+    @timeout_decorator.timeout(5.0)
     def test_input_and_state(self):
         # note: all prints here go to the output item in the json file
 
-        system = self.notebook_locals['pendulum_system']
+        system = self.notebook_locals["pendulum_system"]
 
         assert isinstance(system, System), "pendulum_system is not a System"
         assert system.num_input_ports() == 1, "should have 1 input port"
-        assert system.get_input_port(
-            0).size() == 1, "the input port is the wrong size"
-        assert system.num_continuous_states(
-        ) == 2, "wrong size for the state vector"
-        assert system.num_discrete_state_groups(
-        ) == 0, "your system should not have discrete states"
+        assert (
+            system.get_input_port(0).size() == 1
+        ), "the input port is the wrong size"
+        assert (
+            system.num_continuous_states() == 2
+        ), "wrong size for the state vector"
+        assert (
+            system.num_discrete_state_groups() == 0
+        ), "your system should not have discrete states"
 
     @weight(1)
-    @timeout_decorator.timeout(5.)
+    @timeout_decorator.timeout(5.0)
     def test_dynamics(self):
         # note: all prints here go to the output item in the json file
 
-        system = self.notebook_locals['pendulum_system']
+        system = self.notebook_locals["pendulum_system"]
         context = system.CreateDefaultContext()
 
         q = np.linspace(0, 1, 5)
         v = np.linspace(0, 1, 5)
         u = np.linspace(0, 1, 5)
         qs, vs, us = np.meshgrid(q, v, u)
         for qi, vi, ui in zip(qs.flat, vs.flat, us.flat):
             context.SetContinuousState([qi, vi])
             system.get_input_port(0).FixValue(context, [ui])
             xdot = [vi, ui - vi - 10 * np.sin(qi)]
             np.testing.assert_almost_equal(
-                xdot,
-                system.EvalTimeDerivatives(context).CopyToVector())
+                xdot, system.EvalTimeDerivatives(context).CopyToVector()
+            )
```

### Comparing `underactuated-2023.3.2/underactuated/exercises/lqr/test_drake_diagrams.py` & `underactuated-2023.4.17/underactuated/exercises/lqr/test_drake_diagrams.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,113 +3,137 @@
 import numpy as np
 import timeout_decorator
 from gradescope_utils.autograder_utils.decorators import weight
 from pydrake.all import AffineSystem, Diagram, System
 
 
 class TestDrakeDiagrams(unittest.TestCase):
-
     def __init__(self, test_name, notebook_locals):
         super().__init__(test_name)
         self.notebook_locals = notebook_locals
 
     @weight(1)
-    @timeout_decorator.timeout(5.)
+    @timeout_decorator.timeout(5.0)
     def test_actuator_model(self):
         # note: all prints here go to the output item in the json file
 
-        actuator_model = self.notebook_locals['actuator_model']
+        actuator_model = self.notebook_locals["actuator_model"]
 
-        assert isinstance(actuator_model,
-                          System), "actuator_model must be a System"
-        assert actuator_model.ToAutoDiffXdMaybe(
+        assert isinstance(
+            actuator_model, System
+        ), "actuator_model must be a System"
+        assert (
+            actuator_model.ToAutoDiffXdMaybe()
         ), "Your system isn't compatible with Drake's AutoDiffXd; see the note above."  # noqa
-        assert actuator_model.num_input_ports(
-        ) == 1, "must have exactly one input port"
-        assert actuator_model.get_input_port().size(
-        ) == 1, "input port must have size 1"
-        assert actuator_model.num_output_ports(
-        ) == 1, "must have only one output port"
-        assert actuator_model.get_output_port().size(
-        ) == 1, "output port should have size 1"
-        assert actuator_model.num_continuous_states(
-        ) == 1, "should have exactly one continuous state variable"
-        assert actuator_model.num_discrete_state_groups(
-        ) == 0, "should not have any discrete state"
+        assert (
+            actuator_model.num_input_ports() == 1
+        ), "must have exactly one input port"
+        assert (
+            actuator_model.get_input_port().size() == 1
+        ), "input port must have size 1"
+        assert (
+            actuator_model.num_output_ports() == 1
+        ), "must have only one output port"
+        assert (
+            actuator_model.get_output_port().size() == 1
+        ), "output port should have size 1"
+        assert (
+            actuator_model.num_continuous_states() == 1
+        ), "should have exactly one continuous state variable"
+        assert (
+            actuator_model.num_discrete_state_groups() == 0
+        ), "should not have any discrete state"
 
         context = actuator_model.CreateDefaultContext()
 
         def check_dynamics(x, u):
             context.SetContinuousState([x])
             actuator_model.get_input_port().FixValue(context, [u])
             xdot = actuator_model.EvalTimeDerivatives(context).CopyToVector()
             self.assertAlmostEqual(
-                2 * (u - x), xdot[0],
-                'the state dynamics (xdot) of your actuator model are incorrect'
+                2 * (u - x),
+                xdot[0],
+                "the state dynamics (xdot) of your actuator model are incorrect",
             )
             y = actuator_model.get_output_port().Eval(context)
             self.assertAlmostEqual(
-                y, x, 'the output value of your actuator model is incorrect')
+                y, x, "the output value of your actuator model is incorrect"
+            )
 
         check_dynamics(x=0, u=0)
         check_dynamics(x=0.4, u=0.1)
         check_dynamics(x=0.52, u=0.25)
         check_dynamics(x=-0.91, u=5.2)
         check_dynamics(x=2, u=-2)
 
     @weight(1)
-    @timeout_decorator.timeout(5.)
+    @timeout_decorator.timeout(5.0)
     def test_diagram(self):
-        diagram = self.notebook_locals['diagram']
-        assert isinstance(diagram, Diagram), 'diagram must be a Diagram'
-        assert len(diagram.GetSystems()
-                  ) == 2, 'diagram should have exactly two subsystems'  # noqa
-        assert diagram.ToAutoDiffXdMaybe(
+        diagram = self.notebook_locals["diagram"]
+        assert isinstance(diagram, Diagram), "diagram must be a Diagram"
+        assert (
+            len(diagram.GetSystems()) == 2
+        ), "diagram should have exactly two subsystems"  # noqa
+        assert (
+            diagram.ToAutoDiffXdMaybe()
         ), "Your system isn't compatible with Drake's AutoDiffXd; see the note above."  # noqa
-        assert diagram.num_input_ports(
-        ) == 1, "diagram should have exactly one input port"
-        assert diagram.get_input_port().size(
-        ) == 1, "diagram's input port should have size 1"
-        assert diagram.num_continuous_states(
-        ) == 3, "diagram should have a total of 3 continuous states"
-        assert diagram.num_discrete_state_groups(
-        ) == 0, "diagram should not have any discrete states"
+        assert (
+            diagram.num_input_ports() == 1
+        ), "diagram should have exactly one input port"
+        assert (
+            diagram.get_input_port().size() == 1
+        ), "diagram's input port should have size 1"
+        assert (
+            diagram.num_continuous_states() == 3
+        ), "diagram should have a total of 3 continuous states"
+        assert (
+            diagram.num_discrete_state_groups() == 0
+        ), "diagram should not have any discrete states"
 
     @weight(1)
-    @timeout_decorator.timeout(5.)
+    @timeout_decorator.timeout(5.0)
     def test_diagram_context(self):
-        diagram = self.notebook_locals['diagram']
-        double_integrator = self.notebook_locals['double_integrator']
-        actuator_model = self.notebook_locals['actuator_model']
-        context = self.notebook_locals['diagram_context']
+        diagram = self.notebook_locals["diagram"]
+        double_integrator = self.notebook_locals["double_integrator"]
+        actuator_model = self.notebook_locals["actuator_model"]
+        context = self.notebook_locals["diagram_context"]
 
         double_integrator_context = double_integrator.GetMyContextFromRoot(
-            context)
+            context
+        )
         np.testing.assert_almost_equal(
             double_integrator_context.get_continuous_state_vector().get_value(),
             [1.2, 0],
-            err_msg="the value of the double integrator state is incorrect")
+            err_msg="the value of the double integrator state is incorrect",
+        )
         actuator_model_context = actuator_model.GetMyContextFromRoot(context)
         np.testing.assert_almost_equal(
             actuator_model_context.get_continuous_state_vector().get_value(),
             [0],
-            err_msg="the value of the actuator model state is incorrect")
+            err_msg="the value of the actuator model state is incorrect",
+        )
 
         assert diagram.get_input_port().HasValue(
-            context), "you must fix a value for the diagram's input port"
+            context
+        ), "you must fix a value for the diagram's input port"
         np.testing.assert_almost_equal(
-            diagram.get_input_port().Eval(context), [0],
-            err_msg="the input port value is incorrect")
+            diagram.get_input_port().Eval(context),
+            [0],
+            err_msg="the input port value is incorrect",
+        )
 
     @weight(1)
-    @timeout_decorator.timeout(5.)
+    @timeout_decorator.timeout(5.0)
     def test_controller(self):
-        controller = self.notebook_locals['controller']
-        assert isinstance(controller,
-                          AffineSystem), "controller should be an affine system"
-
-        assert controller.num_continuous_states(
-        ) == 0, "your controller has state; that shouldn't happen"
+        controller = self.notebook_locals["controller"]
+        assert isinstance(
+            controller, AffineSystem
+        ), "controller should be an affine system"
+
+        assert (
+            controller.num_continuous_states() == 0
+        ), "your controller has state; that shouldn't happen"
         np.testing.assert_almost_equal(
             np.sort(controller.D()),
-            np.sort([[-1.06519664, -1., -2.26503715]]),
-            err_msg="your LQR gains do not match the expected value")
+            np.sort([[-1.06519664, -1.0, -2.26503715]]),
+            err_msg="your LQR gains do not match the expected value",
+        )
```

### Comparing `underactuated-2023.3.2/underactuated/exercises/lyapunov/test_control.py` & `underactuated-2023.4.17/underactuated/exercises/lyapunov/test_control.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,145 +1,179 @@
 import unittest
+
+import numpy as np
 import timeout_decorator
 from gradescope_utils.autograder_utils.decorators import weight
-import numpy as np
 
 
 class TestControl(unittest.TestCase):
-
     def __init__(self, test_name, notebook_locals):
         super().__init__(test_name)
         self.notebook_locals = notebook_locals
 
     @weight(4)
-    @timeout_decorator.timeout(1.)
+    @timeout_decorator.timeout(1.0)
     def test_lyapunov_controller_near_origin(self):
         """Test Lyapunov controller near origin"""
         # load controller from locals
-        lyapunov_controller = self.notebook_locals['lyapunov_controller']
+        lyapunov_controller = self.notebook_locals["lyapunov_controller"]
 
         # function that scales a vector in such a way that the third coordinate
         # has absolute value <= a desired tolerance
         # needed to handle the local linearization in the controller
         def project_in(x, tol):
             return x if np.abs(x[2]) <= tol else x * tol / np.abs(x[2])
 
         # generate random states at which evaluate the dynamics
         n = 50
         tol = 1e-4  # must be smaller than the one in the notebook (= 1e-3)
         np.random.seed(0)
         x = [project_in(np.random.randn(3), tol) for i in range(n)]
 
         # desired value of the dynamics at given test points
-        f_des = np.array([[-1.80237445e-04, 2.40885019e-04],
-                          [-2.29299489e-04, -8.90205042e-06],
-                          [-9.20460164e-04, -3.46637175e-04],
-                          [-2.82339256e-05, 2.09904847e-04],
-                          [-1.71457707e-04, 2.27412727e-04],
-                          [-1.62642401e-04, 5.28256832e-04],
-                          [-1.22627869e-05, -2.33454726e-04],
-                          [-8.80691725e-05, -8.35250685e-05],
-                          [-4.96028881e-03, -2.97834965e-03],
-                          [1.27391521e-05, 3.04316199e-04],
-                          [-1.74532454e-05, -1.57403853e-04],
-                          [1.26690727e-03, -2.25228291e-05],
-                          [-3.17636327e-04, 1.10430312e-04],
-                          [2.12886571e-05, -2.73840825e-04],
-                          [3.34791107e-04, 1.82766025e-04],
-                          [5.63446602e-05, 3.88667653e-05],
-                          [1.80229828e-04, -2.23757479e-04],
-                          [-3.27707902e-05, -2.43265392e-04],
-                          [4.23683178e-05, 8.43941306e-04],
-                          [-8.33850482e-05, -3.74869067e-04],
-                          [8.26985819e-05, -2.44217525e-04],
-                          [4.29657666e-04, -1.55840079e-04],
-                          [1.79676102e-04, -1.48993377e-04],
-                          [-4.02730836e-05, 7.65261365e-04],
-                          [-2.83192333e-04, -1.06909774e-04],
-                          [1.18305344e-04, -3.50435804e-04],
-                          [2.67392673e-05, -1.95179561e-04],
-                          [-5.86382545e-05, -1.69688244e-04],
-                          [-1.26253646e-04, 3.60834920e-04],
-                          [1.70633544e-05, 9.84540881e-05],
-                          [1.93579156e-04, 7.86938038e-04],
-                          [-1.38221925e-04, 2.50435880e-04],
-                          [-8.27345956e-06, 1.60717126e-03],
-                          [-2.98265004e-05, -6.02754193e-05],
-                          [1.08299347e-04, -1.17366178e-04],
-                          [-2.60031931e-04, -2.55336988e-04],
-                          [-1.02965532e-04, 2.79275398e-04],
-                          [-4.74352797e-05, 1.54911183e-04],
-                          [2.82927224e-05, 2.84714144e-04],
-                          [1.68086067e-05, 2.66588042e-04],
-                          [-1.26216414e-04, -1.68631814e-04],
-                          [-8.86416924e-04, -6.64176158e-04],
-                          [6.47266017e-05, 4.75067403e-04],
-                          [-7.55609542e-05, 5.72244360e-05],
-                          [1.06052814e-04, -1.94993984e-04],
-                          [-3.24741878e-04, 7.68095349e-05],
-                          [-2.65552184e-05, -2.73297968e-04],
-                          [-6.91921177e-05, 2.26246495e-04],
-                          [-2.61074358e-04, -9.65319357e-05],
-                          [-2.41996000e-04, -4.85084770e-04]])
+        f_des = np.array(
+            [
+                [-1.80237445e-04, 2.40885019e-04],
+                [-2.29299489e-04, -8.90205042e-06],
+                [-9.20460164e-04, -3.46637175e-04],
+                [-2.82339256e-05, 2.09904847e-04],
+                [-1.71457707e-04, 2.27412727e-04],
+                [-1.62642401e-04, 5.28256832e-04],
+                [-1.22627869e-05, -2.33454726e-04],
+                [-8.80691725e-05, -8.35250685e-05],
+                [-4.96028881e-03, -2.97834965e-03],
+                [1.27391521e-05, 3.04316199e-04],
+                [-1.74532454e-05, -1.57403853e-04],
+                [1.26690727e-03, -2.25228291e-05],
+                [-3.17636327e-04, 1.10430312e-04],
+                [2.12886571e-05, -2.73840825e-04],
+                [3.34791107e-04, 1.82766025e-04],
+                [5.63446602e-05, 3.88667653e-05],
+                [1.80229828e-04, -2.23757479e-04],
+                [-3.27707902e-05, -2.43265392e-04],
+                [4.23683178e-05, 8.43941306e-04],
+                [-8.33850482e-05, -3.74869067e-04],
+                [8.26985819e-05, -2.44217525e-04],
+                [4.29657666e-04, -1.55840079e-04],
+                [1.79676102e-04, -1.48993377e-04],
+                [-4.02730836e-05, 7.65261365e-04],
+                [-2.83192333e-04, -1.06909774e-04],
+                [1.18305344e-04, -3.50435804e-04],
+                [2.67392673e-05, -1.95179561e-04],
+                [-5.86382545e-05, -1.69688244e-04],
+                [-1.26253646e-04, 3.60834920e-04],
+                [1.70633544e-05, 9.84540881e-05],
+                [1.93579156e-04, 7.86938038e-04],
+                [-1.38221925e-04, 2.50435880e-04],
+                [-8.27345956e-06, 1.60717126e-03],
+                [-2.98265004e-05, -6.02754193e-05],
+                [1.08299347e-04, -1.17366178e-04],
+                [-2.60031931e-04, -2.55336988e-04],
+                [-1.02965532e-04, 2.79275398e-04],
+                [-4.74352797e-05, 1.54911183e-04],
+                [2.82927224e-05, 2.84714144e-04],
+                [1.68086067e-05, 2.66588042e-04],
+                [-1.26216414e-04, -1.68631814e-04],
+                [-8.86416924e-04, -6.64176158e-04],
+                [6.47266017e-05, 4.75067403e-04],
+                [-7.55609542e-05, 5.72244360e-05],
+                [1.06052814e-04, -1.94993984e-04],
+                [-3.24741878e-04, 7.68095349e-05],
+                [-2.65552184e-05, -2.73297968e-04],
+                [-6.91921177e-05, 2.26246495e-04],
+                [-2.61074358e-04, -9.65319357e-05],
+                [-2.41996000e-04, -4.85084770e-04],
+            ]
+        )
 
         # test the function at the evaluation points
         f = np.vstack([lyapunov_controller(*xi) for xi in x])
         np.testing.assert_array_almost_equal(
             f,
             f_des,
             decimal=4,
-            err_msg='The controller is not correct near the origin.')
+            err_msg="The controller is not correct near the origin.",
+        )
 
     @weight(4)
-    @timeout_decorator.timeout(1.)
+    @timeout_decorator.timeout(1.0)
     def test_lyapunov_controller_away_from_origin(self):
         """Test Lyapunov controller away from origin"""
         # load controller from locals
-        lyapunov_controller = self.notebook_locals['lyapunov_controller']
+        lyapunov_controller = self.notebook_locals["lyapunov_controller"]
 
         # function that scales a vector in such a way that the third coordinate
         # has absolute value >= a desired tolerance
         # needed to handle the local linearization in the controller
         def project_out(x, tol):
             return x if np.abs(x[2]) >= tol else x * tol / np.abs(x[2])
 
         # generate random states at which evaluate the dynamics
         n = 50
         tol = 1e-2  # must be greater than the one in the notebook (= 1e-3)
         np.random.seed(0)
         x = [project_out(np.random.randn(3), tol) for i in range(n)]
 
         # desired value of the dynamics at given test points
-        f_des = np.array([[-0.98446505, 1.63115278], [-1.25328942, -0.5549188],
-                          [-0.94503173, -0.35599057], [-0.0477359, 1.58118168],
-                          [-0.68729272, 0.93799447], [-0.32667676, 1.04789874],
-                          [0.26038379, -1.93673728], [-0.48172147, -0.6600981],
-                          [-2.26737878, -1.3608832], [0.01895493, 1.67519335],
-                          [-0.09779214, -1.16880824], [1.95663546, -0.0321076],
-                          [-1.13915329, 0.34862014], [0.04540821, -1.67817773],
-                          [1.48942757, 0.69456878], [0.31220516, 0.47186241],
-                          [1.00893588, -1.49932112], [-0.14715458, -1.68457734],
-                          [0.0281199, 0.55990795], [-0.28278935, -1.27461434],
-                          [0.46212572, -1.53312378], [1.58881182, -0.60275863],
-                          [1.00400078, -1.14502099], [-0.0515139, 0.97757105],
-                          [-1.04841566, -0.34316574], [0.5732494, -1.72569781],
-                          [0.12294264, -1.51026049], [-0.03111974, -1.56030365],
-                          [-0.56859115, 2.09971095], [0.08882972, 1.04781451],
-                          [0.39446391, 1.59797754], [-0.742823, 1.44942476],
-                          [-0.01041557, 2.01922169], [-0.0889171, -1.26206768],
-                          [0.49202569, -1.23512984], [-1.42549336, -1.52190444],
-                          [0.56231803, 1.3662271], [0.30152939, 1.73773857],
-                          [0.15649151, 1.82285483], [0.09363587, 1.72416136],
-                          [-0.35980848, -0.45625562],
-                          [-1.31156436, -0.98129184], [0.34046179, 2.49985597],
-                          [-0.34964074, 0.35076956], [0.54254751, -1.08972773],
-                          [-0.66181161, 0.14943231], [-0.03146467, -1.62851599],
-                          [-0.35373363, 1.23793387], [-1.45732914, -0.89604197],
-                          [-1.00011818, -1.997144]])
+        f_des = np.array(
+            [
+                [-0.98446505, 1.63115278],
+                [-1.25328942, -0.5549188],
+                [-0.94503173, -0.35599057],
+                [-0.0477359, 1.58118168],
+                [-0.68729272, 0.93799447],
+                [-0.32667676, 1.04789874],
+                [0.26038379, -1.93673728],
+                [-0.48172147, -0.6600981],
+                [-2.26737878, -1.3608832],
+                [0.01895493, 1.67519335],
+                [-0.09779214, -1.16880824],
+                [1.95663546, -0.0321076],
+                [-1.13915329, 0.34862014],
+                [0.04540821, -1.67817773],
+                [1.48942757, 0.69456878],
+                [0.31220516, 0.47186241],
+                [1.00893588, -1.49932112],
+                [-0.14715458, -1.68457734],
+                [0.0281199, 0.55990795],
+                [-0.28278935, -1.27461434],
+                [0.46212572, -1.53312378],
+                [1.58881182, -0.60275863],
+                [1.00400078, -1.14502099],
+                [-0.0515139, 0.97757105],
+                [-1.04841566, -0.34316574],
+                [0.5732494, -1.72569781],
+                [0.12294264, -1.51026049],
+                [-0.03111974, -1.56030365],
+                [-0.56859115, 2.09971095],
+                [0.08882972, 1.04781451],
+                [0.39446391, 1.59797754],
+                [-0.742823, 1.44942476],
+                [-0.01041557, 2.01922169],
+                [-0.0889171, -1.26206768],
+                [0.49202569, -1.23512984],
+                [-1.42549336, -1.52190444],
+                [0.56231803, 1.3662271],
+                [0.30152939, 1.73773857],
+                [0.15649151, 1.82285483],
+                [0.09363587, 1.72416136],
+                [-0.35980848, -0.45625562],
+                [-1.31156436, -0.98129184],
+                [0.34046179, 2.49985597],
+                [-0.34964074, 0.35076956],
+                [0.54254751, -1.08972773],
+                [-0.66181161, 0.14943231],
+                [-0.03146467, -1.62851599],
+                [-0.35373363, 1.23793387],
+                [-1.45732914, -0.89604197],
+                [-1.00011818, -1.997144],
+            ]
+        )
 
         # test the function at the evaluation points
         f = np.vstack([lyapunov_controller(*xi) for xi in x])
         np.testing.assert_array_almost_equal(
             f,
             f_des,
             decimal=4,
-            err_msg='The controller is not correct far away from the origin.')
+            err_msg="The controller is not correct far away from the origin.",
+        )
```

### Comparing `underactuated-2023.3.2/underactuated/exercises/lyapunov/test_van_der_pol.py` & `underactuated-2023.4.17/underactuated/exercises/lyapunov/test_van_der_pol.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,99 +1,151 @@
 import unittest
+
+import numpy as np
 import timeout_decorator
 from gradescope_utils.autograder_utils.decorators import weight
-import numpy as np
 from pydrake.all import Solve
 
 
 class TestVanDerPol(unittest.TestCase):
-
     def __init__(self, test_name, notebook_locals):
         super().__init__(test_name)
         self.notebook_locals = notebook_locals
 
-    @weight(5)
-    @timeout_decorator.timeout(5.)
+    @weight(1)
+    @timeout_decorator.timeout(5.0)
+    def test_linearization(self):
+        """Test linearization matrix A"""
+        A = self.notebook_locals["A"]
+        target_A = np.array([[0, -1], [1, -1]])
+        assert A.shape == (
+            2,
+            2,
+        ), f"A must be a 2x2 matrix. Given A is {A.shape}"  # yapf: disable
+        err = np.linalg.norm(A - target_A)
+        self.assertLessEqual(err, 1e-8, "incorrect linearization matrix A")
+
+    @weight(1)
+    @timeout_decorator.timeout(5.0)
+    def test_lyapunov_matrices(self):
+        """Test lyapunov matrices"""
+        A = self.notebook_locals["A"]
+        Q = self.notebook_locals["Q"]
+        P = self.notebook_locals["P"]
+        assert Q.shape == (
+            2,
+            2,
+        ), f"Q must be a 2x2 matrix. Given Q is {Q.shape}"  # yapf: disable
+        assert P.shape == (
+            2,
+            2,
+        ), f"P must be a 2x2 matrix. Given P is {P.shape}"  # yapf: disable
+        target_Q = -(A.T @ P + P @ A)
+        np.testing.assert_array_almost_equal(
+            Q,
+            target_Q,
+            err_msg="A'P + PA is not equal to -Q.",
+        )
+
+    @weight(3)
+    @timeout_decorator.timeout(5.0)
     def test_method_1(self):
         """Test level set for Method 1"""
         # test level set value up to first digit
-        rho_method_1 = self.notebook_locals['rho_method_1']
-        self.assertEqual(hash(self.round(rho_method_1, 1)), 691752902764107778,
-                         "The level set from Method 1 is incorrect.")
+        rho_method_1 = self.notebook_locals["rho_method_1"]
+        self.assertEqual(
+            hash(self.round(rho_method_1, 1)),
+            691752902764107778,
+            "The level set from Method 1 is incorrect.",
+        )
 
         # test that the line search converged
-        is_verified = self.notebook_locals['is_verified']
+        is_verified = self.notebook_locals["is_verified"]
         self.assertTrue(
             is_verified(rho_method_1),
             "Could not verify the level set rho_method_1 with the function"
-            + "is_verified(rho).")
-        rho_step = self.notebook_locals['rho_step']
+            + "is_verified(rho).",
+        )
+        rho_step = self.notebook_locals["rho_step"]
         self.assertAlmostEqual(
             rho_step,
             0.01,
-            msg="rho_step is different from the predefined value of 0.01.")
+            msg="rho_step is different from the predefined value of 0.01.",
+        )
         self.assertFalse(
             is_verified(rho_method_1 + rho_step),
             "The function is_verified(rho) could verify the level set"
-            + "rho_method_1 + rho_step: line search is not complete.")
+            + "rho_method_1 + rho_step: line search is not complete.",
+        )
 
     @weight(5)
-    @timeout_decorator.timeout(5.)
+    @timeout_decorator.timeout(5.0)
     def test_method_2(self):
         """Test level set for Method 2"""
         # test level set value up to fourth digit
         # (note that the degree of the polynomial does not affect precision
         # in this particular problem)
-        rho_method_2 = self.notebook_locals['rho_method_2']
-        self.assertEqual(hash(self.round(rho_method_2, 4)), 702129196305569794,
-                         "The level set from Method 2 is incorrect.")
+        rho_method_2 = self.notebook_locals["rho_method_2"]
+        self.assertEqual(
+            hash(self.round(rho_method_2, 4)),
+            702129196305569794,
+            "The level set from Method 2 is incorrect.",
+        )
 
         # try to solve again the optimization problem
         # and test that the optimal value of rho is the same
         # to retrieve rho, find the only optimization variable in the cost
-        prog = self.notebook_locals['prog2']
+        prog = self.notebook_locals["prog2"]
         costs = prog.GetAllCosts()
-        self.assertEqual(len(costs), 1,
-                         "prog2 has more than one cost function.")
+        self.assertEqual(
+            len(costs), 1, "prog2 has more than one cost function."
+        )
         variables = prog.GetAllCosts()[0].variables()
-        self.assertEqual(len(variables), 1,
-                         "The cost function of prog2 is incorrect.")
+        self.assertEqual(
+            len(variables), 1, "The cost function of prog2 is incorrect."
+        )
         rho = variables[0]
         result = Solve(prog)
         self.assertAlmostEqual(
             result.GetSolution(rho),
             rho_method_2,
-            msg="Solving prog2 we got a different value of rho_method_2.")
+            msg="Solving prog2 we got a different value of rho_method_2.",
+        )
 
     @weight(5)
-    @timeout_decorator.timeout(5.)
+    @timeout_decorator.timeout(5.0)
     def test_method_3(self):
         """Test level set for Method 3"""
         # test level set value up to fourth digit
         # (note that the degree of the polynomial does not affect precision
         # in this particular problem)
-        rho_method_3 = self.notebook_locals['rho_method_3']
-        self.assertEqual(hash(self.round(rho_method_3, 4) * 2),
-                         1404258392611139588,
-                         "The level set from Method 3 is incorrect.")
+        rho_method_3 = self.notebook_locals["rho_method_3"]
+        self.assertEqual(
+            hash(self.round(rho_method_3, 4) * 2),
+            1404258392611139588,
+            "The level set from Method 3 is incorrect.",
+        )
 
         # try to solve again the optimization problem
         # and test that the optimal value of rho is the same
         # to retrieve rho, find the only optimization variable in the cost
-        prog = self.notebook_locals['prog3']
+        prog = self.notebook_locals["prog3"]
         costs = prog.GetAllCosts()
-        self.assertEqual(len(costs), 1,
-                         "prog3 has more than one cost function.")
+        self.assertEqual(
+            len(costs), 1, "prog3 has more than one cost function."
+        )
         variables = prog.GetAllCosts()[0].variables()
-        self.assertEqual(len(variables), 1,
-                         "The cost function of prog3 is incorrect.")
+        self.assertEqual(
+            len(variables), 1, "The cost function of prog3 is incorrect."
+        )
         rho = variables[0]
         result = Solve(prog)
         self.assertAlmostEqual(
             result.GetSolution(rho),
             rho_method_3,
-            msg="Solving prog3 we got a different value of rho_method_3.")
+            msg="Solving prog3 we got a different value of rho_method_3.",
+        )
 
     @staticmethod
     def round(n, decimals=0):
         multiplier = 10**decimals
         return round(n * multiplier) / multiplier
```

### Comparing `underactuated-2023.3.2/underactuated/exercises/pend/test_hopfield_network.py` & `underactuated-2023.4.17/underactuated/exercises/pend/test_hopfield_network.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,79 +1,83 @@
 import unittest
+
+import numpy as np
 import timeout_decorator
 from gradescope_utils.autograder_utils.decorators import weight
-import numpy as np
 
 
 class TestHopfield(unittest.TestCase):
-
     def __init__(self, test_name, notebook_locals):
         super().__init__(test_name)
         self.notebook_locals = notebook_locals
 
     @weight(6)
-    @timeout_decorator.timeout(5.)
+    @timeout_decorator.timeout(5.0)
     def test_Hopfield_Network(self):
         """Test Hopfield Network"""
         # note: all prints here go to the output item in the json file
 
-        dynamics = self.notebook_locals['dynamics']
-        calc_A = self.notebook_locals['calculate_A']
+        dynamics = self.notebook_locals["dynamics"]
+        calc_A = self.notebook_locals["calculate_A"]
 
         A = np.array([[1, 0], [0, 1], [-1, -1]])
         beta = 5
 
         x = np.array([0, 0])
         x_target = np.array([0, 0])
         x_nxt = dynamics(x, A, beta)
 
         self.assertTrue(
             all(abs(i - j) <= 1e-4 for i, j in zip(x_nxt, x_target)),
-            msg='For x = [0, 0], x_dot should be {}'.format(x_target),
+            msg="For x = [0, 0], x_dot should be {}".format(x_target),
         )
 
         x = np.array([1, 0])
         x_target = np.array([-0.00678274, 0.00664746])
         x_nxt = dynamics(x, A, beta)
 
         self.assertTrue(
             all(abs(i - j) <= 1e-4 for i, j in zip(x_nxt, x_target)),
-            msg='For x = [1, 0], x_dot should be {}'.format(x_target),
+            msg="For x = [1, 0], x_dot should be {}".format(x_target),
         )
 
         x = np.array([1, 1])
         x_target = np.array([-0.50000023, -0.50000023])
         x_nxt = dynamics(x, A, beta)
 
         self.assertTrue(
             all(abs(i - j) <= 1e-4 for i, j in zip(x_nxt, x_target)),
-            msg='Answer is incorrect for x = [1, 1].',
+            msg="Answer is incorrect for x = [1, 1].",
         )
 
         A = []
-        for item in self.notebook_locals['training_data']:
+        for item in self.notebook_locals["training_data"]:
             A += [item.reshape((-1))]
         A_target = np.array(A)
-        A_calc = calc_A(self.notebook_locals['training_data'])
+        A_calc = calc_A(self.notebook_locals["training_data"])
 
         self.assertTrue(
             all(
                 abs(i - j) <= 1e-4
-                for i, j in zip(A_target.shape, A_calc.shape)),
-            msg='Expecting the shape of A to be {}, but got {}.'.format(
-                A_target.shape, A_calc.shape),
+                for i, j in zip(A_target.shape, A_calc.shape)
+            ),
+            msg="Expecting the shape of A to be {}, but got {}.".format(
+                A_target.shape, A_calc.shape
+            ),
         )
 
         A_calc = calc_A(
-            [np.zeros((28, 28)).reshape((-1)),
-             np.ones((28, 28)).reshape((-1))])
+            [np.zeros((28, 28)).reshape((-1)), np.ones((28, 28)).reshape((-1))]
+        )
         A_target1 = np.array(
-            [np.zeros((28, 28)).reshape((-1)),
-             np.ones((28, 28)).reshape((-1))])
+            [np.zeros((28, 28)).reshape((-1)), np.ones((28, 28)).reshape((-1))]
+        )
         A_target2 = np.array(
-            [np.ones((28, 28)).reshape((-1)),
-             np.zeros((28, 28)).reshape((-1))])
+            [np.ones((28, 28)).reshape((-1)), np.zeros((28, 28)).reshape((-1))]
+        )
 
         diff_a = (abs(A_target1 - A_calc)).max() < 1e-4
         diff_b = (abs(A_target2 - A_calc)).max() < 1e-4
-        self.assertTrue(diff_a or diff_b,
-                        msg='calculate_A did not produce expected output.')
+        self.assertTrue(
+            diff_a or diff_b,
+            msg="calculate_A did not produce expected output.",
+        )
```

### Comparing `underactuated-2023.3.2/underactuated/exercises/pend/test_vibrating_pendulum.py` & `underactuated-2023.4.17/underactuated/exercises/pend/test_vibrating_pendulum.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 import unittest
+
 import timeout_decorator
 from gradescope_utils.autograder_utils.decorators import weight
 
 
 class TestVibratingPendulum(unittest.TestCase):
-
     def __init__(self, test_name, notebook_locals):
         super().__init__(test_name)
         self.notebook_locals = notebook_locals
 
     @weight(8)
-    @timeout_decorator.timeout(5.)
+    @timeout_decorator.timeout(5.0)
     def test_q1_pendulum_controller(self):
         """Test pendulum controller"""
         # note: all prints here go to the output item in the json file
 
         # the response must be monotonically increasing
-        theta_dot = self.notebook_locals['log'].data()[-1, :]
+        theta_dot = self.notebook_locals["log"].data()[-1, :]
         self.assertTrue(
             all(i <= j + 1e-4 for i, j in zip(theta_dot, theta_dot[1:])),
-            msg='theta_dot(t) is decreasing.',
+            msg="theta_dot(t) is decreasing.",
         )
 
         # final theta dot in [.99, 1.001]
         self.assertLessEqual(
             theta_dot[-1],
             1.001,
-            msg='theta_dot(t=10) = {} > 1.001'.format(theta_dot[-1]),
+            msg="theta_dot(t=10) = {} > 1.001".format(theta_dot[-1]),
         )
         self.assertGreaterEqual(
             theta_dot[-1],
-            .99,
-            msg='theta_dot(t=10) = {} < 0.99'.format(theta_dot[-1]),
+            0.99,
+            msg="theta_dot(t=10) = {} < 0.99".format(theta_dot[-1]),
         )
```

### Comparing `underactuated-2023.3.2/underactuated/exercises/planning/test_rrt_planning.py` & `underactuated-2023.4.17/underactuated/exercises/planning/test_rrt_planning.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,93 +1,96 @@
 import unittest
+
+import numpy as np
 import timeout_decorator
 from gradescope_utils.autograder_utils.decorators import weight
-import numpy as np
 
 
 class TestRRTPlanning(unittest.TestCase):
-
     def __init__(self, test_name, notebook_locals):
         super().__init__(test_name)
         self.notebook_locals = notebook_locals
 
     @weight(7)
-    @timeout_decorator.timeout(1.)
+    @timeout_decorator.timeout(1.0)
     def test1_rrt_path(self):
         """Test RRT"""
         # load locals
-        RRT = self.notebook_locals['RRT']
+        RRT = self.notebook_locals["RRT"]
 
         start = np.array([11, 0])
         goal = np.array([6, 8])
 
         obstacles = [
             np.array([9, 6, 2]),
             np.array([9, 8, 1]),
             np.array([9, 10, 2]),
             np.array([4, 5, 2]),
             np.array([7, 5, 2]),
-            np.array([4, 10, 1])
+            np.array([4, 10, 1]),
         ]
 
         bounds = np.array([-2, 15])
 
         np.random.seed(7)
-        rrt = RRT(start=start,
-                  goal=goal,
-                  bounds=bounds,
-                  obstacle_list=obstacles)
+        rrt = RRT(
+            start=start, goal=goal, bounds=bounds, obstacle_list=obstacles
+        )
         path = rrt.plan()
 
-        self.assertFalse(path is None,
-                         'The plan method is not implemented correctly')
+        self.assertFalse(
+            path is None, "The plan method is not implemented correctly"
+        )
 
         np.testing.assert_array_almost_equal(
             start,
             path[-1],
-            err_msg='The start location of the path is not the correct '
-            + 'start location')
+            err_msg="The start location of the path is not the correct "
+            + "start location",
+        )
 
         np.testing.assert_array_almost_equal(
             goal,
             path[0],
-            err_msg='The goal location of the path is not the correct '
-            + 'goal location')
+            err_msg="The goal location of the path is not the correct "
+            + "goal location",
+        )
 
         for i in range(len(path) - 1):
-            is_in_collision = RRT.collision(RRT.Node(path[i]),
-                                            RRT.Node(path[i + 1]), obstacles)
-            self.assertFalse(is_in_collision,
-                             'The path is colliding with obstacles')
+            is_in_collision = RRT.collision(
+                RRT.Node(path[i]), RRT.Node(path[i + 1]), obstacles
+            )
+            self.assertFalse(
+                is_in_collision, "The path is colliding with obstacles"
+            )
 
     @weight(7)
-    @timeout_decorator.timeout(20.)
+    @timeout_decorator.timeout(20.0)
     def test2_rrt_star_path(self):
         """Test RRT*"""
         # load locals
-        RRTStar = self.notebook_locals['RRTStar']
+        RRTStar = self.notebook_locals["RRTStar"]
 
         start = np.array([11, 0])
         goal = np.array([6, 8])
 
         obstacles = [
             np.array([9, 6, 2]),
             np.array([9, 8, 1]),
             np.array([9, 10, 2]),
             np.array([4, 5, 2]),
             np.array([7, 5, 2]),
-            np.array([4, 10, 1])
+            np.array([4, 10, 1]),
         ]
 
         bounds = np.array([-2, 15])
 
-        rrt_star = RRTStar(start=start,
-                           goal=goal,
-                           bounds=bounds,
-                           obstacle_list=obstacles)
+        rrt_star = RRTStar(
+            start=start, goal=goal, bounds=bounds, obstacle_list=obstacles
+        )
 
         # Check the choose_parent method
         node1 = rrt_star.Node(np.array([12, 0]))
         node1 = rrt_star.steer(rrt_star.start, node1)
         node1.cost = 10
         node2 = rrt_star.Node(np.array([10, 0]))
         node2 = rrt_star.steer(rrt_star.start, node2)
@@ -99,71 +102,83 @@
         rrt_star.node_list = [node1, node2, node3]
         node4 = rrt_star.steer(rrt_star.start, node4)
         near_inds = rrt_star.near_nodes_inds(node4)
         node4 = rrt_star.choose_parent(node4, near_inds)
 
         self.assertFalse(
             node4.parent is None,
-            'The choose_parent method is not implemented correctly')
+            "The choose_parent method is not implemented correctly",
+        )
 
         self.assertFalse(
             np.linalg.norm(node3.p - node4.parent.p) < 1e-5,
-            'The choose_parent method does not check for collisions')
+            "The choose_parent method does not check for collisions",
+        )
 
         np.testing.assert_array_almost_equal(
             node4.parent.p,
             node1.p,
-            err_msg='The choose_parent method does not seem to'
-            + ' select the best parent node')
+            err_msg="The choose_parent method does not seem to"
+            + " select the best parent node",
+        )
 
         # Check the rewiring method
         node4 = rrt_star.steer(rrt_star.start, node4)
         rrt_star.rewire(node4, near_inds)
         np.testing.assert_array_almost_equal(
             node1.parent.p,
             node4.p,
-            err_msg='The rewiring method does not rewire the correct nodes')
+            err_msg="The rewiring method does not rewire the correct nodes",
+        )
 
         node3.cost = 100
         node4 = rrt_star.steer(rrt_star.start, node4)
         rrt_star.rewire(node4, near_inds)
         self.assertFalse(
             np.linalg.norm(node3.parent.p - node4.p) < 1e-5,
-            'The rewiring method does not check for collision')
+            "The rewiring method does not check for collision",
+        )
 
         np.random.seed(7)
-        rrt_star = RRTStar(start=start,
-                           goal=goal,
-                           bounds=bounds,
-                           obstacle_list=obstacles,
-                           goal_sample_rate=0.0,
-                           max_iter=300)
+        rrt_star = RRTStar(
+            start=start,
+            goal=goal,
+            bounds=bounds,
+            obstacle_list=obstacles,
+            goal_sample_rate=0.0,
+            max_iter=300,
+        )
         path, _ = rrt_star.plan()
 
         np.testing.assert_array_almost_equal(
             start,
             path[-1],
-            err_msg='The start location of the path is not the correct '
-            + 'start location')
+            err_msg="The start location of the path is not the correct "
+            + "start location",
+        )
 
         np.testing.assert_array_almost_equal(
             goal,
             path[0],
-            err_msg='The goal location of the path is not the correct '
-            + 'goal location')
+            err_msg="The goal location of the path is not the correct "
+            + "goal location",
+        )
 
         for i in range(len(path) - 1):
-            is_in_collision = RRTStar.collision(RRTStar.Node(path[i]),
-                                                RRTStar.Node(path[i + 1]),
-                                                obstacles)
-            self.assertFalse(is_in_collision,
-                             'The path is colliding with obstacles')
+            is_in_collision = RRTStar.collision(
+                RRTStar.Node(path[i]), RRTStar.Node(path[i + 1]), obstacles
+            )
+            self.assertFalse(
+                is_in_collision, "The path is colliding with obstacles"
+            )
 
         def path_cost(path):
             total = 0
             for i in range(len(path) - 1):
                 total += np.linalg.norm(path[i] - path[i + 1])
             return total
 
         path_length = path_cost(path)
-        self.assertTrue(path_length < 17.5,
-                        'Length of the path={} > 17.5'.format(path_length))
+        self.assertTrue(
+            path_length < 17.5,
+            "Length of the path={} > 17.5".format(path_length),
+        )
```

### Comparing `underactuated-2023.3.2/underactuated/exercises/sysid/test_glider_sysid.py` & `underactuated-2023.4.17/underactuated/exercises/sysid/test_glider_sysid.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,50 +1,50 @@
 import unittest
+
 import timeout_decorator
 from gradescope_utils.autograder_utils.decorators import weight
 
 
 class TestGliderSysid(unittest.TestCase):
-
     def __init__(self, test_name, notebook_locals):
         super().__init__(test_name)
         self.notebook_locals = notebook_locals
 
     @weight(3)
-    @timeout_decorator.timeout(20.)
+    @timeout_decorator.timeout(20.0)
     def test_lq_fit(self):
         """Test least squares fitting"""
         # note: all prints here go to the output item in the json file
 
         # the best config and best score should have the right values
-        best_config = self.notebook_locals['best_config']
-        best_score = self.notebook_locals['best_score']
-        self.assertFalse(best_config != 6, 'The chosen basis set is incorrect')
-        self.assertFalse(best_score != 63831, 'The best score is incorrect')
+        best_config = self.notebook_locals["best_config"]
+        best_score = self.notebook_locals["best_score"]
+        self.assertFalse(best_config != 6, "The chosen basis set is incorrect")
+        self.assertFalse(best_score != 63831, "The best score is incorrect")
 
     @weight(3)
-    @timeout_decorator.timeout(20.)
+    @timeout_decorator.timeout(20.0)
     def test_basis_dynamics(self):
         """Test basis function dynamics"""
         # note: all prints here go to the output item in the json file
-        trajectories_fit = self.notebook_locals['trajectories_fit']
+        trajectories_fit = self.notebook_locals["trajectories_fit"]
         last_x = trajectories_fit[0][-1][0]
         last_z = trajectories_fit[0][-1][1]
         last_th = trajectories_fit[0][-1][2]
-        self.assertLessEqual(last_x,
-                             3.36,
-                             msg='Simulated trajectory x is incorrect')
-        self.assertGreaterEqual(last_x,
-                                3.34,
-                                msg='Simulated trajectory x is incorrect')
-        self.assertLessEqual(last_z,
-                             5.10,
-                             msg='Simulated trajectory z is incorrect')
-        self.assertGreaterEqual(last_z,
-                                4.99,
-                                msg='Simulated trajectory z is incorrect')
-        self.assertLessEqual(last_th,
-                             -0.52,
-                             msg='Simulated trajectory theta is incorrect')
-        self.assertGreaterEqual(last_th,
-                                -0.54,
-                                msg='Simulated trajectory theta is incorrect')
+        self.assertLessEqual(
+            last_x, 3.36, msg="Simulated trajectory x is incorrect"
+        )
+        self.assertGreaterEqual(
+            last_x, 3.34, msg="Simulated trajectory x is incorrect"
+        )
+        self.assertLessEqual(
+            last_z, 5.10, msg="Simulated trajectory z is incorrect"
+        )
+        self.assertGreaterEqual(
+            last_z, 4.99, msg="Simulated trajectory z is incorrect"
+        )
+        self.assertLessEqual(
+            last_th, -0.52, msg="Simulated trajectory theta is incorrect"
+        )
+        self.assertGreaterEqual(
+            last_th, -0.54, msg="Simulated trajectory theta is incorrect"
+        )
```

### Comparing `underactuated-2023.3.2/underactuated/exercises/sysid/test_linear_sysid.py` & `underactuated-2023.4.17/underactuated/exercises/sysid/test_linear_sysid.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,61 +1,70 @@
 import unittest
+
+import numpy as np
 import timeout_decorator
 from gradescope_utils.autograder_utils.decorators import weight
-import numpy as np
 
 
 class TestLinearSysid(unittest.TestCase):
-
     def __init__(self, test_name, notebook_locals):
         super().__init__(test_name)
         self.notebook_locals = notebook_locals
 
     @weight(3)
-    @timeout_decorator.timeout(20.)
+    @timeout_decorator.timeout(20.0)
     def test_L2_regression(self):
         """Test L2 regression"""
-        Ahat = self.notebook_locals['Ahat_2norm']
-        Bhat = self.notebook_locals['Bhat_2norm']
-        X = self.notebook_locals['X']
-        U = self.notebook_locals['U']
+        Ahat = self.notebook_locals["Ahat_2norm"]
+        Bhat = self.notebook_locals["Bhat_2norm"]
+        X = self.notebook_locals["X"]
+        U = self.notebook_locals["U"]
         res = Ahat @ X[:, :-1] + Bhat @ U[:, :-1] - X[:, 1:]
         self.assertLessEqual(
-            np.sum(res**2), 6e-7,
-            'The residual for 2-norm minimization is too high!')
+            np.sum(res**2),
+            6e-7,
+            "The residual for 2-norm minimization is too high!",
+        )
 
     @weight(3)
-    @timeout_decorator.timeout(20.)
+    @timeout_decorator.timeout(20.0)
     def test_Linf_regression(self):
         """Test L infinite regression"""
-        Ahat = self.notebook_locals['Ahat_infnorm']
-        Bhat = self.notebook_locals['Bhat_infnorm']
-        X = self.notebook_locals['X']
-        U = self.notebook_locals['U']
+        Ahat = self.notebook_locals["Ahat_infnorm"]
+        Bhat = self.notebook_locals["Bhat_infnorm"]
+        X = self.notebook_locals["X"]
+        U = self.notebook_locals["U"]
         res = Ahat @ X[:, :-1] + Bhat @ U[:, :-1] - X[:, 1:]
         residual = np.sum(np.max(np.abs(res), axis=0))
         self.assertLessEqual(
-            residual, 0.02,
-            'The residual for infinity-norm minimization is too high!')
+            residual,
+            0.02,
+            "The residual for infinity-norm minimization is too high!",
+        )
 
-        obj_infnorm = self.notebook_locals['obj_infnorm']
+        obj_infnorm = self.notebook_locals["obj_infnorm"]
         self.assertLessEqual(
-            np.abs(obj_infnorm - residual), 0.1,
-            'Objective from optimizer and empirical evaluations are different!')
+            np.abs(obj_infnorm - residual),
+            0.1,
+            "Objective from optimizer and empirical evaluations are different!",
+        )
 
     @weight(3)
-    @timeout_decorator.timeout(20.)
+    @timeout_decorator.timeout(20.0)
     def test_L1_regression(self):
         """Test L1 regression"""
-        Ahat = self.notebook_locals['Ahat_1norm']
-        Bhat = self.notebook_locals['Bhat_1norm']
-        X = self.notebook_locals['X']
-        U = self.notebook_locals['U']
+        Ahat = self.notebook_locals["Ahat_1norm"]
+        Bhat = self.notebook_locals["Bhat_1norm"]
+        X = self.notebook_locals["X"]
+        U = self.notebook_locals["U"]
         res = Ahat @ X[:, :-1] + Bhat @ U[:, :-1] - X[:, 1:]
         residual = np.sum(np.abs(res))
         self.assertLessEqual(
-            residual, 0.04, 'The residual for 1-norm minimization is too high!')
+            residual, 0.04, "The residual for 1-norm minimization is too high!"
+        )
 
-        obj_1norm = self.notebook_locals['obj_1norm']
+        obj_1norm = self.notebook_locals["obj_1norm"]
         self.assertLessEqual(
-            np.abs(obj_1norm - residual), 0.1,
-            'Objective from optimizer and empirical evaluations are different!')
+            np.abs(obj_1norm - residual),
+            0.1,
+            "Objective from optimizer and empirical evaluations are different!",
+        )
```

### Comparing `underactuated-2023.3.2/underactuated/exercises/trajopt/test_ilqr_driving.py` & `underactuated-2023.4.17/underactuated/exercises/trajopt/test_ilqr_driving.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,56 +1,62 @@
 import unittest
+
+import numpy as np
 import timeout_decorator
 from gradescope_utils.autograder_utils.decorators import weight
-import numpy as np
 
 
 class TestIlqrDriving(unittest.TestCase):
-
     def __init__(self, test_name, notebook_locals):
         super().__init__(test_name)
         self.notebook_locals = notebook_locals
 
     @weight(1)
-    @timeout_decorator.timeout(1.)
+    @timeout_decorator.timeout(1.0)
     def test1_discrete_dynamics(self):
         """Test discrete_dynamics"""
         # load locals
-        f = self.notebook_locals['discrete_dynamics']
+        f = self.notebook_locals["discrete_dynamics"]
 
         f_target = [
             np.array(
-                [0.14181286, 0.81062987, 0.54580749, 0.77731476, 1.02810156]),
+                [0.14181286, 0.81062987, 0.54580749, 0.77731476, 1.02810156]
+            ),
             np.array([0.131663, 0.300996, 0.57034388, 0.71732411, 0.81033267]),
             np.array(
-                [0.33233256, 0.91916814, 0.27416228, 0.45461388, 0.99126091]),
+                [0.33233256, 0.91916814, 0.27416228, 0.45461388, 0.99126091]
+            ),
             np.array(
-                [1.02770659, 0.27770476, 0.56066881, 0.96146963, 0.20821043]),
-            np.array([0.71706372, 0.47773599, 0.22401885, 0.538506, 0.40897373])
+                [1.02770659, 0.27770476, 0.56066881, 0.96146963, 0.20821043]
+            ),
+            np.array(
+                [0.71706372, 0.47773599, 0.22401885, 0.538506, 0.40897373]
+            ),
         ]
 
         np.random.seed(7)
         n_rands = 5
         f_eval = []
         for i in range(n_rands):
             x = np.random.rand(5)
             u = np.random.rand(2)
             f_eval = f(x, u)
             np.testing.assert_array_almost_equal(
                 f_eval,
                 f_target[i],
-                err_msg='The discrete dynamics are incorrect. '
-                f'Expected output {f_target[i]} with x={x} and u={u}')
+                err_msg="The discrete dynamics are incorrect. "
+                f"Expected output {f_target[i]} with x={x} and u={u}",
+            )
 
     @weight(1)
-    @timeout_decorator.timeout(1.)
+    @timeout_decorator.timeout(1.0)
     def test2_rollout(self):
         """Test rollout"""
         # load locals
-        f = self.notebook_locals['rollout']
+        f = self.notebook_locals["rollout"]
 
         f_target_test_target = [
             0.36531949939751773,
             2.25991775105549,
             -0.05889795147375571,
             0.5476245815855634,
             0.8066768897676444,
@@ -59,133 +65,151 @@
         np.random.seed(7)
         n_rands = 5
         for i in range(n_rands):
             N = 5
             n_u = 2
             x0 = np.array([1, 0, 0, 1, 0])
             u_trj = np.random.randn(N - 1, n_u) * 0.4
-            f_eval_test = np.random.randn(N) @ f(x0, u_trj) @ np.random.randn(N)
-            msg = f'The discrete dynamics are incorrect.' + \
-                'Expected output {f_target_test_target[i]} got {f_eval_test}'
-            self.assertAlmostEqual(f_eval_test,
-                                   f_target_test_target[i],
-                                   msg=msg)
+            f_eval_test = (
+                np.random.randn(N) @ f(x0, u_trj) @ np.random.randn(N)
+            )
+            msg = (
+                f"The discrete dynamics are incorrect."
+                + "Expected output {f_target_test_target[i]} got {f_eval_test}"
+            )
+            self.assertAlmostEqual(
+                f_eval_test, f_target_test_target[i], msg=msg
+            )
 
     @weight(1)
-    @timeout_decorator.timeout(1.)
+    @timeout_decorator.timeout(1.0)
     def test3_cost_trj(self):
         """Test cost_trj"""
         # load locals
-        f = self.notebook_locals['cost_trj']
+        f = self.notebook_locals["cost_trj"]
 
         f_target = [
-            29.946731429035616, 34.805336401404986, 27.626872505986434,
-            33.25730851334137, 33.83897480138296
+            29.946731429035616,
+            34.805336401404986,
+            27.626872505986434,
+            33.25730851334137,
+            33.83897480138296,
         ]
 
         np.random.seed(7)
         n_rands = 5
         f_eval = []
         for i in range(n_rands):
             N = 5
             n_u = 2
             n_x = 5
-            x0 = np.array([1, 0, 0, 1, 0])
+            np.array([1, 0, 0, 1, 0])
             u_trj = np.random.randn(N - 1, n_u) * 0.4
             x_trj = np.random.randn(N, n_x) * 0.4
             f_eval = f(x_trj, u_trj)
             np.testing.assert_almost_equal(
                 f_eval,
                 f_target[i],
-                err_msg='The cost_trj function is incorrect. '
-                f'Expected output {f_target[i]} with x_trj=\n{x_trj}'
-                f' and u=\n{u_trj}')
+                err_msg="The cost_trj function is incorrect. "
+                f"Expected output {f_target[i]} with x_trj=\n{x_trj}"
+                f" and u=\n{u_trj}",
+            )
 
     @weight(5)
-    @timeout_decorator.timeout(1.)
+    @timeout_decorator.timeout(1.0)
     def test4_Q_terms(self):
         """Test Q_terms"""
         # load locals
-        Q_terms = self.notebook_locals['Q_terms']
-        derivs = self.notebook_locals['derivs']
+        Q_terms = self.notebook_locals["Q_terms"]
+        derivs = self.notebook_locals["derivs"]
 
         np.random.seed(7)
         x = np.random.rand(5)
         u = np.random.rand(2)
 
         l_x, l_u, l_xx, l_ux, l_uu, f_x, f_u = derivs.stage(x, u)
         V_x, V_xx = derivs.final(x + 0.1)
-        Q_x, Q_u, Q_xx, Q_ux, Q_uu = Q_terms(l_x, l_u, l_xx, l_ux, l_uu, f_x,
-                                             f_u, V_x, V_xx)
-
-        Q_x_test_val = (Q_x @ np.random.randn(Q_x.shape[0]))
-        Q_u_test_val = (Q_u @ np.random.randn(Q_u.shape[0]))
-        Q_xx_test_val = (np.random.randn(Q_xx.shape[0]) @ Q_xx
-                         @ np.random.randn(Q_xx.shape[0]))
-        Q_ux_test_val = (np.random.randn(Q_ux.shape[0]) @ Q_ux
-                         @ np.random.randn(Q_ux.shape[1]))
-        Q_uu_test_val = (np.random.randn(Q_uu.shape[0]) @ Q_uu
-                         @ np.random.randn(Q_uu.shape[0]))
+        Q_x, Q_u, Q_xx, Q_ux, Q_uu = Q_terms(
+            l_x, l_u, l_xx, l_ux, l_uu, f_x, f_u, V_x, V_xx
+        )
+
+        Q_x_test_val = Q_x @ np.random.randn(Q_x.shape[0])
+        Q_u_test_val = Q_u @ np.random.randn(Q_u.shape[0])
+        Q_xx_test_val = (
+            np.random.randn(Q_xx.shape[0])
+            @ Q_xx
+            @ np.random.randn(Q_xx.shape[0])
+        )
+        Q_ux_test_val = (
+            np.random.randn(Q_ux.shape[0])
+            @ Q_ux
+            @ np.random.randn(Q_ux.shape[1])
+        )
+        Q_uu_test_val = (
+            np.random.randn(Q_uu.shape[0])
+            @ Q_uu
+            @ np.random.randn(Q_uu.shape[0])
+        )
 
         Q_x_test_target = 1.1817013977437874
         Q_u_test_target = -0.1716142906672626
         Q_xx_test_target = 0.5337352394014466
         Q_ux_test_target = 0.5156605288974515
         Q_uu_test_target = -0.28166353613679074
 
-        self.assertAlmostEqual(Q_x_test_val,
-                               Q_x_test_target,
-                               msg="Incorrect Q_x")
-        self.assertAlmostEqual(Q_u_test_val,
-                               Q_u_test_target,
-                               msg="Incorrect Q_u")
-        self.assertAlmostEqual(Q_xx_test_val,
-                               Q_xx_test_target,
-                               msg="Incorrect Q_xx")
-        self.assertAlmostEqual(Q_ux_test_val,
-                               Q_ux_test_target,
-                               msg="Incorrect Q_ux")
-        self.assertAlmostEqual(Q_uu_test_val,
-                               Q_uu_test_target,
-                               msg="Incorrect Q_uu")
+        self.assertAlmostEqual(
+            Q_x_test_val, Q_x_test_target, msg="Incorrect Q_x"
+        )
+        self.assertAlmostEqual(
+            Q_u_test_val, Q_u_test_target, msg="Incorrect Q_u"
+        )
+        self.assertAlmostEqual(
+            Q_xx_test_val, Q_xx_test_target, msg="Incorrect Q_xx"
+        )
+        self.assertAlmostEqual(
+            Q_ux_test_val, Q_ux_test_target, msg="Incorrect Q_ux"
+        )
+        self.assertAlmostEqual(
+            Q_uu_test_val, Q_uu_test_target, msg="Incorrect Q_uu"
+        )
 
     @weight(3)
-    @timeout_decorator.timeout(1.)
+    @timeout_decorator.timeout(1.0)
     def test5_gains(self):
         """Test gains"""
         # load locals
-        gains = self.notebook_locals['gains']
+        gains = self.notebook_locals["gains"]
 
         np.random.seed(8)
         Q_u = np.random.randn(2)
         Q_uu = np.random.randn(2, 2)
         Q_uu = 0.5 * (Q_uu + Q_uu.T)
         Q_ux = np.random.randn(2, 5)
         k, K = gains(Q_uu, Q_u, Q_ux)
 
         test_inputs = 10 * np.random.randn(k.shape[0], 5)
 
         k_test_val = (k @ test_inputs).sum()
         K_test_val = (test_inputs.T @ K).sum()
 
-        self.assertAlmostEqual(k_test_val,
-                               10.712481345027399,
-                               msg="Incorrect k gain")
-
-        self.assertAlmostEqual(K_test_val,
-                               -12.949530490536842,
-                               msg="Incorrect K gain")
+        self.assertAlmostEqual(
+            k_test_val, 10.712481345027399, msg="Incorrect k gain"
+        )
+
+        self.assertAlmostEqual(
+            K_test_val, -12.949530490536842, msg="Incorrect K gain"
+        )
 
     @weight(3)
-    @timeout_decorator.timeout(1.)
+    @timeout_decorator.timeout(1.0)
     def test6_V_terms(self):
         """Test V_terms"""
         # load locals
-        V_terms = self.notebook_locals['V_terms']
-        gains = self.notebook_locals['gains']
+        V_terms = self.notebook_locals["V_terms"]
+        gains = self.notebook_locals["gains"]
 
         np.random.seed(7)
         Q_x = np.random.randn(5)
         Q_u = np.random.randn(2)
         Q_uu = np.random.randn(2, 2)
         Q_uu = 0.5 * (Q_uu + Q_uu.T)
         Q_ux = np.random.randn(2, 5)
@@ -195,54 +219,56 @@
 
         V_x, V_xx = V_terms(Q_x, Q_u, Q_xx, Q_ux, Q_uu, K, k)
         test_inputs = np.random.randn(V_x.shape[0])
 
         V_x_test_val = V_x @ test_inputs
         V_xx_test_val = test_inputs @ V_xx @ test_inputs
 
-        self.assertAlmostEqual(V_x_test_val,
-                               -2.113959925580339,
-                               msg="Incorrect V_x")
-
-        self.assertAlmostEqual(V_xx_test_val,
-                               35.931091753768,
-                               msg="Incorrect V_xx")
+        self.assertAlmostEqual(
+            V_x_test_val, -2.113959925580339, msg="Incorrect V_x"
+        )
+
+        self.assertAlmostEqual(
+            V_xx_test_val, 35.931091753768, msg="Incorrect V_xx"
+        )
 
         # this tests whether the student simplified the V_terms expression
         k2, K2 = 10 * np.random.randn(*k.shape), 10 * np.random.randn(*K.shape)
         V_x2, V_xx2 = V_terms(Q_x, Q_u, Q_xx, Q_ux, Q_uu, K2, k2)
 
         V_x2_test_val = V_x2 @ test_inputs
         V_xx2_test_val = test_inputs @ V_xx2 @ test_inputs
 
         self.assertNotAlmostEqual(
             V_x2_test_val,
             2.484304411129088,
             msg="""It appears you may have simplified the expression for V_x.
-            Do not do this""")
+            Do not do this""",
+        )
         self.assertNotAlmostEqual(
             V_xx2_test_val,
             265.0164583112695,
             msg="""It appears you may have simplified the expression for V_xx.
-            Do not do this""")
+            Do not do this""",
+        )
 
-        self.assertAlmostEqual(V_x2_test_val,
-                               -6.043415622930539,
-                               msg="Incorrect V_x")
-
-        self.assertAlmostEqual(V_xx2_test_val,
-                               -52.01732694080634,
-                               msg="Incorrect V_xx")
+        self.assertAlmostEqual(
+            V_x2_test_val, -6.043415622930539, msg="Incorrect V_x"
+        )
+
+        self.assertAlmostEqual(
+            V_xx2_test_val, -52.01732694080634, msg="Incorrect V_xx"
+        )
 
     @weight(2)
-    @timeout_decorator.timeout(1.)
+    @timeout_decorator.timeout(1.0)
     def test7_forward_pass(self):
         """Test forward_pass"""
         # load locals
-        forward_pass = self.notebook_locals['forward_pass']
+        forward_pass = self.notebook_locals["forward_pass"]
 
         np.random.seed(7)
         N = 5
         n_u = 2
         n_x = 5
         u_trj = np.random.randn(N - 1, n_u)
         x_trj = np.random.randn(N, n_x)
@@ -252,47 +278,48 @@
 
         x_test = np.random.randn(x_trj_new.shape[0])
         u_test = np.random.randn(u_trj_new.shape[0])
 
         x_trj_new_test_val = x_test @ x_trj_new @ x_test
         u_trj_new_test_val = (u_test @ u_trj_new).sum()
 
-        self.assertAlmostEqual(x_trj_new_test_val,
-                               -1.0615491271322297,
-                               msg="Incorrect x_trj_new")
-
-        self.assertAlmostEqual(u_trj_new_test_val,
-                               -10.649763284585609,
-                               msg="Incorrect u_trj_new")
+        self.assertAlmostEqual(
+            x_trj_new_test_val, -1.0615491271322297, msg="Incorrect x_trj_new"
+        )
+
+        self.assertAlmostEqual(
+            u_trj_new_test_val, -10.649763284585609, msg="Incorrect u_trj_new"
+        )
 
     @weight(2)
-    @timeout_decorator.timeout(1.)
+    @timeout_decorator.timeout(1.0)
     def test8_backward_pass(self):
         """Test backward_pass"""
         # load locals
-        backward_pass = self.notebook_locals['backward_pass']
+        backward_pass = self.notebook_locals["backward_pass"]
 
         np.random.seed(7)
         N = 5
         n_u = 2
         n_x = 5
-        k = np.random.randn(2)
-        K = np.random.randn(2, 5)
+        np.random.randn(2)
+        np.random.randn(2, 5)
         u_trj = np.random.randn(N - 1, n_u)
         x_trj = np.random.randn(N, n_x)
 
         k_trj, K_trj, _ = backward_pass(x_trj, u_trj, 100.0)
 
         r_test = 10 * np.random.randn(k_trj.shape[1])
         l_test = 10 * np.random.randn(k_trj.shape[0])
 
         k_trj_test_val = l_test @ k_trj @ r_test
-        K_trj_test_val = np.einsum("i, ijk, j -> k", l_test, K_trj,
-                                   r_test).sum()
-
-        self.assertAlmostEqual(k_trj_test_val,
-                               -5.380572857461254,
-                               msg="Incorrect k_trj")
-
-        self.assertAlmostEqual(K_trj_test_val,
-                               3.770894929116537,
-                               msg="Incorrect K_trj")
+        K_trj_test_val = np.einsum(
+            "i, ijk, j -> k", l_test, K_trj, r_test
+        ).sum()
+
+        self.assertAlmostEqual(
+            k_trj_test_val, -5.380572857461254, msg="Incorrect k_trj"
+        )
+
+        self.assertAlmostEqual(
+            K_trj_test_val, 3.770894929116537, msg="Incorrect K_trj"
+        )
```

### Comparing `underactuated-2023.3.2/underactuated/exercises/trajopt/test_orbital_transfer.py` & `underactuated-2023.4.17/underactuated/exercises/trajopt/test_orbital_transfer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,123 +1,133 @@
 import unittest
+
+import numpy as np
 import timeout_decorator
 from gradescope_utils.autograder_utils.decorators import weight
-import numpy as np
 
 
 class TestOrbitalTransfer(unittest.TestCase):
-
     def __init__(self, test_name, notebook_locals):
         super().__init__(test_name)
         self.notebook_locals = notebook_locals
 
     def trajopt_feasibility(self):
         """Test feasibility of the trajopt solution"""
         # load locals
-        universe = self.notebook_locals['universe']
-        thrust = self.notebook_locals['thrust_opt']
-        state = self.notebook_locals['state_opt']
-        time_steps = self.notebook_locals['time_steps']
-        time_interval = self.notebook_locals['time_interval']
+        universe = self.notebook_locals["universe"]
+        thrust = self.notebook_locals["thrust_opt"]
+        state = self.notebook_locals["state_opt"]
+        time_steps = self.notebook_locals["time_steps"]
+        time_interval = self.notebook_locals["time_interval"]
 
         # initial state in Earth orbit
-        residuals = universe.constraint_state_to_orbit(state[0], 'Earth')
+        residuals = universe.constraint_state_to_orbit(state[0], "Earth")
         np.testing.assert_array_almost_equal(
             residuals,
             np.zeros(residuals.shape),
-            err_msg='The initial state in not on the Earth orbit.')
+            err_msg="The initial state in not on the Earth orbit.",
+        )
 
         # final state in Mars orbit
-        residuals = universe.constraint_state_to_orbit(state[-1], 'Mars')
+        residuals = universe.constraint_state_to_orbit(state[-1], "Mars")
         np.testing.assert_array_almost_equal(
             residuals,
             np.zeros(residuals.shape),
             # decimal=4,
-            err_msg='The final state in not on the Mars orbit.')
+            err_msg="The final state in not on the Mars orbit.",
+        )
 
         # discretized dynamics
         for t in range(time_steps):
             residuals = universe.rocket_discrete_dynamics(
-                state[t], state[t + 1], thrust[t], time_interval)
+                state[t], state[t + 1], thrust[t], time_interval
+            )
             np.testing.assert_array_almost_equal(
                 residuals,
                 np.zeros(residuals.shape),
-                err_msg=f'Discrete dynamics at time step {t} is not verified.')
+                err_msg=f"Discrete dynamics at time step {t} is not verified.",
+            )
 
     @weight(3)
-    @timeout_decorator.timeout(1.)
+    @timeout_decorator.timeout(1.0)
     def test_thrust_limits(self):
         """Test thrust limits"""
         # check feasibility first
         self.trajopt_feasibility()
 
         # load locals
-        universe = self.notebook_locals['universe']
-        thrust = self.notebook_locals['thrust_opt']
-        time_steps = self.notebook_locals['time_steps']
+        universe = self.notebook_locals["universe"]
+        thrust = self.notebook_locals["thrust_opt"]
+        time_steps = self.notebook_locals["time_steps"]
 
         # check thrust limits
         tol = 1e-3
         thrust_limit = universe.rocket.thrust_limit
         for t in range(time_steps):
-            self.assertTrue(np.linalg.norm(thrust[t]) <= thrust_limit + tol,
-                            msg=f'Thrust limit violated at time step {t}.')
+            self.assertTrue(
+                np.linalg.norm(thrust[t]) <= thrust_limit + tol,
+                msg=f"Thrust limit violated at time step {t}.",
+            )
 
     @weight(3)
-    @timeout_decorator.timeout(1.)
+    @timeout_decorator.timeout(1.0)
     def test_velocity_limits(self):
         """Test velocity limits"""
         # check feasibility first
         self.trajopt_feasibility()
 
         # load locals
-        universe = self.notebook_locals['universe']
-        velocity = self.notebook_locals['state_opt'][:, 2:]
-        time_steps = self.notebook_locals['time_steps']
+        universe = self.notebook_locals["universe"]
+        velocity = self.notebook_locals["state_opt"][:, 2:]
+        time_steps = self.notebook_locals["time_steps"]
 
         # check velocity limits
         tol = 1e-3
         velocity_limit = universe.rocket.velocity_limit
         for t in range(time_steps + 1):
-            self.assertTrue(np.linalg.norm(velocity[t]) <= velocity_limit + tol,
-                            msg=f'Velocity limit violated at time step {t}.')
+            self.assertTrue(
+                np.linalg.norm(velocity[t]) <= velocity_limit + tol,
+                msg=f"Velocity limit violated at time step {t}.",
+            )
 
     @weight(6)
-    @timeout_decorator.timeout(1.)
+    @timeout_decorator.timeout(1.0)
     def test_asteroid_collision_limits(self):
         """Test asteroid collision"""
         # check feasibility first
         self.trajopt_feasibility()
 
         # load locals
-        universe = self.notebook_locals['universe']
-        state = self.notebook_locals['state_opt']
-        time_steps = self.notebook_locals['time_steps']
-        n_asteroids = self.notebook_locals['n_asteroids']
+        universe = self.notebook_locals["universe"]
+        state = self.notebook_locals["state_opt"]
+        time_steps = self.notebook_locals["time_steps"]
+        n_asteroids = self.notebook_locals["n_asteroids"]
 
         # avoid collision with asteroids
         tol = 1e-3
         for i in range(n_asteroids):
-            asteroid_orbit = universe.get_planet(f'Asteroid_{i}').orbit
+            asteroid_orbit = universe.get_planet(f"Asteroid_{i}").orbit
             for t in range(time_steps + 1):
-                p = universe.position_wrt_planet(state[t], f'Asteroid_{i}')
+                p = universe.position_wrt_planet(state[t], f"Asteroid_{i}")
                 self.assertTrue(
                     p.dot(p) >= asteroid_orbit**2 - tol,
-                    msg=f'Collision with asteroid {i} at time step {t}.')
+                    msg=f"Collision with asteroid {i} at time step {t}.",
+                )
 
     @weight(3)
-    @timeout_decorator.timeout(1.)
+    @timeout_decorator.timeout(1.0)
     def test_fuel_consumption_limits(self):
         """Test fuel consumption"""
         # check feasibility first
         self.trajopt_feasibility()
 
         # load locals
-        universe = self.notebook_locals['universe']
-        thrust = self.notebook_locals['thrust_opt']
-        time_interval = self.notebook_locals['time_interval']
+        self.notebook_locals["universe"]
+        thrust = self.notebook_locals["thrust_opt"]
+        time_interval = self.notebook_locals["time_interval"]
 
         # check maximum consumption
         consumption = time_interval * sum(t.dot(t) for t in thrust)
         self.assertTrue(
             consumption <= 250,
-            msg=f'Fuel consumption is {consumption}, greater than 250.')
+            msg=f"Fuel consumption is {consumption}, greater than 250.",
+        )
```

### Comparing `underactuated-2023.3.2/underactuated/exercises/trajopt/test_shooting_vs_transcription.py` & `underactuated-2023.4.17/underactuated/exercises/trajopt/test_shooting_vs_transcription.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,207 +1,302 @@
 import unittest
+
+import numpy as np
 import timeout_decorator
 from gradescope_utils.autograder_utils.decorators import weight
-import numpy as np
 
 
 class TestShootingVsTranscription(unittest.TestCase):
-
     def __init__(self, test_name, notebook_locals):
         super().__init__(test_name)
         self.notebook_locals = notebook_locals
 
     @weight(3)
-    @timeout_decorator.timeout(1.)
+    @timeout_decorator.timeout(1.0)
     def test_lost_bits_shooting(self):
         """Test number of bits lost with direct shooting"""
         # get list of lost bits
-        lost_bits = self.notebook_locals['lost_bits_shooting']
+        lost_bits = self.notebook_locals["lost_bits_shooting"]
 
         # check list length and types
         self.assertEqual(
-            len(lost_bits), 45,
-            'The list lost_bits_shooting must have length equal' + 'to 45.')
+            len(lost_bits),
+            45,
+            "The list lost_bits_shooting must have length equal" + "to 45.",
+        )
         bits_type = [isinstance(bits, (float, int)) for bits in lost_bits]
         self.assertTrue(
-            all(bits_type), 'Some entries in lost_bits_shooting are neither'
-            + 'floats nor ints.')
+            all(bits_type),
+            "Some entries in lost_bits_shooting are neither"
+            + "floats nor ints.",
+        )
 
         # check values
         lost_bits_shooting = [
-            0.0, 0.9543364613711909, 1.8123366596726525, 2.845325160323255,
-            3.997099761655346, 5.181146076477944, 6.367665432089994,
-            7.549745045378025, 8.727297345452408, 9.901650046513046,
-            11.074027866040504, 12.245271423678894, 13.415892162590488,
-            14.586181089218373, 15.75629682473095, 16.92632331212132,
-            18.096304057604645, 19.266261289075352, 20.436206266052793,
-            21.606144677268965, 22.776079410190473, 23.94601195116546,
-            25.115943085840197, 26.285873247157944, 27.455802687733357,
-            28.625731565680532, 29.795659987345097, 30.965588028826133,
-            32.13551574866848, 33.30544319406715, 34.47537039717343,
-            35.64529738697145, 36.81522421237407, 37.98515087701531,
-            39.15507737686514, 40.32500371458269, 41.49492968101353,
-            42.6648551872069, 43.83478032928076, 45.00470555237002,
-            46.174631383871656, 47.34456378440541, 48.52985492074265,
-            49.72208993747556, 50.8608777068896
+            0.0,
+            0.9543364613711909,
+            1.8123366596726525,
+            2.845325160323255,
+            3.997099761655346,
+            5.181146076477944,
+            6.367665432089994,
+            7.549745045378025,
+            8.727297345452408,
+            9.901650046513046,
+            11.074027866040504,
+            12.245271423678894,
+            13.415892162590488,
+            14.586181089218373,
+            15.75629682473095,
+            16.92632331212132,
+            18.096304057604645,
+            19.266261289075352,
+            20.436206266052793,
+            21.606144677268965,
+            22.776079410190473,
+            23.94601195116546,
+            25.115943085840197,
+            26.285873247157944,
+            27.455802687733357,
+            28.625731565680532,
+            29.795659987345097,
+            30.965588028826133,
+            32.13551574866848,
+            33.30544319406715,
+            34.47537039717343,
+            35.64529738697145,
+            36.81522421237407,
+            37.98515087701531,
+            39.15507737686514,
+            40.32500371458269,
+            41.49492968101353,
+            42.6648551872069,
+            43.83478032928076,
+            45.00470555237002,
+            46.174631383871656,
+            47.34456378440541,
+            48.52985492074265,
+            49.72208993747556,
+            50.8608777068896,
         ]
         for i, bits in enumerate(lost_bits):
-            self.assertAlmostEqual(bits,
-                                   lost_bits_shooting[i],
-                                   places=1,
-                                   msg='lost_bits_shooting are incorrect.')
+            self.assertAlmostEqual(
+                bits,
+                lost_bits_shooting[i],
+                places=1,
+                msg="lost_bits_shooting are incorrect.",
+            )
 
     @weight(4)
-    @timeout_decorator.timeout(1.)
+    @timeout_decorator.timeout(1.0)
     def test_Mb_diagonal_block(self):
         """Test construction of diagonal block of Mb"""
         # get function to construct the block
-        Mb_diagonal_block = self.notebook_locals['Mb_diagonal_block']
+        Mb_diagonal_block = self.notebook_locals["Mb_diagonal_block"]
 
         # test function directly on the problem data
-        A = np.array([[1, .5], [.5, 1]])
-        B = np.array([[0], [.5]])
+        A = np.array([[1, 0.5], [0.5, 1]])
+        B = np.array([[0], [0.5]])
         Q = np.array([[1, 0], [0, 0]])
         R = np.array([[1]])
 
         # run sudent function
         Mb_block = Mb_diagonal_block(A, B, Q, R).toarray()
 
         # correct solution for the fake data
-        Mb_block_target = np.array([
-            [-1, 0, 2, 0, 0, 1, .5, 0, 0],
-            [0, -1, 0, 0, 0, .5, 1, 0, 0],
-            [0, 0, 0, 0, 2, 0, .5, 0, 0],
-            [0, 0, 1, .5, 0, 0, 0, -1, 0],
-            [0, 0, .5, 1, .5, 0, 0, 0, -1],
-        ])
+        Mb_block_target = np.array(
+            [
+                [-1, 0, 2, 0, 0, 1, 0.5, 0, 0],
+                [0, -1, 0, 0, 0, 0.5, 1, 0, 0],
+                [0, 0, 0, 0, 2, 0, 0.5, 0, 0],
+                [0, 0, 1, 0.5, 0, 0, 0, -1, 0],
+                [0, 0, 0.5, 1, 0.5, 0, 0, 0, -1],
+            ]
+        )
         self.assertTrue(
             Mb_block.shape == Mb_block_target.shape,
-            'The matrix we got from Mb_diagonal_block has wrong dimensions.')
+            "The matrix we got from Mb_diagonal_block has wrong dimensions.",
+        )
         np.testing.assert_array_almost_equal(
             Mb_block,
             Mb_block_target,
-            err_msg='The function Mb_diagonal_block is incorrect on the '
-            + f'problem data A = {A}, B = {B}, Q = {Q}, and R = {R}.')
+            err_msg="The function Mb_diagonal_block is incorrect on the "
+            + f"problem data A = {A}, B = {B}, Q = {Q}, and R = {R}.",
+        )
 
         # test function directly on synthtic data
         A = np.arange(9).reshape(3, 3)
         B = np.arange(6).reshape(3, 2)
         Q = np.ones((3, 3)) * 2
         R = np.ones((2, 2)) * 3
 
         # run sudent function
         Mb_block = Mb_diagonal_block(A, B, Q, R).toarray()
 
         # correct solution for the fake data
-        Mb_block_target = np.array([
-            [-1, 0, 0, 4, 4, 4, 0, 0, 0, 3, 6, 0, 0, 0],
-            [0, -1, 0, 4, 4, 4, 0, 0, 1, 4, 7, 0, 0, 0],
-            [0, 0, -1, 4, 4, 4, 0, 0, 2, 5, 8, 0, 0, 0],
-            [0, 0, 0, 0, 0, 0, 6, 6, 0, 2, 4, 0, 0, 0],
-            [0, 0, 0, 0, 0, 0, 6, 6, 1, 3, 5, 0, 0, 0],
-            [0, 0, 0, 0, 1, 2, 0, 1, 0, 0, 0, -1, 0, 0],
-            [0, 0, 0, 3, 4, 5, 2, 3, 0, 0, 0, 0, -1, 0],
-            [0, 0, 0, 6, 7, 8, 4, 5, 0, 0, 0, 0, 0, -1],
-        ])
+        Mb_block_target = np.array(
+            [
+                [-1, 0, 0, 4, 4, 4, 0, 0, 0, 3, 6, 0, 0, 0],
+                [0, -1, 0, 4, 4, 4, 0, 0, 1, 4, 7, 0, 0, 0],
+                [0, 0, -1, 4, 4, 4, 0, 0, 2, 5, 8, 0, 0, 0],
+                [0, 0, 0, 0, 0, 0, 6, 6, 0, 2, 4, 0, 0, 0],
+                [0, 0, 0, 0, 0, 0, 6, 6, 1, 3, 5, 0, 0, 0],
+                [0, 0, 0, 0, 1, 2, 0, 1, 0, 0, 0, -1, 0, 0],
+                [0, 0, 0, 3, 4, 5, 2, 3, 0, 0, 0, 0, -1, 0],
+                [0, 0, 0, 6, 7, 8, 4, 5, 0, 0, 0, 0, 0, -1],
+            ]
+        )
         self.assertTrue(
             Mb_block.shape == Mb_block_target.shape,
-            'The matrix we got from Mb_diagonal_block has wrong dimensions.')
+            "The matrix we got from Mb_diagonal_block has wrong dimensions.",
+        )
         np.testing.assert_array_almost_equal(
             Mb_block,
             Mb_block_target,
-            err_msg='The function Mb_diagonal_block is incorrect on the '
-            + f'problem data A = {A}, B = {B}, Q = {Q}, and R = {R}.')
+            err_msg="The function Mb_diagonal_block is incorrect on the "
+            + f"problem data A = {A}, B = {B}, Q = {Q}, and R = {R}.",
+        )
 
     @weight(4)
-    @timeout_decorator.timeout(1.)
+    @timeout_decorator.timeout(1.0)
     def test_J_star_N_transcription(self):
         """Test value function direct transcription"""
         # get list of costs to go
-        J_star_N = self.notebook_locals['J_star_N_transcription']
+        J_star_N = self.notebook_locals["J_star_N_transcription"]
 
         # check list length and types
         self.assertEqual(
-            len(J_star_N), 45,
-            'The list J_star_N_transcription must have length'
-            + 'equal to 100.')
+            len(J_star_N),
+            45,
+            "The list J_star_N_transcription must have length"
+            + "equal to 100.",
+        )
         J_star_type = [isinstance(J, (float, int)) for J in J_star_N]
         self.assertTrue(
             all(J_star_type),
-            'Some entries in J_star_N_transcription are neither'
-            + 'floats nor ints.')
+            "Some entries in J_star_N_transcription are neither"
+            + "floats nor ints.",
+        )
 
         # check values
-        self._test_J_star(J_star_N, 'J_star_N_transcription is incorrect.')
+        self._test_J_star(J_star_N, "J_star_N_transcription is incorrect.")
 
     @weight(3)
-    @timeout_decorator.timeout(1.)
+    @timeout_decorator.timeout(1.0)
     def test_lost_bits_transcription(self):
         """Test number of bits lost with direct transcription"""
         # get list of lost bits
-        lost_bits = self.notebook_locals['lost_bits_transcription']
+        lost_bits = self.notebook_locals["lost_bits_transcription"]
 
         # check list length and types
         self.assertEqual(
-            len(lost_bits), 45,
-            'The list lost_bits_transcription must have length'
-            + 'equl to 100.')
+            len(lost_bits),
+            45,
+            "The list lost_bits_transcription must have length"
+            + "equl to 100.",
+        )
         bits_type = [isinstance(bits, (float, int)) for bits in lost_bits]
         self.assertTrue(
             all(bits_type),
-            'Some entries in lost_bits_transcription are neither'
-            + 'floats nor ints.')
+            "Some entries in lost_bits_transcription are neither"
+            + "floats nor ints.",
+        )
 
         # check values
         lost_bits_transcription_30 = [
-            6.659823518580827, 7.566530101329372, 7.989788581807347,
-            8.126275184924792, 8.156165618892503, 8.158803371775676,
-            8.1571939291375, 8.155956959505353, 8.155384990230832,
-            8.155170750799739, 8.155101341468276, 8.155081672171026,
-            8.155076924745707, 8.155076049611791, 8.15507599036841,
-            8.155076036096093, 8.155076066576788, 8.155076079192476,
-            8.155076083345309, 8.1550760844654, 8.155076084693125,
-            8.155076084711247, 8.155076084698281, 8.155076084688659,
-            8.15507608468425, 8.15507608468261, 8.155076084682092,
-            8.15507608468194, 8.155076084681896, 8.155076084681886
+            6.659823518580827,
+            7.566530101329372,
+            7.989788581807347,
+            8.126275184924792,
+            8.156165618892503,
+            8.158803371775676,
+            8.1571939291375,
+            8.155956959505353,
+            8.155384990230832,
+            8.155170750799739,
+            8.155101341468276,
+            8.155081672171026,
+            8.155076924745707,
+            8.155076049611791,
+            8.15507599036841,
+            8.155076036096093,
+            8.155076066576788,
+            8.155076079192476,
+            8.155076083345309,
+            8.1550760844654,
+            8.155076084693125,
+            8.155076084711247,
+            8.155076084698281,
+            8.155076084688659,
+            8.15507608468425,
+            8.15507608468261,
+            8.155076084682092,
+            8.15507608468194,
+            8.155076084681896,
+            8.155076084681886,
         ]
         for i, bits in enumerate(lost_bits):
-            self.assertAlmostEqual(bits,
-                                   lost_bits_transcription_30[min(i, 29)],
-                                   msg='lost_bits_transcription are incorrect.')
+            self.assertAlmostEqual(
+                bits,
+                lost_bits_transcription_30[min(i, 29)],
+                msg="lost_bits_transcription are incorrect.",
+            )
 
     @weight(4)
-    @timeout_decorator.timeout(1.)
+    @timeout_decorator.timeout(1.0)
     def test_J_star_N_riccati(self):
         """Test value function Riccati recursion"""
         # get list of costs to go
-        J_star_N = self.notebook_locals['J_star_N_riccati']
+        J_star_N = self.notebook_locals["J_star_N_riccati"]
 
         # check list length and types
         self.assertEqual(
-            len(J_star_N), 500,
-            'The list J_star_N_riccati must have length equal' + 'to 1000.')
+            len(J_star_N),
+            500,
+            "The list J_star_N_riccati must have length equal" + "to 1000.",
+        )
         J_star_type = [isinstance(J, (float, int)) for J in J_star_N]
         self.assertTrue(
             all(J_star_type),
-            'Some entries in J_star_N_riccati are neither floats' + 'nor ints.')
+            "Some entries in J_star_N_riccati are neither floats"
+            + "nor ints.",
+        )
 
         # check values
-        self._test_J_star(J_star_N, 'J_star_N_riccati is incorrect.')
+        self._test_J_star(J_star_N, "J_star_N_riccati is incorrect.")
 
     def _test_J_star(self, J_star_N, msg):
-
         # check values
         J_star_N_30 = [
-            10.75, 18.506849315068493, 24.221925133689837, 26.538390153365242,
-            27.14309163681062, 27.243582216689365, 27.242000076428884,
-            27.231499085690622, 27.225612316892573, 27.223217461345843,
-            27.222393413120585, 27.222143703386408, 27.222076887248043,
-            27.222061591713505, 27.22205892953035, 27.22205878066236,
-            27.222058926005232, 27.222059017397356, 27.22205905444766,
-            27.222059066651646, 27.222059070055877, 27.22205907083573,
-            27.222059070957876, 27.222059070953733, 27.22205907093976,
-            27.22205907093211, 27.22205907092905, 27.222059070928,
-            27.222059070927678, 27.222059070927585
+            10.75,
+            18.506849315068493,
+            24.221925133689837,
+            26.538390153365242,
+            27.14309163681062,
+            27.243582216689365,
+            27.242000076428884,
+            27.231499085690622,
+            27.225612316892573,
+            27.223217461345843,
+            27.222393413120585,
+            27.222143703386408,
+            27.222076887248043,
+            27.222061591713505,
+            27.22205892953035,
+            27.22205878066236,
+            27.222058926005232,
+            27.222059017397356,
+            27.22205905444766,
+            27.222059066651646,
+            27.222059070055877,
+            27.22205907083573,
+            27.222059070957876,
+            27.222059070953733,
+            27.22205907093976,
+            27.22205907093211,
+            27.22205907092905,
+            27.222059070928,
+            27.222059070927678,
+            27.222059070927585,
         ]
         for i, J in enumerate(J_star_N):
             self.assertAlmostEqual(J, J_star_N_30[min(i, 29)], msg=msg)
```

### Comparing `underactuated-2023.3.2/underactuated/jupyter.py` & `underactuated-2023.4.17/underactuated/jupyter.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,60 +1,64 @@
 import asyncio
 import os
 import sys
+from warnings import warn
 
 from IPython import get_ipython
-from IPython.display import display, HTML
+from IPython.display import HTML, display
 from ipywidgets.widgets import FloatSlider
-import numpy as np
-from warnings import warn
-
 from pydrake.systems.framework import VectorSystem
 
 # Use a global variable here because some calls to IPython will actually case an
 # interpreter to be created.  This file needs to be imported BEFORE that
 # happens.
-running_as_notebook = "COLAB_TESTING" not in os.environ and get_ipython(
-) and hasattr(get_ipython(), 'kernel')
+running_as_notebook = (
+    "COLAB_TESTING" not in os.environ
+    and get_ipython()
+    and hasattr(get_ipython(), "kernel")
+)
 
 
 def pyplot_is_interactive():
     # import needs to happen after the backend is set.
     import matplotlib.pyplot as plt
     from matplotlib.rcsetup import interactive_bk
+
     return plt.get_backend() in interactive_bk
 
 
-def AdvanceToAndVisualize(simulator,
-                          visualizer,
-                          time,
-                          time_if_running_headless=0.1,
-                          movie_filename=None):
+def AdvanceToAndVisualize(
+    simulator,
+    visualizer,
+    time,
+    time_if_running_headless=0.1,
+    movie_filename=None,
+):
     """
     Helper to support visualizing a simulation with pyplot visualizer.
     Will simply simulate (with target_realtime_rate = 1) if visualizer.show =
     True, or will record and render an animation if visualizer.show = False. If
     specified, time_if_running_headless will be used instead of time if
     running_as_notebook is False.
     """
     if visualizer._show:
         target_rate = simulator.get_target_realtime_rate()
-        simulator.set_target_realtime_rate(1.)
+        simulator.set_target_realtime_rate(1.0)
     else:
         print("simulating... ", end=" ")
         visualizer.start_recording()
     if time_if_running_headless and not running_as_notebook:
         time = time_if_running_headless
     simulator.AdvanceTo(time)
     if not visualizer._show or movie_filename:
         print("done.\ngenerating animation...")
         ani = visualizer.get_recording_as_animation()
         display(HTML(ani.to_jshtml()))
         if movie_filename:
-            with open(movie_filename, 'w') as f:
+            with open(movie_filename, "w") as f:
                 f.write(ani.to_jshtml())
     else:
         simulator.set_target_realtime_rate(target_rate)
 
 
 def SetupMatplotlibBackend(wishlist=["notebook"]):
     """
@@ -70,15 +74,15 @@
     # To find available backends, one can access the lists:
     # matplotlib.rcsetup.interactive_bk
     # matplotlib.rcsetup.non_interactive_bk
     # matplotlib.rcsetup.all_backends
     if running_as_notebook:
         ipython = get_ipython()
         # Short-circuit for google colab.
-        if 'google.colab' in sys.modules:
+        if "google.colab" in sys.modules:
             ipython.run_line_magic("matplotlib", "inline")
             return False
         # TODO: Find a way to detect vscode, and use inline instead of notebook
         for backend in wishlist:
             try:
                 ipython.run_line_magic("matplotlib", backend)
                 return pyplot_is_interactive()
@@ -111,24 +115,24 @@
 def update_widgets(num_ui_events_to_process=1):
     shell = get_ipython()
     # Ok to do nothing if running from console
     if shell is None:
         return
     kernel = shell.kernel
     events = []
-    kernel.shell_handlers['execute_request'] = lambda *e: events.append(e)
+    kernel.shell_handlers["execute_request"] = lambda *e: events.append(e)
     current_parent = (kernel._parent_ident, kernel._parent_header)
 
     for _ in range(num_ui_events_to_process):
         # ensure stdout still happens in the same cell
         kernel.set_parent(*current_parent)
         kernel.do_one_iteration()
         kernel.set_parent(*current_parent)
 
-    kernel.shell_handlers['execute_request'] = kernel.execute_request
+    kernel.shell_handlers["execute_request"] = kernel.execute_request
 
     def _replay_events(shell, events):
         kernel = shell.kernel
         sys.stdout.flush()
         sys.stderr.flush()
         for stream, ident, parent in events:
             kernel.set_parent(ident, parent)
@@ -137,30 +141,33 @@
             else:
                 kernel.execute_request(stream, ident, parent)
 
     loop = asyncio.get_event_loop()
     if loop.is_running():
         loop.call_soon(lambda: _replay_events(shell, events))
     else:
-        warn('Automatic execution of scheduled cells only works with '
-             'asyncio-based ipython')
+        warn(
+            "Automatic execution of scheduled cells only works with "
+            "asyncio-based ipython"
+        )
 
 
 # TODO(russt): generalize this to e.g. WidgetSystem (should work for any widget,
 # or list of widgets).
 class SliderSystem(VectorSystem):
-
     def __init__(self, min, max, value=0, description=""):
         # 0 inputs, 1 output.
         VectorSystem.__init__(self, 0, 1)
-        self.slider = FloatSlider(value=value,
-                                  description=description,
-                                  min=min,
-                                  max=max,
-                                  continuous_update=True)
+        self.slider = FloatSlider(
+            value=value,
+            description=description,
+            min=min,
+            max=max,
+            continuous_update=True,
+        )
 
         if get_ipython() is not None:
             display(self.slider)
 
     def DoCalcVectorOutput(self, context, unused, unused2, output):
         update_widgets()
         output[:] = self.slider.value
```

### Comparing `underactuated-2023.3.2/underactuated/meshcat_utils.py` & `underactuated-2023.4.17/underactuated/meshcat_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,24 @@
-from functools import partial
 import time
+from collections import namedtuple
+from functools import partial
+from inspect import Parameter, signature
 
 import numpy as np
-
-from pydrake.geometry import Cylinder, Rgba, Sphere
-from pydrake.perception import PointCloud, Fields, BaseField
-from pydrake.solvers import BoundingBoxConstraint
-
-# imports for interact
-from inspect import signature, Parameter
-from ipywidgets.widgets.interaction import (_get_min_max_value,
-                                            _yield_abbreviations_for_parameter)
-
-# imports for the pose sliders
-from collections import namedtuple
+from ipywidgets.widgets.interaction import (
+    _get_min_max_value,
+    _yield_abbreviations_for_parameter,
+)
 from pydrake.common.value import AbstractValue
-from pydrake.math import RollPitchYaw, RigidTransform, RotationMatrix
-from pydrake.systems.framework import LeafSystem, PublishEvent
-
-# imports for the joint sliders
+from pydrake.geometry import Cylinder, Rgba, Sphere
+from pydrake.math import RigidTransform, RollPitchYaw, RotationMatrix
 from pydrake.multibody.tree import JointIndex
-from pydrake.systems.framework import PublishEvent
+from pydrake.perception import BaseField, Fields, PointCloud
+from pydrake.solvers import BoundingBoxConstraint
+from pydrake.systems.framework import LeafSystem
 
 from underactuated import running_as_notebook
 
 # Some GUI code that will be moved into Drake.
 
 
 def interact(meshcat, callback, **kwargs):
@@ -45,38 +39,42 @@
             sig = signature(callback)
         except (ValueError, TypeError):
             # can't inspect, no info from function; only use kwargs
             return [(key, value, value) for key, value in kwargs.items()]
 
         for param in sig.parameters.values():
             for name, value, default in _yield_abbreviations_for_parameter(
-                    param, kwargs):
+                param, kwargs
+            ):
                 if value is Parameter.empty:
                     raise ValueError(
-                        'cannot find widget or abbreviation for argument: {!r}'.
-                        format(name))
+                        "cannot find widget or abbreviation for argument: {!r}".format(
+                            name
+                        )
+                    )
                 new_kwargs.append((name, value, default))
         return new_kwargs
 
     new_kwargs = find_abbreviations(callback, kwargs)
 
     for name, abbrev, default in new_kwargs:
         kw = {}
-        kw['value'] = None if default is Parameter.empty else default
+        kw["value"] = None if default is Parameter.empty else default
         if isinstance(abbrev, tuple):
-            kw['step'] = abbrev[2] if len(abbrev) != 3 else None
+            kw["step"] = abbrev[2] if len(abbrev) != 3 else None
             kw["min"], kw["max"], kw["value"] = _get_min_max_value(
-                abbrev[0], abbrev[1], **kw)
-            if kw['step'] is None:
-                kw['step'] = 0.1
+                abbrev[0], abbrev[1], **kw
+            )
+            if kw["step"] is None:
+                kw["step"] = 0.1
             meshcat.AddSlider(name, **kw)
         else:
             raise ValueError("This case is not implemented yet")
             # It might be simple.  I just haven't tried!
-        values[name] = kw['value']
+        values[name] = kw["value"]
 
     def update_values():
         changed = False
         for name in values:
             v = meshcat.GetSliderValue(name)
             changed |= v != values[name]
             values[name] = v
@@ -89,15 +87,15 @@
         return
 
     print("Press the 'Stop Interacting' button in Meshcat to continue.")
     meshcat.AddButton("Stop Interacting")
     while meshcat.GetButtonClicks("Stop Interacting") < 1:
         if update_values():
             callback(**values)
-        time.sleep(.1)
+        time.sleep(0.1)
 
     meshcat.DeleteButton("Stop Interacting")
     for name in values:
         meshcat.DeleteSlider(name)
 
 
 class MeshcatSliders(LeafSystem):
@@ -124,16 +122,18 @@
         """
         LeafSystem.__init__(self)
 
         self._meshcat = meshcat
         self._sliders = slider_names
         for i, slider_iterable in enumerate(self._sliders):
             port = self.DeclareVectorOutputPort(
-                f"slider_group_{i}", len(slider_iterable),
-                partial(self.DoCalcOutput, port_index=i))
+                f"slider_group_{i}",
+                len(slider_iterable),
+                partial(self.DoCalcOutput, port_index=i),
+            )
             port.disable_caching_by_default()
 
     def DoCalcOutput(self, context, output, port_index):
         for i, slider in enumerate(self._sliders[port_index]):
             output[i] = self._meshcat.GetSliderValue(slider)
 
 
@@ -145,66 +145,73 @@
 
     .. pydrake_system::
 
         name: PoseSliders
         output_ports:
         - pose
     """
+
     # TODO(russt): Use namedtuple defaults parameter once we are Python >= 3.7.
     Visible = namedtuple("Visible", ("roll", "pitch", "yaw", "x", "y", "z"))
     Visible.__new__.__defaults__ = (True, True, True, True, True, True)
     MinRange = namedtuple("MinRange", ("roll", "pitch", "yaw", "x", "y", "z"))
     MinRange.__new__.__defaults__ = (-np.pi, -np.pi, -np.pi, -1.0, -1.0, -1.0)
     MaxRange = namedtuple("MaxRange", ("roll", "pitch", "yaw", "x", "y", "z"))
     MaxRange.__new__.__defaults__ = (np.pi, np.pi, np.pi, 1.0, 1.0, 1.0)
     Value = namedtuple("Value", ("roll", "pitch", "yaw", "x", "y", "z"))
     Value.__new__.__defaults__ = (0.0, 0.0, 0.0, 0.0, 0.0, 0.0)
 
-    def __init__(self,
-                 meshcat,
-                 visible=Visible(),
-                 min_range=MinRange(),
-                 max_range=MaxRange(),
-                 value=Value()):
+    def __init__(
+        self,
+        meshcat,
+        visible=Visible(),
+        min_range=MinRange(),
+        max_range=MaxRange(),
+        value=Value(),
+    ):
         """
         Args:
             meshcat: A Meshcat instance.
             visible: An object with boolean elements for 'roll', 'pitch',
                      'yaw', 'x', 'y', 'z'; the intention is for this to be the
                      PoseSliders.Visible() namedtuple.  Defaults to all true.
             min_range, max_range, value: Objects with float values for 'roll',
                       'pitch', 'yaw', 'x', 'y', 'z'; the intention is for the
                       caller to use the PoseSliders.MinRange, MaxRange, and
                       Value namedtuples.  See those tuples for default values.
         """
         LeafSystem.__init__(self)
         port = self.DeclareAbstractOutputPort(
-            "pose", lambda: AbstractValue.Make(RigidTransform()),
-            self.DoCalcOutput)
+            "pose",
+            lambda: AbstractValue.Make(RigidTransform()),
+            self.DoCalcOutput,
+        )
 
         # The widgets themselves have undeclared state.  For now, we accept it,
         # and simply disable caching on the output port.
         # TODO(russt): consider implementing the more elaborate methods seen
         # in, e.g., LcmMessageSubscriber.
         port.disable_caching_by_default()
 
         self._meshcat = meshcat
         self._visible = visible
         self._value = list(value)
 
         for i in range(6):
             if visible[i]:
-                meshcat.AddSlider(min=min_range[i],
-                                  max=max_range[i],
-                                  value=value[i],
-                                  step=0.01,
-                                  name=value._fields[i])
+                meshcat.AddSlider(
+                    min=min_range[i],
+                    max=max_range[i],
+                    value=value[i],
+                    step=0.01,
+                    name=value._fields[i],
+                )
 
     def __del__(self):
-        for s in ['roll', 'pitch', 'yaw', 'x', 'y', 'z']:
+        for s in ["roll", "pitch", "yaw", "x", "y", "z"]:
             if visible[s]:
                 self._meshcat.DeleteSlider(s)
 
     def SetPose(self, pose):
         """
         Sets the current value of the sliders.
 
@@ -224,76 +231,81 @@
             rpy: An instance of drake.math.RollPitchYaw
         """
         self._value[0] = rpy.roll_angle()
         self._value[1] = rpy.pitch_angle()
         self._value[2] = rpy.yaw_angle()
         for i in range(3):
             if self._visible[i]:
-                self._meshcat.SetSliderValue(self._visible._fields[i],
-                                             self._value[i])
+                self._meshcat.SetSliderValue(
+                    self._visible._fields[i], self._value[i]
+                )
 
     def SetXyz(self, xyz):
         """
         Sets the current value of the sliders for x, y, and z.
 
         Args:
             xyz: A 3 element iterable object with x, y, z.
         """
         self._value[3:] = xyz
         for i in range(3, 6):
             if self._visible[i]:
-                self._meshcat.SetSliderValue(self._visible._fields[i],
-                                             self._value[i])
+                self._meshcat.SetSliderValue(
+                    self._visible._fields[i], self._value[i]
+                )
 
     def _update_values(self):
         changed = False
         for i in range(6):
             if self._visible[i]:
                 old_value = self._value[i]
                 self._value[i] = self._meshcat.GetSliderValue(
-                    self._visible._fields[i])
+                    self._visible._fields[i]
+                )
                 changed = changed or self._value[i] != old_value
         return changed
 
     def _get_transform(self):
         return RigidTransform(
             RollPitchYaw(self._value[0], self._value[1], self._value[2]),
-            self._value[3:])
+            self._value[3:],
+        )
 
     def DoCalcOutput(self, context, output):
         """Constructs the output values from the sliders."""
         self._update_values()
         output.set_value(self._get_transform())
 
     def Run(self, publishing_system, root_context, callback):
         # Calls callback(root_context, pose), then publishing_system.Publish()
         # each time the sliders change value.
         if not running_as_notebook:
             return
 
         publishing_context = publishing_system.GetMyContextFromRoot(
-            root_context)
+            root_context
+        )
 
         print("Press the 'Stop PoseSliders' button in Meshcat to continue.")
         self._meshcat.AddButton("Stop PoseSliders")
         while self._meshcat.GetButtonClicks("Stop PoseSliders") < 1:
             if self._update_values():
                 callback(root_context, self._get_transform())
                 publishing_system.Publish(publishing_context)
-            time.sleep(.1)
+            time.sleep(0.1)
 
         self._meshcat.DeleteButton("Stop PoseSliders")
 
 
 class WsgButton(LeafSystem):
-
     def __init__(self, meshcat):
         LeafSystem.__init__(self)
-        port = self.DeclareVectorOutputPort("wsg_position", 1,
-                                            self.DoCalcOutput)
+        port = self.DeclareVectorOutputPort(
+            "wsg_position", 1, self.DoCalcOutput
+        )
         port.disable_caching_by_default()
         self._meshcat = meshcat
         self._button = "Open/Close Gripper"
         meshcat.AddButton(self._button)
 
     def __del__(self):
         self._meshcat.DeleteButton(self._button)
@@ -321,21 +333,23 @@
 
     In addition to being used inside a Diagram that is being simulated with
     Simulator, this class also offers a `Run` method that runs its own simple
     event loop, querying the slider values and calling `Publish`.  It does not
     simulate any state dynamics.
     """
 
-    def __init__(self,
-                 meshcat,
-                 plant,
-                 root_context=None,
-                 lower_limit=-10.,
-                 upper_limit=10.,
-                 resolution=0.01):
+    def __init__(
+        self,
+        meshcat,
+        plant,
+        root_context=None,
+        lower_limit=-10.0,
+        upper_limit=10.0,
+        resolution=0.01,
+    ):
         """
         Creates an meshcat slider for each joint in the plant.
 
         Args:
             meshcat:      A Meshcat instance.
             plant:        A MultibodyPlant. publishing_system: The System whose
                           Publish method will be called.  Can be the entire
@@ -365,39 +379,45 @@
 
         lower_limit = _broadcast(lower_limit, plant.num_positions())
         upper_limit = _broadcast(upper_limit, plant.num_positions())
         resolution = _broadcast(resolution, plant.num_positions())
 
         self._meshcat = meshcat
         self._plant = plant
-        plant_context = plant.GetMyContextFromRoot(root_context) if \
-            root_context else plant.CreateDefaultContext()
+        plant_context = (
+            plant.GetMyContextFromRoot(root_context)
+            if root_context
+            else plant.CreateDefaultContext()
+        )
 
         self._sliders = {}
         self._positions = plant.GetPositions(plant_context)
         slider_num = 0
         for i in range(plant.num_joints()):
             joint = plant.get_joint(JointIndex(i))
             low = joint.position_lower_limits()
             upp = joint.position_upper_limits()
             for j in range(joint.num_positions()):
                 index = joint.position_start() + j
                 description = joint.name()
                 if joint.num_positions() > 1:
-                    description += '_' + joint.position_suffix(j)
-                meshcat.AddSlider(value=self._positions[index],
-                                  min=max(low[j], lower_limit[slider_num]),
-                                  max=min(upp[j], upper_limit[slider_num]),
-                                  step=resolution[slider_num],
-                                  name=description)
+                    description += "_" + joint.position_suffix(j)
+                meshcat.AddSlider(
+                    value=self._positions[index],
+                    min=max(low[j], lower_limit[slider_num]),
+                    max=min(upp[j], upper_limit[slider_num]),
+                    step=resolution[slider_num],
+                    name=description,
+                )
                 self._sliders[index] = description
                 slider_num += 1
 
-        port = self.DeclareVectorOutputPort("positions", plant.num_positions(),
-                                            self.DoCalcOutput)
+        port = self.DeclareVectorOutputPort(
+            "positions", plant.num_positions(), self.DoCalcOutput
+        )
         port.disable_caching_by_default()
 
     def DoCalcOutput(self, context, output):
         output.SetFromVector(self._positions)
         for i, s in self._sliders.items():
             output[i] = self._meshcat.GetSliderValue(s)
 
@@ -415,92 +435,98 @@
         if not running_as_notebook:
             return
         print("Press the 'Stop JointSliders' button in Meshcat to continue.")
         self._meshcat.AddButton("Stop JointSliders")
 
         plant_context = self._plant.GetMyContextFromRoot(root_context)
         publishing_context = publishing_system.GetMyContextFromRoot(
-            root_context)
+            root_context
+        )
 
         publishing_system.Publish(publishing_context)
         while self._meshcat.GetButtonClicks("Stop JointSliders") < 1:
             old_positions = self._plant.GetPositions(plant_context)
             positions = self._positions
             for i, s in self._sliders.items():
                 positions[i] = self._meshcat.GetSliderValue(s)
             if not np.array_equal(positions, old_positions):
                 self._plant.SetPositions(plant_context, positions)
                 if callback:
                     callback(plant_context)
                 publishing_system.Publish(publishing_context)
-            time.sleep(.1)
+            time.sleep(0.1)
 
         self._meshcat.DeleteButton("Stop JointSliders")
 
 
-def AddMeshcatTriad(meshcat,
-                    path,
-                    length=.25,
-                    radius=0.01,
-                    opacity=1.,
-                    X_PT=RigidTransform()):
+def AddMeshcatTriad(
+    meshcat, path, length=0.25, radius=0.01, opacity=1.0, X_PT=RigidTransform()
+):
     meshcat.SetTransform(path, X_PT)
     # x-axis
-    X_TG = RigidTransform(RotationMatrix.MakeYRotation(np.pi / 2),
-                          [length / 2., 0, 0])
+    X_TG = RigidTransform(
+        RotationMatrix.MakeYRotation(np.pi / 2), [length / 2.0, 0, 0]
+    )
     meshcat.SetTransform(path + "/x-axis", X_TG)
-    meshcat.SetObject(path + "/x-axis", Cylinder(radius, length),
-                      Rgba(1, 0, 0, opacity))
+    meshcat.SetObject(
+        path + "/x-axis", Cylinder(radius, length), Rgba(1, 0, 0, opacity)
+    )
 
     # y-axis
-    X_TG = RigidTransform(RotationMatrix.MakeXRotation(np.pi / 2),
-                          [0, length / 2., 0])
+    X_TG = RigidTransform(
+        RotationMatrix.MakeXRotation(np.pi / 2), [0, length / 2.0, 0]
+    )
     meshcat.SetTransform(path + "/y-axis", X_TG)
-    meshcat.SetObject(path + "/y-axis", Cylinder(radius, length),
-                      Rgba(0, 1, 0, opacity))
+    meshcat.SetObject(
+        path + "/y-axis", Cylinder(radius, length), Rgba(0, 1, 0, opacity)
+    )
 
     # z-axis
-    X_TG = RigidTransform([0, 0, length / 2.])
+    X_TG = RigidTransform([0, 0, length / 2.0])
     meshcat.SetTransform(path + "/z-axis", X_TG)
-    meshcat.SetObject(path + "/z-axis", Cylinder(radius, length),
-                      Rgba(0, 0, 1, opacity))
+    meshcat.SetObject(
+        path + "/z-axis", Cylinder(radius, length), Rgba(0, 0, 1, opacity)
+    )
 
 
-def draw_open3d_point_cloud(meshcat,
-                            path,
-                            pcd,
-                            normals_scale=0.0,
-                            point_size=0.001):
+def draw_open3d_point_cloud(
+    meshcat, path, pcd, normals_scale=0.0, point_size=0.001
+):
     pts = np.asarray(pcd.points)
-    assert (pcd.has_colors())  # TODO(russt): handle this case better
+    assert pcd.has_colors()  # TODO(russt): handle this case better
     cloud = PointCloud(pts.shape[0], Fields(BaseField.kXYZs | BaseField.kRGBs))
     cloud.mutable_xyzs()[:] = pts.T
     cloud.mutable_rgbs()[:] = 255 * np.asarray(pcd.colors).T
     meshcat.SetObject(path, cloud, point_size=point_size)
     if pcd.has_normals() and normals_scale > 0.0:
-        assert ('need to implement LineSegments in meshcat c++')
+        assert "need to implement LineSegments in meshcat c++"
         normals = np.asarray(pcd.normals)
-        vertices = np.hstack(
-            (pts, pts + normals_scale * normals)).reshape(-1, 3).T
+        vertices = (
+            np.hstack((pts, pts + normals_scale * normals)).reshape(-1, 3).T
+        )
         meshcat["normals"].set_object(
-            g.LineSegments(g.PointsGeometry(vertices),
-                           g.MeshBasicMaterial(color=0x000000)))
-
-
-def plot_surface(meshcat,
-                 path,
-                 X,
-                 Y,
-                 Z,
-                 rgba=Rgba(.87, .6, .6, 1.0),
-                 wireframe=False,
-                 wireframe_line_width=1.0):
+            g.LineSegments(
+                g.PointsGeometry(vertices), g.MeshBasicMaterial(color=0x000000)
+            )
+        )
+
+
+def plot_surface(
+    meshcat,
+    path,
+    X,
+    Y,
+    Z,
+    rgba=Rgba(0.87, 0.6, 0.6, 1.0),
+    wireframe=False,
+    wireframe_line_width=1.0,
+):
     (rows, cols) = Z.shape
-    assert (np.array_equal(X.shape, Y.shape))
-    assert (np.array_equal(X.shape, Z.shape))
+    assert np.array_equal(X.shape, Y.shape)
+    assert np.array_equal(X.shape, Z.shape)
 
     vertices = np.empty((rows * cols, 3), dtype=np.float32)
     vertices[:, 0] = X.reshape((-1))
     vertices[:, 1] = Y.reshape((-1))
     vertices[:, 2] = Z.reshape((-1))
 
     # Vectorized faces code from https://stackoverflow.com/questions/44934631/making-grid-triangular-mesh-quickly-with-numpy  # noqa
@@ -510,29 +536,26 @@
     faces[:, :, 1, 0] = r[:-1, 1:]
     faces[:, :, 0, 1] = r[:-1, 1:]
     faces[:, :, 1, 1] = r[1:, 1:]
     faces[:, :, :, 2] = r[1:, :-1, None]
     faces.shape = (-1, 3)
 
     # TODO(Russ): support per vertex / Colormap colors.
-    meshcat.SetTriangleMesh(path, vertices.T, faces.T, rgba, wireframe,
-                            wireframe_line_width)
+    meshcat.SetTriangleMesh(
+        path, vertices.T, faces.T, rgba, wireframe, wireframe_line_width
+    )
 
 
-def plot_mathematical_program(meshcat,
-                              path,
-                              prog,
-                              X,
-                              Y,
-                              result=None,
-                              point_size=0.05):
+def plot_mathematical_program(
+    meshcat, path, prog, X, Y, result=None, point_size=0.05
+):
     assert prog.num_vars() == 2
     assert X.size == Y.size
 
-    N = X.size
+    X.size
     values = np.vstack((X.reshape(-1), Y.reshape(-1)))
     costs = prog.GetAllCosts()
 
     # Vectorized multiply for the quadratic form.
     # Z = (D*np.matmul(Q,D)).sum(0).reshape(nx, ny)
 
     if costs:
@@ -545,58 +568,66 @@
         if isinstance(binding.evaluator(), BoundingBoxConstraint):
             c = binding.evaluator()
             var_indices = [
                 int(prog.decision_variable_index()[v.get_id()])
                 for v in binding.variables()
             ]
             satisfied = np.array(
-                c.CheckSatisfiedVectorized(values[var_indices, :],
-                                           0.001)).reshape(1, -1)
+                c.CheckSatisfiedVectorized(values[var_indices, :], 0.001)
+            ).reshape(1, -1)
             if costs:
                 Z[~satisfied] = np.nan
 
             v = f"{cv}/{type(c).__name__}"
             Zc = np.zeros(Z.shape)
             Zc[satisfied] = np.nan
-            plot_surface(meshcat,
-                         v,
-                         X,
-                         Y,
-                         Zc.reshape(X.shape),
-                         rgba=Rgba(1.0, .2, .2, 1.0),
-                         wireframe=True)
+            plot_surface(
+                meshcat,
+                v,
+                X,
+                Y,
+                Zc.reshape(X.shape),
+                rgba=Rgba(1.0, 0.2, 0.2, 1.0),
+                wireframe=True,
+            )
         else:
             Zc = prog.EvalBindingVectorized(binding, values)
             evaluator = binding.evaluator()
             low = evaluator.lower_bound()
             up = evaluator.upper_bound()
             cvb = f"{cv}/{type(evaluator).__name__}"
             for index in range(Zc.shape[0]):
                 # TODO(russt): Plot infeasible points in a different color.
-                infeasible = np.logical_or(Zc[index, :] < low[index],
-                                           Zc[index, :] > up[index])
-                plot_surface(meshcat,
-                             f"{cvb}/{index}",
-                             X,
-                             Y,
-                             Zc[index, :].reshape(X.shape),
-                             rgba=Rgba(1.0, .3, 1.0, 1.0),
-                             wireframe=True)
+                infeasible = np.logical_or(
+                    Zc[index, :] < low[index], Zc[index, :] > up[index]
+                )
+                plot_surface(
+                    meshcat,
+                    f"{cvb}/{index}",
+                    X,
+                    Y,
+                    Zc[index, :].reshape(X.shape),
+                    rgba=Rgba(1.0, 0.3, 1.0, 1.0),
+                    wireframe=True,
+                )
 
     if costs:
-        plot_surface(meshcat,
-                     f"{path}/objective",
-                     X,
-                     Y,
-                     Z.reshape(X.shape),
-                     rgba=Rgba(.3, 1.0, .3, 1.0),
-                     wireframe=True)
+        plot_surface(
+            meshcat,
+            f"{path}/objective",
+            X,
+            Y,
+            Z.reshape(X.shape),
+            rgba=Rgba(0.3, 1.0, 0.3, 1.0),
+            wireframe=True,
+        )
 
     if result:
         v = f"{path}/solution"
-        meshcat.SetObject(v, Sphere(point_size), Rgba(.3, 1.0, .3, 1.0))
+        meshcat.SetObject(v, Sphere(point_size), Rgba(0.3, 1.0, 0.3, 1.0))
         x_solution = result.get_x_val()
         meshcat.SetTransform(
             v,
             RigidTransform(
-                [x_solution[0], x_solution[1],
-                 result.get_optimal_cost()]))
+                [x_solution[0], x_solution[1], result.get_optimal_cost()]
+            ),
+        )
```

### Comparing `underactuated-2023.3.2/underactuated/models/cartpole.urdf` & `underactuated-2023.4.17/underactuated/models/cartpole.urdf`

 * *Files identical despite different names*

### Comparing `underactuated-2023.3.2/underactuated/models/compass_gait_limit_cycle.urdf` & `underactuated-2023.4.17/underactuated/models/compass_gait_limit_cycle.urdf`

 * *Files identical despite different names*

### Comparing `underactuated-2023.3.2/underactuated/models/double_pendulum.sdf` & `underactuated-2023.4.17/underactuated/models/double_pendulum.sdf`

 * *Files identical despite different names*

### Comparing `underactuated-2023.3.2/underactuated/models/double_pendulum.urdf` & `underactuated-2023.4.17/underactuated/models/double_pendulum.urdf`

 * *Files identical despite different names*

### Comparing `underactuated-2023.3.2/underactuated/models/glider/glider.urdf` & `underactuated-2023.4.17/underactuated/models/glider/glider.urdf`

 * *Files 14% similar despite different names*

#### Comparing `underactuated-2023.3.2/underactuated/models/glider/glider.urdf` & `underactuated-2023.4.17/underactuated/models/glider/glider.urdf`

```diff
@@ -9,136 +9,136 @@
       <origin xyz="-0.0818128241934648 -1.22124532708767E-15 -0.00908986598442222" rpy="0 0 0"/>
       <mass value="0.00370301987946561"/>
       <inertia ixx="2.07978185361861E-06" ixy="-6.51921720268355E-22" ixz="4.10535888298005E-07" iyy="6.8353862114488E-05" iyz="3.50540764772016E-22" izz="6.62780619947118E-05"/>
     </inertial>
     <visual>
       <origin xyz="0 0 0" rpy="0 0 0"/>
       <geometry>
-        <mesh filename="meshes/fuselagev_main.obj"/>
+        <mesh filename="package://underactuated/models/glider/meshes/fuselagev_main.obj"/>
       </geometry>
       <material name="">
         <color rgba=".7 .7 .7 1"/>
       </material>
     </visual>
     <collision>
       <origin xyz="0 0 0" rpy="0 0 0"/>
       <geometry>
-        <mesh filename="meshes/fuselagev_main.obj"/>
+        <mesh filename="package://underactuated/models/glider/meshes/fuselagev_main.obj"/>
       </geometry>
     </collision>
     <visual>
       <origin xyz="0 0 0" rpy="0 0 0"/>
       <geometry>
-        <mesh filename="meshes/fuselagev_top.obj"/>
+        <mesh filename="package://underactuated/models/glider/meshes/fuselagev_top.obj"/>
       </geometry>
       <material name="">
         <color rgba=".7 .7 .7 1"/>
       </material>
     </visual>
     <collision>
       <origin xyz="0 0 0" rpy="0 0 0"/>
       <geometry>
-        <mesh filename="meshes/fuselagev_top.obj"/>
+        <mesh filename="package://underactuated/models/glider/meshes/fuselagev_top.obj"/>
       </geometry>
     </collision>
     <visual>
       <origin xyz="0 0 0" rpy="0 0 0"/>
       <geometry>
-        <mesh filename="meshes/fuselagev_vstab.obj"/>
+        <mesh filename="package://underactuated/models/glider/meshes/fuselagev_vstab.obj"/>
       </geometry>
       <material name="">
         <color rgba=".7 .7 .7 1"/>
       </material>
     </visual>
     <collision>
       <origin xyz="0 0 0" rpy="0 0 0"/>
       <geometry>
-        <mesh filename="meshes/fuselagev_vstab.obj"/>
+        <mesh filename="package://underactuated/models/glider/meshes/fuselagev_vstab.obj"/>
       </geometry>
     </collision>
     <visual>
       <origin xyz="0 0 0" rpy="0 0 0"/>
       <geometry>
-        <mesh filename="meshes/fuselageh_main.obj"/>
+        <mesh filename="package://underactuated/models/glider/meshes/fuselageh_main.obj"/>
       </geometry>
       <material name="">
         <color rgba=".7 .7 .7 1"/>
       </material>
     </visual>
     <collision>
       <origin xyz="0 0 0" rpy="0 0 0"/>
       <geometry>
-        <mesh filename="meshes/fuselageh_main.obj"/>
+        <mesh filename="package://underactuated/models/glider/meshes/fuselageh_main.obj"/>
       </geometry>
     </collision>
     <visual>
       <origin xyz="0 0 0" rpy="0 0 0"/>
       <geometry>
-        <mesh filename="meshes/fuselageh_hstab.obj"/>
+        <mesh filename="package://underactuated/models/glider/meshes/fuselageh_hstab.obj"/>
       </geometry>
       <material name="">
         <color rgba=".7 .7 .7 1"/>
       </material>
     </visual>
     <collision>
       <origin xyz="0 0 0" rpy="0 0 0"/>
       <geometry>
-        <mesh filename="meshes/fuselageh_hstab.obj"/>
+        <mesh filename="package://underactuated/models/glider/meshes/fuselageh_hstab.obj"/>
       </geometry>
     </collision>
     <visual>
       <origin xyz="0 0 0" rpy="0 0 0"/>
       <geometry>
-        <mesh filename="meshes/wing_left.obj"/>
+        <mesh filename="package://underactuated/models/glider/meshes/wing_left.obj"/>
       </geometry>
       <material name="">
         <color rgba="0 .34 .9 1"/>
       </material>
     </visual>
     <collision>
       <origin xyz="0 0 0" rpy="0 0 0"/>
       <geometry>
-        <mesh filename="meshes/wing_left.obj"/>
+        <mesh filename="package://underactuated/models/glider/meshes/wing_left.obj"/>
       </geometry>
     </collision>
     <visual>
       <origin xyz="0 0 0" rpy="0 0 0"/>
       <geometry>
-        <mesh filename="meshes/wing_right.obj"/>
+        <mesh filename="package://underactuated/models/glider/meshes/wing_right.obj"/>
       </geometry>
       <material name="">
         <color rgba="0 .34 .9 1"/>
       </material>
     </visual>
     <collision>
       <origin xyz="0 0 0" rpy="0 0 0"/>
       <geometry>
-        <mesh filename="meshes/wing_right.obj"/>
+        <mesh filename="package://underactuated/models/glider/meshes/wing_right.obj"/>
       </geometry>
     </collision>
   </link>
   <link name="elevator">
     <inertial>
       <origin xyz="-0.0233269083291484 5.1589050238332E-05 -2.16840434497101E-19" rpy="0 0 0"/>
       <mass value="0.00149262442134654"/>
       <inertia ixx="7.52285851301533E-06" ixy="-1.45222492008535E-12" ixz="1.75768911831126E-23" iyy="6.94987923385513E-07" iyz="-1.92169321155844E-23" izz="8.21624146684023E-06"/>
     </inertial>
     <visual>
       <origin xyz="0 0 0" rpy="0 0 0"/>
       <geometry>
-        <mesh filename="meshes/elevator.obj"/>
+        <mesh filename="package://underactuated/models/glider/meshes/elevator.obj"/>
       </geometry>
       <material name="">
         <color rgba="0 .34 .9 1"/>
       </material>
     </visual>
     <collision>
       <origin xyz="0 0 0" rpy="0 0 0"/>
       <geometry>
-        <mesh filename="meshes/elevator.obj"/>
+        <mesh filename="package://underactuated/models/glider/meshes/elevator.obj"/>
       </geometry>
     </collision>
   </link>
   <joint name="elevator_hinge" type="revolute">
     <origin xyz="-0.317 0 0" rpy="0 0 0"/>
     <parent link="fuselage"/>
     <child link="elevator"/>
```

### Comparing `underactuated-2023.3.2/underactuated/models/glider/meshes/elevator.obj` & `underactuated-2023.4.17/underactuated/models/glider/meshes/elevator.obj`

 * *Files identical despite different names*

### Comparing `underactuated-2023.3.2/underactuated/models/glider/meshes/fuselageh_hstab.obj` & `underactuated-2023.4.17/underactuated/models/glider/meshes/fuselageh_hstab.obj`

 * *Files identical despite different names*

### Comparing `underactuated-2023.3.2/underactuated/models/glider/meshes/fuselageh_main.obj` & `underactuated-2023.4.17/underactuated/models/glider/meshes/fuselageh_main.obj`

 * *Files identical despite different names*

### Comparing `underactuated-2023.3.2/underactuated/models/glider/meshes/fuselagev_main.obj` & `underactuated-2023.4.17/underactuated/models/glider/meshes/fuselagev_main.obj`

 * *Files identical despite different names*

### Comparing `underactuated-2023.3.2/underactuated/models/glider/meshes/fuselagev_top.obj` & `underactuated-2023.4.17/underactuated/models/glider/meshes/fuselagev_top.obj`

 * *Files identical despite different names*

### Comparing `underactuated-2023.3.2/underactuated/models/glider/meshes/fuselagev_vstab.obj` & `underactuated-2023.4.17/underactuated/models/glider/meshes/fuselagev_vstab.obj`

 * *Files identical despite different names*

### Comparing `underactuated-2023.3.2/underactuated/models/glider/meshes/wing_left.obj` & `underactuated-2023.4.17/underactuated/models/glider/meshes/wing_left.obj`

 * *Files identical despite different names*

### Comparing `underactuated-2023.3.2/underactuated/models/glider/meshes/wing_right.obj` & `underactuated-2023.4.17/underactuated/models/glider/meshes/wing_right.obj`

 * *Files identical despite different names*

### Comparing `underactuated-2023.3.2/underactuated/models/littledog/LICENSE.txt` & `underactuated-2023.4.17/underactuated/models/littledog/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `underactuated-2023.3.2/underactuated/models/littledog/LittleDog.urdf` & `underactuated-2023.4.17/underactuated/models/littledog/LittleDog.urdf`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
   <link name="body">
     <inertial>
       <mass value="1.800000" />
       <inertia ixx="0.001625" ixy="0" ixz="0" iyy="0.009178" iyz="0" izz="0.008794" />
     </inertial>
     <visual>
       <geometry>
-        <mesh filename="meshes/body.obj" scale=".0254 .0254 .0254" />
+        <mesh filename="package://underactuated/models/littledog/meshes/body.obj" scale=".0254 .0254 .0254" />
       </geometry>
       <material name="black">
       	<color rgba="0.1 0.1 0.1 1" />
       </material>
     </visual>
   </link>
 
@@ -25,15 +25,15 @@
       <mass value="0.062300" />
       <inertia ixx="0.000004" ixy="0" ixz="0" iyy="0.000015" iyz="0" izz="0.000015" />
     </inertial>
 <!--
     <visual>
       <origin xyz="0 0 0" rpy="0 0 0" />
       <geometry>
-        <mesh filename="meshes/front_left_hip.obj" scale=".0254 .0254 .0254"/>
+        <mesh filename="package://underactuated/models/littledog/meshes/front_left_hip.obj" scale=".0254 .0254 .0254"/>
       </geometry>
       <material name="black" />
     </visual>
 -->
   </link>
 
   <joint name="front_left_hip_roll" type="revolute">
@@ -54,15 +54,15 @@
       <origin xyz="0.000000 0.000000 -0.016600" rpy="0 0 0" />
       <mass value="0.127900" />
       <inertia ixx="0.000082" ixy="0" ixz="0" iyy="0.000089" iyz="0" izz="0.000015" />
     </inertial>
     <visual>
       <origin xyz="0 0 0" rpy="0 0 0" />
       <geometry>
-        <mesh filename="meshes/front_left_upper.obj" scale=".0254 .0254 .0254"/>
+        <mesh filename="package://underactuated/models/littledog/meshes/front_left_upper.obj" scale=".0254 .0254 .0254"/>
       </geometry>
       <material name="black" />
     </visual>
   </link>
   
   <joint name="front_left_hip_pitch" type="revolute">
     <parent link="front_left_hip" />
@@ -82,15 +82,15 @@
       <origin xyz="0.000000 0.000000 -0.020200" rpy="0 0 0" />
       <mass value="0.046400" />
       <inertia ixx="0.000038" ixy="0" ixz="0" iyy="0.000035" iyz="0" izz="0.000004" />
     </inertial>
     <visual>
       <origin xyz="0 0 0" rpy="0 0 0" />
       <geometry>
-        <mesh filename="meshes/front_left_lower.obj" scale="0.0254 0.0254 0.0254"/>
+        <mesh filename="package://underactuated/models/littledog/meshes/front_left_lower.obj" scale="0.0254 0.0254 0.0254"/>
       </geometry>
       <material name="black" />
     </visual>
     <collision>
       <origin xyz="-0.0265 0 -0.048" /> <!-- note this is approximate -->
       <geometry>
         <capsule radius="0.012" length="0.09" />
@@ -125,15 +125,15 @@
       <mass value="0.062300" />
       <inertia ixx="0.000004" ixy="0" ixz="0" iyy="0.000015" iyz="0" izz="0.000015" />
     </inertial>
 <!--
     <visual>
       <origin xyz="0 0 0" rpy="0 0 0" />
       <geometry>
-        <mesh filename="meshes/front_right_hip.obj" scale="0.0254 0.0254 0.0254"/>
+        <mesh filename="package://underactuated/models/littledog/meshes/front_right_hip.obj" scale="0.0254 0.0254 0.0254"/>
       </geometry>
       <material name="black" />
     </visual>
  -->
    </link>
 
   <joint name="front_right_hip_roll" type="revolute">
@@ -154,15 +154,15 @@
       <origin xyz="0.000000 0.000000 -0.016600" rpy="0 0 0" />
       <mass value="0.127900" />
       <inertia ixx="0.000082" ixy="0" ixz="0" iyy="0.000089" iyz="0" izz="0.000015" />
     </inertial>
     <visual>
       <origin xyz="0 0 0" rpy="0 0 0" />
       <geometry>
-        <mesh filename="meshes/front_right_upper.obj" scale="0.0254 0.0254 0.0254"/>
+        <mesh filename="package://underactuated/models/littledog/meshes/front_right_upper.obj" scale="0.0254 0.0254 0.0254"/>
       </geometry>
       <material name="black"/>
     </visual>
   </link>
 
   <joint name="front_right_hip_pitch" type="revolute">
     <parent link="front_right_hip" />
@@ -182,15 +182,15 @@
       <origin xyz="0.000000 0.000000 -0.020200" rpy="0 0 0" />
       <mass value="0.046400" />
       <inertia ixx="0.000038" ixy="0" ixz="0" iyy="0.000035" iyz="0" izz="0.000004" />
     </inertial>
     <visual>
       <origin xyz="0 0 0" rpy="0 0 0" />
       <geometry>
-        <mesh filename="meshes/front_right_lower.obj" scale="0.0254 0.0254 0.0254"/>
+        <mesh filename="package://underactuated/models/littledog/meshes/front_right_lower.obj" scale="0.0254 0.0254 0.0254"/>
       </geometry>
       <material name="black"/>
     </visual>
     <collision>
       <origin xyz="-0.0265 0 -0.048" /> <!-- note this is approximate -->
       <geometry>
         <capsule radius="0.012" length="0.09" />
@@ -224,15 +224,15 @@
       <origin xyz="0.000000 0.002900 0.000000" rpy="0 0 0" />
       <mass value="0.062300" />
       <inertia ixx="0.000004" ixy="0" ixz="0" iyy="0.000015" iyz="0" izz="0.000015" />
     </inertial>
 <!--    <visual>
       <origin xyz="0 0 0" rpy="0 0 0" />
       <geometry>
-        <mesh filename="meshes/back_left_hip.obj" scale="0.0254 0.0254 0.0254"/>
+        <mesh filename="package://underactuated/models/littledog/meshes/back_left_hip.obj" scale="0.0254 0.0254 0.0254"/>
       </geometry>
       <material name="black" />
     </visual>
 -->
   </link>
 
   <joint name="back_left_hip_roll" type="revolute">
@@ -253,15 +253,15 @@
       <origin xyz="0.000000 0.000000 -0.016600" rpy="0 0 0" />
       <mass value="0.127900" />
       <inertia ixx="0.000082" ixy="0" ixz="0" iyy="0.000089" iyz="0" izz="0.000015" />
     </inertial>
     <visual>
       <origin xyz="0 0 0" rpy="0 0 0" />
       <geometry>
-        <mesh filename="meshes/back_left_upper.obj" scale="0.0254 0.0254 0.0254"/>
+        <mesh filename="package://underactuated/models/littledog/meshes/back_left_upper.obj" scale="0.0254 0.0254 0.0254"/>
       </geometry>
       <material name="black" />
     </visual>
   </link>
 
   <joint name="back_left_hip_pitch" type="revolute">
     <parent link="back_left_hip" />
@@ -281,15 +281,15 @@
       <origin xyz="0.000000 0.000000 -0.020200" rpy="0 0 0" />
       <mass value="0.046400" />
       <inertia ixx="0.000038" ixy="0" ixz="0" iyy="0.000035" iyz="0" izz="0.000004" />
     </inertial>
     <visual>
       <origin xyz="0 0 0" rpy="0 0 0" />
       <geometry>
-        <mesh filename="meshes/back_left_lower.obj" scale="0.0254 0.0254 0.0254"/>
+        <mesh filename="package://underactuated/models/littledog/meshes/back_left_lower.obj" scale="0.0254 0.0254 0.0254"/>
       </geometry>
       <material name="black" />
     </visual>
     <collision>
       <origin xyz="0.0265 0 -0.048" /> <!-- note this is approximate -->
       <geometry>
         <capsule radius="0.012" length="0.09" />
@@ -323,15 +323,15 @@
       <origin xyz="0.000000 -0.002900 0.000000" rpy="0 0 0" />
       <mass value="0.062300" />
       <inertia ixx="0.000004" ixy="0" ixz="0" iyy="0.000015" iyz="0" izz="0.000015" />
     </inertial>
 <!--    <visual>
       <origin xyz="0 0 0" rpy="0 0 0" />
       <geometry>
-        <mesh filename="meshes/back_right_hip.obj" scale="0.0254 0.0254 0.0254"/>
+        <mesh filename="package://underactuated/models/littledog/meshes/back_right_hip.obj" scale="0.0254 0.0254 0.0254"/>
       </geometry>
       <material name="black" />
     </visual>
 -->
   </link>
 
   <joint name="back_right_hip_roll" type="revolute">
@@ -352,15 +352,15 @@
       <origin xyz="0.000000 0.000000 -0.016600" rpy="0 0 0" />
       <mass value="0.127900" />
       <inertia ixx="0.000082" ixy="0" ixz="0" iyy="0.000089" iyz="0" izz="0.000015" />
     </inertial>
     <visual>
       <origin xyz="0 0 0" rpy="0 0 0" />
       <geometry>
-        <mesh filename="meshes/back_right_upper.obj" scale="0.0254 0.0254 0.0254"/>
+        <mesh filename="package://underactuated/models/littledog/meshes/back_right_upper.obj" scale="0.0254 0.0254 0.0254"/>
       </geometry>
       <material name="black" />
     </visual>
   </link>
 
   <joint name="back_right_hip_pitch" type="revolute">
     <parent link="back_right_hip" />
@@ -380,15 +380,15 @@
       <origin xyz="0.000000 0.000000 -0.020200" rpy="0 0 0" />
       <mass value="0.046400" />
       <inertia ixx="0.000038" ixy="0" ixz="0" iyy="0.000035" iyz="0" izz="0.000004" />
     </inertial>
     <visual>
       <origin xyz="0 0 0" rpy="0 0 0" />
       <geometry>
-        <mesh filename="meshes/back_right_lower.obj" scale="0.0254 0.0254 0.0254"/>
+        <mesh filename="package://underactuated/models/littledog/meshes/back_right_lower.obj" scale="0.0254 0.0254 0.0254"/>
       </geometry>
       <material name="black" />
     </visual>
     <collision>
       <origin xyz="0.0265 0 -0.048" /> <!-- note this is approximate -->
       <geometry>
         <capsule radius="0.012" length="0.09" />
```

### Comparing `underactuated-2023.3.2/underactuated/models/littledog/ground.urdf` & `underactuated-2023.4.17/underactuated/models/littledog/ground.urdf`

 * *Files identical despite different names*

### Comparing `underactuated-2023.3.2/underactuated/models/littledog/meshes/back_left_hip.obj` & `underactuated-2023.4.17/underactuated/models/littledog/meshes/back_left_hip.obj`

 * *Files identical despite different names*

### Comparing `underactuated-2023.3.2/underactuated/models/littledog/meshes/back_left_lower.obj` & `underactuated-2023.4.17/underactuated/models/littledog/meshes/back_left_lower.obj`

 * *Files identical despite different names*

### Comparing `underactuated-2023.3.2/underactuated/models/littledog/meshes/back_left_lower.obj.mtl` & `underactuated-2023.4.17/underactuated/models/littledog/meshes/back_left_lower.obj.mtl`

 * *Files identical despite different names*

### Comparing `underactuated-2023.3.2/underactuated/models/littledog/meshes/back_left_upper.obj` & `underactuated-2023.4.17/underactuated/models/littledog/meshes/back_left_upper.obj`

 * *Files identical despite different names*

### Comparing `underactuated-2023.3.2/underactuated/models/littledog/meshes/back_left_upper.obj.mtl` & `underactuated-2023.4.17/underactuated/models/littledog/meshes/back_left_upper.obj.mtl`

 * *Files identical despite different names*

### Comparing `underactuated-2023.3.2/underactuated/models/littledog/meshes/back_right_hip.obj` & `underactuated-2023.4.17/underactuated/models/littledog/meshes/back_right_hip.obj`

 * *Files identical despite different names*

### Comparing `underactuated-2023.3.2/underactuated/models/littledog/meshes/back_right_lower.obj` & `underactuated-2023.4.17/underactuated/models/littledog/meshes/back_right_lower.obj`

 * *Files identical despite different names*

### Comparing `underactuated-2023.3.2/underactuated/models/littledog/meshes/back_right_lower.obj.mtl` & `underactuated-2023.4.17/underactuated/models/littledog/meshes/back_right_lower.obj.mtl`

 * *Files identical despite different names*

### Comparing `underactuated-2023.3.2/underactuated/models/littledog/meshes/back_right_upper.obj` & `underactuated-2023.4.17/underactuated/models/littledog/meshes/back_right_upper.obj`

 * *Files identical despite different names*

### Comparing `underactuated-2023.3.2/underactuated/models/littledog/meshes/back_right_upper.obj.mtl` & `underactuated-2023.4.17/underactuated/models/littledog/meshes/back_right_upper.obj.mtl`

 * *Files identical despite different names*

### Comparing `underactuated-2023.3.2/underactuated/models/littledog/meshes/body.obj` & `underactuated-2023.4.17/underactuated/models/littledog/meshes/body.obj`

 * *Files identical despite different names*

### Comparing `underactuated-2023.3.2/underactuated/models/littledog/meshes/body2.jpg` & `underactuated-2023.4.17/underactuated/models/littledog/meshes/body2.jpg`

 * *Files identical despite different names*

### Comparing `underactuated-2023.3.2/underactuated/models/littledog/meshes/body3.jpg` & `underactuated-2023.4.17/underactuated/models/littledog/meshes/body3.jpg`

 * *Files identical despite different names*

### Comparing `underactuated-2023.3.2/underactuated/models/littledog/meshes/foot.jpg` & `underactuated-2023.4.17/underactuated/models/littledog/meshes/foot.jpg`

 * *Files identical despite different names*

### Comparing `underactuated-2023.3.2/underactuated/models/littledog/meshes/front_left_hip.obj` & `underactuated-2023.4.17/underactuated/models/littledog/meshes/front_left_hip.obj`

 * *Files identical despite different names*

### Comparing `underactuated-2023.3.2/underactuated/models/littledog/meshes/front_left_lower.obj` & `underactuated-2023.4.17/underactuated/models/littledog/meshes/front_left_lower.obj`

 * *Files identical despite different names*

### Comparing `underactuated-2023.3.2/underactuated/models/littledog/meshes/front_left_lower.obj.mtl` & `underactuated-2023.4.17/underactuated/models/littledog/meshes/front_left_lower.obj.mtl`

 * *Files identical despite different names*

### Comparing `underactuated-2023.3.2/underactuated/models/littledog/meshes/front_left_upper.obj` & `underactuated-2023.4.17/underactuated/models/littledog/meshes/front_left_upper.obj`

 * *Files identical despite different names*

### Comparing `underactuated-2023.3.2/underactuated/models/littledog/meshes/front_left_upper.obj.mtl` & `underactuated-2023.4.17/underactuated/models/littledog/meshes/front_left_upper.obj.mtl`

 * *Files identical despite different names*

### Comparing `underactuated-2023.3.2/underactuated/models/littledog/meshes/front_right_hip.obj` & `underactuated-2023.4.17/underactuated/models/littledog/meshes/front_right_hip.obj`

 * *Files identical despite different names*

### Comparing `underactuated-2023.3.2/underactuated/models/littledog/meshes/front_right_lower.obj` & `underactuated-2023.4.17/underactuated/models/littledog/meshes/front_right_lower.obj`

 * *Files identical despite different names*

### Comparing `underactuated-2023.3.2/underactuated/models/littledog/meshes/front_right_lower.obj.mtl` & `underactuated-2023.4.17/underactuated/models/littledog/meshes/front_right_lower.obj.mtl`

 * *Files identical despite different names*

### Comparing `underactuated-2023.3.2/underactuated/models/littledog/meshes/front_right_upper.obj` & `underactuated-2023.4.17/underactuated/models/littledog/meshes/front_right_upper.obj`

 * *Files identical despite different names*

### Comparing `underactuated-2023.3.2/underactuated/models/littledog/meshes/front_right_upper.obj.mtl` & `underactuated-2023.4.17/underactuated/models/littledog/meshes/front_right_upper.obj.mtl`

 * *Files identical despite different names*

### Comparing `underactuated-2023.3.2/underactuated/models/littledog/meshes/leg.jpg` & `underactuated-2023.4.17/underactuated/models/littledog/meshes/leg.jpg`

 * *Files identical despite different names*

### Comparing `underactuated-2023.3.2/underactuated/models/one_d_hopper.urdf` & `underactuated-2023.4.17/underactuated/models/one_d_hopper.urdf`

 * *Files identical despite different names*

### Comparing `underactuated-2023.3.2/underactuated/models/undamped_cartpole.urdf` & `underactuated-2023.4.17/underactuated/models/undamped_cartpole.urdf`

 * *Files identical despite different names*

### Comparing `underactuated-2023.3.2/underactuated/models/vibrating_pendulum.urdf` & `underactuated-2023.4.17/underactuated/models/vibrating_pendulum.urdf`

 * *Files identical despite different names*

### Comparing `underactuated-2023.3.2/underactuated/multibody.py` & `underactuated-2023.4.17/underactuated/multibody.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,8 @@
-from pydrake.autodiffutils import AutoDiffXd
 from pydrake.multibody.tree import MultibodyForces_
-from pydrake.multibody.plant import MultibodyPlant_
-from pydrake.symbolic import Expression
-import numpy as np
 
 
 def ManipulatorDynamics(plant, q, v=None, context=None):
     if context is None:
         context = plant.CreateDefaultContext()
     plant.SetPositions(context, q)
     if v is not None:
```

### Comparing `underactuated-2023.3.2/underactuated/optimizers.py` & `underactuated-2023.4.17/underactuated/optimizers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 import numpy as np
 
 
-class Adam():
-
-    def __init__(self,
-                 params,
-                 lr=1e-3,
-                 betas=(0.9, 0.999),
-                 eps=1e-8,
-                 weight_decay=0,
-                 amsgrad=False):
+class Adam:
+    def __init__(
+        self,
+        params,
+        lr=1e-3,
+        betas=(0.9, 0.999),
+        eps=1e-8,
+        weight_decay=0,
+        amsgrad=False,
+    ):
         self.params = params
         if not 0.0 <= lr:
             raise ValueError("Invalid learning rate: {}".format(lr))
         self.lr = lr
         if not 0.0 <= eps:
             raise ValueError("Invalid epsilon value: {}".format(eps))
         self.eps = eps
         if not 0.0 <= betas[0] < 1.0:
-            raise ValueError("Invalid beta parameter at index 0: {}".format(
-                betas[0]))
+            raise ValueError(
+                "Invalid beta parameter at index 0: {}".format(betas[0])
+            )
         if not 0.0 <= betas[1] < 1.0:
-            raise ValueError("Invalid beta parameter at index 1: {}".format(
-                betas[1]))
+            raise ValueError(
+                "Invalid beta parameter at index 1: {}".format(betas[1])
+            )
         self.beta1 = betas[0]
         self.beta2 = betas[1]
         if not 0.0 <= weight_decay:
             raise ValueError(
-                "Invalid weight_decay value: {}".format(weight_decay))
+                "Invalid weight_decay value: {}".format(weight_decay)
+            )
         self.weight_decay = weight_decay
         self.amsgrad = amsgrad
 
         self.exp_avgs = 0 * params
         self.exp_avgs_sqs = 0 * params
         self.max_exp_avgs_sqs = 0 * params
         self.num_steps = 0
@@ -49,18 +53,20 @@
         self.exp_avgs += (1 - self.beta1) * dloss_dparams
 
         self.exp_avgs_sqs *= self.beta2
         self.exp_avgs_sqs += (1 - self.beta2) * (dloss_dparams**2)
 
         if self.amsgrad:
             # Maintains the maximum of all 2nd moment running avg. till now
-            np.maximumtorch.maximum(self.max_exp_avg_sqs,
-                                    exp_avgs_sqs,
-                                    out=self.max_exp_avgs_sqs)
+            np.maximumtorch.maximum(
+                self.max_exp_avg_sqs, exp_avgs_sqs, out=self.max_exp_avgs_sqs
+            )
             # Use the max. for normalizing running avg. of gradient
-            denom = (np.sqrt(self.max_exp_avgs_sqs)
-                     / np.sqrt(bias_correction2)) + self.eps
+            denom = (
+                np.sqrt(self.max_exp_avgs_sqs) / np.sqrt(bias_correction2)
+            ) + self.eps
         else:
-            denom = (np.sqrt(self.exp_avgs_sqs)
-                     / np.sqrt(bias_correction2)) + self.eps
+            denom = (
+                np.sqrt(self.exp_avgs_sqs) / np.sqrt(bias_correction2)
+            ) + self.eps
         step_size = self.lr / bias_correction1
         self.params -= step_size * self.exp_avgs / denom
```

### Comparing `underactuated-2023.3.2/underactuated/pendulum.py` & `underactuated-2023.4.17/underactuated/pendulum.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,58 +1,68 @@
 import numpy as np
-import math
-import matplotlib.animation as animation
 from pydrake.systems.framework import Context, PortDataType
 from pydrake.systems.pyplot_visualizer import PyPlotVisualizer
 
 
 class PendulumVisualizer(PyPlotVisualizer):
     a1 = 0.75
     ac1 = 0.75
-    av = np.linspace(0, math.pi, 20)
-    rb = .03
-    hb = .07
-    aw = .01
+    av = np.linspace(0, np.pi, 20)
+    rb = 0.03
+    hb = 0.07
+    aw = 0.01
     base_x = rb * np.concatenate(([1], np.cos(av), [-1]))
     base_y = np.concatenate(([-hb], rb * np.sin(av), [-hb]))
     arm_x = np.concatenate(
-        (aw * np.sin(av - math.pi / 2), aw * np.sin(av + math.pi / 2)))
+        (aw * np.sin(av - np.pi / 2), aw * np.sin(av + np.pi / 2))
+    )
     arm_y = np.concatenate(
-        (aw * np.cos(av - math.pi / 2), -a1 + aw * np.cos(av + math.pi / 2)))
+        (aw * np.cos(av - np.pi / 2), -a1 + aw * np.cos(av + np.pi / 2))
+    )
 
     def __init__(self, ax=None, show=None):
         PyPlotVisualizer.__init__(self, ax=ax, show=show)
         self.set_name("pendulum_visualizer")
         self.DeclareInputPort("state", PortDataType.kVectorValued, 2)
 
         self.ax.set_xlim([-1.2, 1.2])
         self.ax.set_ylim([-1.2, 1.2])
-        # yapf: disable
         self.base = self.ax.fill(
-            self.base_x, self.base_y, zorder=1, facecolor=(.3, .6, .4),
-            edgecolor="k")
+            self.base_x,
+            self.base_y,
+            zorder=1,
+            facecolor=(0.3, 0.6, 0.4),
+            edgecolor="k",
+        )
 
         # arm_x and arm_y are closed (last element == first element), but don't
         # pass the last element to the fill command, because it gets closed
         # anyhow (and we want the sizes to match for the update).
         self.arm = self.ax.fill(
-            self.arm_x[0:-1], self.arm_y[0:-1], zorder=0, facecolor=(.9, .1, 0),
-            edgecolor="k")
+            self.arm_x[0:-1],
+            self.arm_y[0:-1],
+            zorder=0,
+            facecolor=(0.9, 0.1, 0),
+            edgecolor="k",
+        )
         self.center_of_mass = self.ax.plot(
-            0, -self.ac1, zorder=1, color="b", marker="o", markersize=14)
-        # yapf: enable
+            0, -self.ac1, zorder=1, color="b", marker="o", markersize=14
+        )
 
     def draw(self, context):
         if isinstance(context, Context):
             theta = self.EvalVectorInput(context, 0).get_value()[0]
             self.ax.set_title("t = {:.1f}".format(context.get_time()))
         else:
             theta = context[0]
             self.ax.set_title("")
 
         path = self.arm[0].get_path()
-        path.vertices[:, 0] = self.arm_x * math.cos(
-            theta) - self.arm_y * math.sin(theta)
-        path.vertices[:, 1] = self.arm_x * math.sin(
-            theta) + self.arm_y * math.cos(theta)
-        self.center_of_mass[0].set_data(self.ac1 * math.sin(theta),
-                                        -self.ac1 * math.cos(theta))
+        path.vertices[:, 0] = self.arm_x * np.cos(theta) - self.arm_y * np.sin(
+            theta
+        )
+        path.vertices[:, 1] = self.arm_x * np.sin(theta) + self.arm_y * np.cos(
+            theta
+        )
+        self.center_of_mass[0].set_data(
+            self.ac1 * np.sin(theta), -self.ac1 * np.cos(theta)
+        )
```

### Comparing `underactuated-2023.3.2/underactuated/plot_utils.py` & `underactuated-2023.4.17/underactuated/plot_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from copy import copy
-import numpy as np
-import matplotlib.pyplot as plt
 
+import matplotlib.pyplot as plt
+import numpy as np
 from pydrake.all import System
 
 
 def plot_2d_phase_portrait(f, x1lim=(-1, 1), x2lim=(-1, 1), n=100j, **kwargs):
     """
     Plots the phase portrait for a 2D dynamical system.
 
@@ -21,15 +21,15 @@
         Minimum and maximum values (floats) for the vertical axis of the
         plot.
     n : complex
         Purely imaginary number with imaginary part equal to the number of knot
         points on each axis of the plot.
     """
     # grid state space, careful here x2 before x1
-    X1, X2 = np.mgrid[x1lim[0]:x1lim[1]:n, x2lim[0]:x2lim[1]:n]
+    X1, X2 = np.mgrid[x1lim[0] : x1lim[1] : n, x2lim[0] : x2lim[1] : n]
     if isinstance(f, System):
         context = f.CreateDefaultContext()
         X1d = copy(X1)
         X2d = copy(X2)
         for i in range(X1.shape[0]):
             for j in range(X1.shape[1]):
                 context.SetContinuousState([X1[i, j], X2[i, j]])
@@ -39,18 +39,20 @@
     else:
         X1d, X2d = f([X1, X2])
 
     # color the streamlines according to the magnitude of xdot
     color = np.sqrt(X1d**2 + X2d**2)
 
     # phase portrait (annoying input format of streamplot)
-    strm = plt.streamplot(X1.T[0], X2[0], X1d.T, X2d.T, color=color.T, **kwargs)
+    strm = plt.streamplot(
+        X1.T[0], X2[0], X1d.T, X2d.T, color=color.T, **kwargs
+    )
 
     # colorbar on the right that measures the magnitude of xdot
-    plt.gcf().colorbar(strm.lines, label=r'$|\dot\mathbf{x}|$')
+    plt.gcf().colorbar(strm.lines, label=r"$|\dot\mathbf{x}|$")
 
     # misc plot settings
-    plt.xlabel(r'$x_1$')
-    plt.ylabel(r'$x_2$')
+    plt.xlabel(r"$x_1$")
+    plt.ylabel(r"$x_2$")
     plt.xlim(x1lim)
     plt.ylim(x2lim)
-    plt.gca().set_aspect('equal')
+    plt.gca().set_aspect("equal")
```

### Comparing `underactuated-2023.3.2/underactuated/pyplot_visualizer.py` & `underactuated-2023.4.17/underactuated/pyplot_visualizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-from matplotlib.widgets import Slider
 from matplotlib.animation import HTMLWriter
-
+from matplotlib.widgets import Slider
 from pydrake.systems.framework import VectorSystem
 
 
 class SliderSystem(VectorSystem):
-
     def __init__(self, ax, title, min, max):
         # 0 inputs, 1 output.
         VectorSystem.__init__(self, 0, 1)
         self.value = 0
         self.slider = Slider(ax, title, min, max, valinit=self.value)
         self.slider.on_changed(self.update)
 
@@ -23,9 +21,9 @@
 def AdvanceToAndSaveAnimation(simulator, visualizer, time, filename):
     visualizer.start_recording()
     simulator.AdvanceTo(time)
     ani = visualizer.get_recording_as_animation()
     # Note: Wanted to use embed_frames=True, but it did not render
     # the image properly for me.
     writer = HTMLWriter()
-    writer.frame_format = 'svg'
+    writer.frame_format = "svg"
     ani.save(filename, writer=writer)
```

### Comparing `underactuated-2023.3.2/underactuated/quadrotor2d.py` & `underactuated-2023.4.17/underactuated/quadrotor2d.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 import numpy as np
-
 from pydrake.systems.framework import LeafSystem_, PortDataType
 from pydrake.systems.pyplot_visualizer import PyPlotVisualizer
 from pydrake.systems.scalar_conversion import TemplateSystem
 
 # Note: In order to use the Python system with drake's autodiff features, we
 # have to add a little "TemplateSystem" boilerplate (for now).  For details,
 # see https://drake.mit.edu/pydrake/pydrake.systems.scalar_conversion.html
 
 
 # TODO(russt): Clean this up pending any resolutions on
 #  https://github.com/RobotLocomotion/drake/issues/10745
 @TemplateSystem.define("Quadrotor2D_")
 def Quadrotor2D_(T):
-
     class Impl(LeafSystem_[T]):
-
         def _construct(self, converter=None):
             LeafSystem_[T].__init__(self, converter)
             # two inputs (thrust)
             self.DeclareVectorInputPort("u", 2)
             # three positions, three velocities
             state_index = self.DeclareContinuousState(3, 3, 0)
             # six outputs (full state)
@@ -35,46 +32,57 @@
             Impl._construct(self, converter=converter)
 
         def DoCalcTimeDerivatives(self, context, derivatives):
             x = context.get_continuous_state_vector().CopyToVector()
             u = self.EvalVectorInput(context, 0).CopyToVector()
             q = x[:3]
             qdot = x[3:]
-            qddot = np.array([
-                -np.sin(q[2]) / self.mass * (u[0] + u[1]),
-                np.cos(x[2]) / self.mass * (u[0] + u[1]) - self.gravity,
-                self.length / self.inertia * (u[0] - u[1])
-            ])
+            qddot = np.array(
+                [
+                    -np.sin(q[2]) / self.mass * (u[0] + u[1]),
+                    np.cos(x[2]) / self.mass * (u[0] + u[1]) - self.gravity,
+                    self.length / self.inertia * (u[0] - u[1]),
+                ]
+            )
             derivatives.get_mutable_vector().SetFromVector(
-                np.concatenate((qdot, qddot)))
+                np.concatenate((qdot, qddot))
+            )
 
     return Impl
 
 
 Quadrotor2D = Quadrotor2D_[None]  # Default instantiation
 
 
 class Quadrotor2DVisualizer(PyPlotVisualizer):
-
     def __init__(self, ax=None, show=None):
         PyPlotVisualizer.__init__(self, ax=ax, show=show)
         self.DeclareInputPort("state", PortDataType.kVectorValued, 6)
         self.ax.set_aspect("equal")
         self.ax.set_xlim(-2, 2)
         self.ax.set_ylim(-1, 1)
 
-        self.length = .25  # moment arm (meters)
+        self.length = 0.25  # moment arm (meters)
 
-        self.base = np.vstack((1.2 * self.length * np.array([1, -1, -1, 1, 1]),
-                               0.025 * np.array([1, 1, -1, -1, 1])))
-        self.pin = np.vstack((0.005 * np.array([1, 1, -1, -1, 1]),
-                              .1 * np.array([1, 0, 0, 1, 1])))
+        self.base = np.vstack(
+            (
+                1.2 * self.length * np.array([1, -1, -1, 1, 1]),
+                0.025 * np.array([1, 1, -1, -1, 1]),
+            )
+        )
+        self.pin = np.vstack(
+            (
+                0.005 * np.array([1, 1, -1, -1, 1]),
+                0.1 * np.array([1, 0, 0, 1, 1]),
+            )
+        )
         a = np.linspace(0, 2 * np.pi, 50)
         self.prop = np.vstack(
-            (self.length / 1.5 * np.cos(a), .1 + .02 * np.sin(2 * a)))
+            (self.length / 1.5 * np.cos(a), 0.1 + 0.02 * np.sin(2 * a))
+        )
 
         # yapf: disable
         self.base_fill = self.ax.fill(
             self.base[0, :], self.base[1, :], zorder=1, edgecolor="k",
             facecolor=[.6, .6, .6])
         self.left_pin_fill = self.ax.fill(
             self.pin[0, :], self.pin[1, :], zorder=0, edgecolor="k",
@@ -88,33 +96,39 @@
         self.right_prop_fill = self.ax.fill(
             self.prop[0, :], self.prop[0, :], zorder=0, edgecolor="k",
             facecolor=[0, 0, 1])
         # yapf: enable
 
     def draw(self, context):
         x = self.EvalVectorInput(context, 0).CopyToVector()
-        R = np.array([[np.cos(x[2]), -np.sin(x[2])],
-                      [np.sin(x[2]), np.cos(x[2])]])
+        R = np.array(
+            [[np.cos(x[2]), -np.sin(x[2])], [np.sin(x[2]), np.cos(x[2])]]
+        )
 
         p = np.dot(R, self.base)
         self.base_fill[0].get_path().vertices[:, 0] = x[0] + p[0, :]
         self.base_fill[0].get_path().vertices[:, 1] = x[1] + p[1, :]
 
-        p = np.dot(R, np.vstack(
-            (-self.length + self.pin[0, :], self.pin[1, :])))
+        p = np.dot(
+            R, np.vstack((-self.length + self.pin[0, :], self.pin[1, :]))
+        )
         self.left_pin_fill[0].get_path().vertices[:, 0] = x[0] + p[0, :]
         self.left_pin_fill[0].get_path().vertices[:, 1] = x[1] + p[1, :]
-        p = np.dot(R, np.vstack((self.length + self.pin[0, :], self.pin[1, :])))
+        p = np.dot(
+            R, np.vstack((self.length + self.pin[0, :], self.pin[1, :]))
+        )
         self.right_pin_fill[0].get_path().vertices[:, 0] = x[0] + p[0, :]
         self.right_pin_fill[0].get_path().vertices[:, 1] = x[1] + p[1, :]
 
-        p = np.dot(R,
-                   np.vstack((-self.length + self.prop[0, :], self.prop[1, :])))
+        p = np.dot(
+            R, np.vstack((-self.length + self.prop[0, :], self.prop[1, :]))
+        )
         self.left_prop_fill[0].get_path().vertices[:, 0] = x[0] + p[0, :]
         self.left_prop_fill[0].get_path().vertices[:, 1] = x[1] + p[1, :]
 
-        p = np.dot(R, np.vstack(
-            (self.length + self.prop[0, :], self.prop[1, :])))
+        p = np.dot(
+            R, np.vstack((self.length + self.prop[0, :], self.prop[1, :]))
+        )
         self.right_prop_fill[0].get_path().vertices[:, 0] = x[0] + p[0, :]
         self.right_prop_fill[0].get_path().vertices[:, 1] = x[1] + p[1, :]
 
         self.ax.set_title("t = {:.1f}".format(context.get_time()))
```

### Comparing `underactuated-2023.3.2/underactuated/scenarios.py` & `underactuated-2023.4.17/underactuated/scenarios.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,85 +1,121 @@
 """
 This file contains a number of helper utilities to set up our various
 experiments with less code.
 """
 import numpy as np
-from pydrake.all import (BallRpyJoint, Box, CoulombFriction, Cylinder,
-                         PrismaticJoint, RevoluteJoint, RigidTransform,
-                         SpatialInertia, Sphere, UnitInertia)
+from pydrake.all import (
+    BallRpyJoint,
+    Box,
+    CoulombFriction,
+    Cylinder,
+    PrismaticJoint,
+    RevoluteJoint,
+    RigidTransform,
+    SpatialInertia,
+    Sphere,
+    UnitInertia,
+)
 
 
-def AddShape(plant, shape, name, mass=1, mu=1, color=[.5, .5, .9, 1.0]):
+def AddShape(plant, shape, name, mass=1, mu=1, color=[0.5, 0.5, 0.9, 1.0]):
     instance = plant.AddModelInstance(name)
     # TODO: Add a method to UnitInertia that accepts a geometry shape (unless
     # that dependency is somehow gross) and does this.
     if isinstance(shape, Box):
-        inertia = UnitInertia.SolidBox(shape.width(), shape.depth(),
-                                       shape.height())
+        inertia = UnitInertia.SolidBox(
+            shape.width(), shape.depth(), shape.height()
+        )
     elif isinstance(shape, Cylinder):
         inertia = UnitInertia.SolidCylinder(shape.radius(), shape.length())
     elif isinstance(shape, Sphere):
         inertia = UnitInertia.SolidSphere(shape.radius())
     else:
         raise RunTimeError(
-            f"need to write the unit inertia for shapes of type {shape}")
+            f"need to write the unit inertia for shapes of type {shape}"
+        )
     body = plant.AddRigidBody(
-        name, instance,
-        SpatialInertia(mass=mass,
-                       p_PScm_E=np.array([0., 0., 0.]),
-                       G_SP_E=inertia))
+        name,
+        instance,
+        SpatialInertia(
+            mass=mass, p_PScm_E=np.array([0.0, 0.0, 0.0]), G_SP_E=inertia
+        ),
+    )
     if plant.geometry_source_is_registered():
         if isinstance(shape, Box):
             plant.RegisterCollisionGeometry(
-                body, RigidTransform(),
-                Box(shape.width() - 0.001,
+                body,
+                RigidTransform(),
+                Box(
+                    shape.width() - 0.001,
                     shape.depth() - 0.001,
-                    shape.height() - 0.001), name, CoulombFriction(mu, mu))
+                    shape.height() - 0.001,
+                ),
+                name,
+                CoulombFriction(mu, mu),
+            )
             i = 0
             for x in [-shape.width() / 2.0, shape.width() / 2.0]:
                 for y in [-shape.depth() / 2.0, shape.depth() / 2.0]:
                     for z in [-shape.height() / 2.0, shape.height() / 2.0]:
                         plant.RegisterCollisionGeometry(
-                            body, RigidTransform([x, y, z]),
-                            Sphere(radius=1e-7), f"contact_sphere{i}",
-                            CoulombFriction(mu, mu))
+                            body,
+                            RigidTransform([x, y, z]),
+                            Sphere(radius=1e-7),
+                            f"contact_sphere{i}",
+                            CoulombFriction(mu, mu),
+                        )
                         i += 1
         else:
-            plant.RegisterCollisionGeometry(body, RigidTransform(), shape, name,
-                                            CoulombFriction(mu, mu))
+            plant.RegisterCollisionGeometry(
+                body, RigidTransform(), shape, name, CoulombFriction(mu, mu)
+            )
 
-        plant.RegisterVisualGeometry(body, RigidTransform(), shape, name, color)
+        plant.RegisterVisualGeometry(
+            body, RigidTransform(), shape, name, color
+        )
 
     return instance
 
 
 # https://github.com/RobotLocomotion/drake/issues/14949
 def AddFloatingRpyJoint(plant, frame, instance, use_ball_rpy=True):
-    inertia = SpatialInertia(mass=0,
-                             p_PScm_E=[0., 0., 0.],
-                             G_SP_E=UnitInertia(0, 0, 0))
+    inertia = SpatialInertia(
+        mass=0, p_PScm_E=[0.0, 0.0, 0.0], G_SP_E=UnitInertia(0, 0, 0)
+    )
     x_body = plant.AddRigidBody("x", instance, inertia)
     plant.AddJoint(
-        PrismaticJoint("x", plant.world_frame(), x_body.body_frame(),
-                       [1, 0, 0]))
+        PrismaticJoint(
+            "x", plant.world_frame(), x_body.body_frame(), [1, 0, 0]
+        )
+    )
     y_body = plant.AddRigidBody("y", instance, inertia)
     plant.AddJoint(
-        PrismaticJoint("y", x_body.body_frame(), y_body.body_frame(),
-                       [0, 1, 0]))
+        PrismaticJoint(
+            "y", x_body.body_frame(), y_body.body_frame(), [0, 1, 0]
+        )
+    )
     z_body = plant.AddRigidBody("z", instance, inertia)
     plant.AddJoint(
-        PrismaticJoint("z", y_body.body_frame(), z_body.body_frame(),
-                       [0, 0, 1]))
+        PrismaticJoint(
+            "z", y_body.body_frame(), z_body.body_frame(), [0, 0, 1]
+        )
+    )
     if use_ball_rpy:
         plant.AddJoint(BallRpyJoint("ball", z_body.body_frame(), frame))
     else:
         # RollPitchYaw is body z-y-x
         rz_body = plant.AddRigidBody("rz", instance, inertia)
         plant.AddJoint(
-            RevoluteJoint("rz", z_body.body_frame(), rz_body.body_frame(),
-                          [0, 0, 1]))
+            RevoluteJoint(
+                "rz", z_body.body_frame(), rz_body.body_frame(), [0, 0, 1]
+            )
+        )
         ry_body = plant.AddRigidBody("ry", instance, inertia)
         plant.AddJoint(
-            RevoluteJoint("ry", rz_body.body_frame(), ry_body.body_frame(),
-                          [0, 1, 0]))
+            RevoluteJoint(
+                "ry", rz_body.body_frame(), ry_body.body_frame(), [0, 1, 0]
+            )
+        )
         plant.AddJoint(
-            RevoluteJoint("rx", ry_body.body_frame(), frame, [1, 0, 0]))
+            RevoluteJoint("rx", ry_body.body_frame(), frame, [1, 0, 0])
+        )
```

### Comparing `underactuated-2023.3.2/underactuated.egg-info/PKG-INFO` & `underactuated-2023.4.17/underactuated.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: underactuated
-Version: 2023.3.2
+Version: 2023.4.17
 Summary: MIT 6.832 - Underactuated Robotics
 Home-page: https://underactuated.csail.mit.edu
 Author: Russ Tedrake
 Author-email: russt@mit.edu
 Project-URL: Bug Tracker, https://github.com/RussTedrake/underactuated/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `underactuated-2023.3.2/underactuated.egg-info/SOURCES.txt` & `underactuated-2023.4.17/underactuated.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 underactuated/__init__.py
 underactuated/double_integrator.py
 underactuated/jupyter.py
 underactuated/meshcat_cpp_utils.py
 underactuated/meshcat_utils.py
 underactuated/multibody.py
 underactuated/optimizers.py
+underactuated/package.xml
 underactuated/pendulum.py
 underactuated/plot_utils.py
 underactuated/pyplot_visualizer.py
 underactuated/quadrotor2d.py
 underactuated/scenarios.py
 underactuated/utils.py
 underactuated.egg-info/PKG-INFO
@@ -29,28 +30,30 @@
 underactuated/exercises/dp/test_lp_dp.py
 underactuated/exercises/dp/test_minimum_time.py
 underactuated/exercises/dp/test_pendulum_cvi.py
 underactuated/exercises/humanoids/test_footstep_planning.py
 underactuated/exercises/intro/test_drake_systems.py
 underactuated/exercises/lqr/test_drake_diagrams.py
 underactuated/exercises/lyapunov/test_control.py
+underactuated/exercises/lyapunov/test_sos_and_psd.py
 underactuated/exercises/lyapunov/test_van_der_pol.py
 underactuated/exercises/pend/test_hopfield_network.py
 underactuated/exercises/pend/test_vibrating_pendulum.py
 underactuated/exercises/planning/test_rrt_planning.py
 underactuated/exercises/simple_legs/test_one_d_hopper.py
 underactuated/exercises/sysid/test_glider_sysid.py
 underactuated/exercises/sysid/test_linear_sysid.py
 underactuated/exercises/trajopt/test_ilqr_driving.py
 underactuated/exercises/trajopt/test_orbital_transfer.py
 underactuated/exercises/trajopt/test_shooting_vs_transcription.py
 underactuated/models/cartpole.urdf
 underactuated/models/compass_gait_limit_cycle.urdf
 underactuated/models/double_pendulum.sdf
 underactuated/models/double_pendulum.urdf
+underactuated/models/kneed_compass_gait.urdf
 underactuated/models/one_d_hopper.urdf
 underactuated/models/undamped_cartpole.urdf
 underactuated/models/vibrating_pendulum.urdf
 underactuated/models/glider/glider.urdf
 underactuated/models/glider/meshes/elevator.obj
 underactuated/models/glider/meshes/fuselageh_hstab.obj
 underactuated/models/glider/meshes/fuselageh_main.obj
```

