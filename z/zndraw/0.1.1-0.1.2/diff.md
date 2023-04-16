# Comparing `tmp/zndraw-0.1.1.tar.gz` & `tmp/zndraw-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zndraw-0.1.1.tar", max compression
+gzip compressed data, was "zndraw-0.1.2.tar", max compression
```

## Comparing `zndraw-0.1.1.tar` & `zndraw-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0    13576 2023-04-12 16:10:14.508402 zndraw-0.1.1/LICENSE
--rw-r--r--   0        0        0     1054 2023-04-16 15:12:56.780430 zndraw-0.1.1/README.md
--rw-r--r--   0        0        0      646 2023-04-15 20:56:07.240790 zndraw-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      125 2023-04-15 20:56:00.080869 zndraw-0.1.1/zndraw/__init__.py
--rw-r--r--   0        0        0     2403 2023-04-16 13:08:44.451924 zndraw-0.1.1/zndraw/app.py
--rw-r--r--   0        0        0     2184 2023-04-16 13:36:29.983571 zndraw-0.1.1/zndraw/cli.py
--rw-r--r--   0        0        0     1222 2023-04-16 12:56:04.890308 zndraw-0.1.1/zndraw/globals.py
--rw-r--r--   0        0        0     1074 2023-04-15 22:53:05.753961 zndraw-0.1.1/zndraw/io.py
--rw-r--r--   0        0        0     4398 2023-04-16 11:38:33.242164 zndraw-0.1.1/zndraw/static/main.css
--rw-r--r--   0        0        0    14752 2023-04-16 14:54:27.672532 zndraw-0.1.1/zndraw/static/main.js
--rw-r--r--   0        0        0     9431 2023-04-16 14:55:41.771724 zndraw-0.1.1/zndraw/templates/index.html
--rw-r--r--   0        0        0     1691 1970-01-01 00:00:00.000000 zndraw-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    13576 2023-04-12 16:10:14.508402 zndraw-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1087 2023-04-16 21:37:27.597455 zndraw-0.1.2/README.md
+-rw-r--r--   0        0        0      663 2023-04-16 22:45:01.403863 zndraw-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      125 2023-04-15 20:56:00.080869 zndraw-0.1.2/zndraw/__init__.py
+-rw-r--r--   0        0        0     2123 2023-04-16 23:24:29.648456 zndraw-0.1.2/zndraw/app.py
+-rw-r--r--   0        0        0     2121 2023-04-16 23:27:51.346288 zndraw-0.1.2/zndraw/cli.py
+-rw-r--r--   0        0        0     1377 2023-04-16 23:24:33.028420 zndraw-0.1.2/zndraw/globals.py
+-rw-r--r--   0        0        0     1074 2023-04-15 22:53:05.753961 zndraw-0.1.2/zndraw/io.py
+-rw-r--r--   0        0        0     9533 2023-04-16 19:41:04.734213 zndraw-0.1.2/zndraw/static/favion-192x192.png
+-rw-r--r--   0        0        0     4541 2023-04-16 21:05:21.578456 zndraw-0.1.2/zndraw/static/main.css
+-rw-r--r--   0        0        0    18045 2023-04-16 23:24:48.368255 zndraw-0.1.2/zndraw/static/main.js
+-rw-r--r--   0        0        0    11491 2023-04-16 22:23:39.187556 zndraw-0.1.2/zndraw/templates/index.html
+-rw-r--r--   0        0        0     1762 1970-01-01 00:00:00.000000 zndraw-0.1.2/PKG-INFO
```

### Comparing `zndraw-0.1.1/LICENSE` & `zndraw-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.1/README.md` & `zndraw-0.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -18,12 +18,12 @@
 - atom_ids: list[int], the ids of the currently selected atoms
 - atoms: ase.Atoms, the configuration as `ase.Atoms` file where atom_ids where selected.
 
 and as an output:
 - list[ase.Atoms], a list of ase Atoms objects to display.
 
 ```python
-def function(atom_ids: list[int], atoms: ase.Atoms) -> list[ase.Atoms]:
+def function(atom_ids: list[int], atoms: ase.Atoms) -> list[ase.Atoms]|Generator[ase.Atoms, None, None]:
     ...
 ```
 
 ![Alt text](https://raw.githubusercontent.com/zincware/ZnDraw/main/misc/zndraw_ui.png "ZnDraw UI")
```

### Comparing `zndraw-0.1.1/pyproject.toml` & `zndraw-0.1.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [tool.poetry]
 name = "zndraw"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["zincwarecode <zincwarecode@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 ase = "^3.22.1"
 networkx = "^3.1"
 typer = {extras = ["all"], version = "^0.7.0"}
 flask = "^2.2.3"
+tqdm = "^4.65.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 ruff = "^0.0.261"
 pytest = "^7.3.0"
 
 [build-system]
```

### Comparing `zndraw-0.1.1/zndraw/cli.py` & `zndraw-0.1.2/zndraw/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -22,41 +22,40 @@
     sphere_size: float = typer.Option(1.0, help="size of the hydrogen sphere"),
     bond_size: float = typer.Option(1.0, help="size of a bond"),
     max_fps: int = typer.Option(100, help="Maximum frames per second"),
     update_function: str = typer.Option(
         None, help="Path to a python file with an update function 'module.function'."
     ),
     repeat: int = typer.Option(1, help="Repeat the trajectory n times"),
-    frame_buffer: int = typer.Option(
-        100,
-        help="Buffer size. Must be smaller than the total number of frames.",
-    ),
     resolution: int = typer.Option(5, help="Proportional to the number of polygons."),
     restart_animation: bool = typer.Option(
         False, help="run the animation in an endless loop."
     ),
-    frames_per_post: int = typer.Option(10, help="Number of frames to send per POST."),
+    frames_per_post: int = typer.Option(100, help="Number of frames to send per POST."),
     browser: bool = typer.Option(True, help="Open the browser automatically."),
 ):
     """ZnDraw: Visualize Molecules
 
     The ZnDraw CLI. Use 'zndraw version' to get the current version.
     """
     sys.path.insert(1, pathlib.Path.cwd().as_posix())
 
     if file == "version":
         version_callback()
 
+    if not pathlib.Path(file).exists():
+        typer.echo(f"File {file} does not exist.")
+        raise typer.Exit()
+
     globals.config.file = file
     globals.config.animate = animate
     globals.config.sphere_size = sphere_size
     globals.config.bond_size = bond_size
     globals.config.max_fps = max_fps
     globals.config.update_function = update_function
-    globals.config.frame_buffer = frame_buffer
     globals.config.resolution = resolution
     globals.config.frames_per_post = frames_per_post
     globals.config.restart_animation = restart_animation
     globals.config.repeat = (repeat, repeat, repeat)
 
     if browser:
         webbrowser.open(f"http://localhost:{port}")
```

### Comparing `zndraw-0.1.1/zndraw/globals.py` & `zndraw-0.1.2/zndraw/globals.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,53 @@
 import dataclasses
 import importlib
 
 import ase.io
+import tqdm
 
 
 @dataclasses.dataclass
 class Config:
     file: str = None
     animate: bool = None
     sphere_size: float = None
     bond_size: float = None
     max_fps: int = None
     update_function: str = None
-    frames_per_post: int = 10
+    frames_per_post: int = 100
     restart_animation: bool = False
     resolution: int = 5
     repeat: tuple = (1, 1, 1)
-    frame_buffer: int = 100
 
     def get_update_function(self):
         if self.update_function is None:
             return None
         module_name, function_name = self.update_function.rsplit(".", 1)
         module = importlib.import_module(module_name)
         return getattr(module, function_name)
 
+    def load_atoms(self):
+        if self.update_function is not None:
+            return
+        if len(_atoms_cache) > 1:
+            # already loaded
+            return
+        for idx, atom in enumerate(
+            tqdm.tqdm(ase.io.iread(self.file), desc="File Reading")
+        ):
+            _atoms_cache[idx] = atom
+
     def get_atoms(self, step=0) -> ase.Atoms:
         try:
-            return _atoms_cache[step]
+            return _atoms_cache[step].repeat(self.repeat)
         except KeyError:
-            if self.update_function is not None and step != 0:
+            if step != 0:
                 raise
-            for idx, atoms in enumerate(ase.io.iread(self.file)):
-                _atoms_cache[idx] = atoms.copy().repeat(self.repeat)
-                if step == 0:
-                    break
-
-        return _atoms_cache[step]
+            _atoms_cache[0] = ase.io.read(self.file)
+            return _atoms_cache[0]
 
 
 # TODO set defaults here and load in typer?
 
 _atoms_cache: dict = {}
 config = Config()
```

### Comparing `zndraw-0.1.1/zndraw/io.py` & `zndraw-0.1.2/zndraw/io.py`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.1/zndraw/static/main.css` & `zndraw-0.1.2/zndraw/static/main.css`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,24 @@
     position: absolute;
     bottom: 50%;
     left: 50%;
     z-index: 100;
     display: block;
 }
 
+#help_btn {
+    position: absolute;
+    top: 5px;
+    right: 10px;
+    width: 30px;
+    z-index: 100;
+    display: block;
+    opacity: 0.5;
+}
+
 .atom-spinner,
 .atom-spinner * {
     box-sizing: border-box;
 }
 
 .atom-spinner {
     height: 150px;
@@ -47,30 +57,30 @@
     height: 100%;
     width: 100%;
 }
 
 .atom-spinner .spinner-circle {
     display: block;
     position: absolute;
-    color: #ff00cc;
+    color: #ffa500;
     font-size: calc(60px * 0.24);
     top: 50%;
     left: 50%;
     transform: translate(-50%, -50%);
 }
 
 .atom-spinner .spinner-line {
     position: absolute;
     width: 100%;
     height: 100%;
     border-radius: 50%;
     animation-duration: 2s;
     border-left-width: calc(60px / 25);
     border-top-width: calc(60px / 25);
-    border-left-color: #ff00cc;
+    border-left-color: #ffa500;
     border-left-style: solid;
     border-top-style: solid;
     border-top-color: transparent;
 }
 
 .atom-spinner .spinner-line:nth-child(1) {
     animation: atom-spinner-animation-1 1s linear infinite;
@@ -223,15 +233,15 @@
     width: 40%;
     height: 100%;
     margin: 0;
     padding: 30px 0;
     /* padding from the top */
     list-style: none;
     background-color: #ECEFF1;
-    opacity: 90%;
+    opacity: 95%;
     box-shadow: 2px 2px 6px rgba(0, 0, 0, .4);
     transition-duration: .25s;
 }
 
 .menu__header {
     padding: 12px 24px;
     text-align: center;
```

### Comparing `zndraw-0.1.1/zndraw/static/main.js` & `zndraw-0.1.2/zndraw/static/main.js`

 * *Files 13% similar despite different names*

#### js-beautify {}

```diff
@@ -35,67 +35,147 @@
 const renderer = new THREE.WebGLRenderer({
     antialias: true,
     alpha: true
 });
 renderer.setSize(window.innerWidth, window.innerHeight);
 document.body.appendChild(renderer.domElement);
 
-const hemisphere_light = new THREE.HemisphereLight(0xffffff, 0x777777, 1);
-scene.add(hemisphere_light);
+const hemisphereLight = new THREE.HemisphereLight(0xffffff, 0x777777, 0.1);
+const spotLight = new THREE.SpotLight(0xffffff, 1);
+spotLight.position.set(0, 0, 100);
+scene.add(spotLight);
+
+scene.add(hemisphereLight);
 
 
 const atomsGroup = new THREE.Group();
 
 const bondsGroup = new THREE.Group();
 const bondsGroup_1 = new THREE.Group();
 const bondsGroup_2 = new THREE.Group();
 
 let node1 = new THREE.Vector3();
 let node2 = new THREE.Vector3();
 
+const materials = {
+    "MeshBasicMaterial": new THREE.MeshBasicMaterial({
+        color: "#ffa500"
+    }),
+    "MeshLambertMaterial": new THREE.MeshLambertMaterial({
+        color: "#ffa500"
+    }),
+    "MeshMatcapMaterial": new THREE.MeshMatcapMaterial({
+        color: "#ffa500"
+    }),
+    "MeshPhongMaterial": new THREE.MeshPhongMaterial({
+        color: "#ffa500"
+    }),
+    "MeshPhysicalMaterial": new THREE.MeshPhysicalMaterial({
+        color: "#ffa500"
+    }),
+    "MeshStandardMaterial": new THREE.MeshStandardMaterial({
+        color: "#ffa500"
+    }),
+    "MeshToonMaterial": new THREE.MeshToonMaterial({
+        color: "#ffa500"
+    }),
+
+};
+
 // some global variables
 let frames = [];
 let selected_ids = [];
 let animation_frame = 0;
 let scene_building = false;
 let animation_running = true;
+let data_loading = false;
+let fps = [];
+
 const div_info = document.getElementById('info');
 const div_loading = document.getElementById('loading');
 const div_progressBar = document.getElementById('progressBar');
 const div_bufferBar = document.getElementById('bufferBar');
 const div_greyOut = document.getElementById('greyOut');
 const div_lst_selected_ids = document.getElementById('lst_selected_ids');
 const div_FPS = document.getElementById('FPS');
 const div_n_particles = document.getElementById('n_particles');
 const div_n_bonds = document.getElementById('n_bonds');
+const div_help_container = document.getElementById('help_container');
 
 const o_selectAtoms = document.getElementById('selectAtoms');
 const o_autoRestart = document.getElementById('autoRestart');
 const o_animate = document.getElementById('animate');
 const o_reset_selection = document.getElementById('reset_selection');
 const o_hide_selection = document.getElementById('hide_selection');
 const o_reset = document.getElementById('reset');
 const o_max_fps = document.getElementById('max_fps');
-const o_frame_buffer = document.getElementById('frame_buffer');
 const o_frames_per_post = document.getElementById('frames_per_post');
 const o_sphere_plus = document.getElementById('sphere_plus');
 const o_sphere_minus = document.getElementById('sphere_minus');
 const o_bond_plus = document.getElementById('bond_plus');
 const o_bond_minus = document.getElementById('bond_minus');
 const o_resolution_plus = document.getElementById('resolution_plus');
 const o_resolution_minus = document.getElementById('resolution_minus');
+const o_materialSelect = document.getElementById('materialSelect');
+const o_wireframe = document.getElementById('wireframe');
+const o_spotLightIntensity = document.getElementById('spotLightIntensity');
+const o_hemisphereLightIntensity = document.getElementById('hemisphereLightIntensity');
+const o_help_btn = document.getElementById('help_btn');
 
 
 // Helper Functions
 
 async function load_config() {
     config = await (await fetch("config")).json();
     console.log(config)
 }
 
+async function update_materials() {
+    for (const material in materials) {
+        const option = document.createElement("option");
+        option.text = material;
+        option.value = material;
+        o_materialSelect.appendChild(option);
+    }
+    o_materialSelect.value = "MeshPhongMaterial";
+}
+
+function center_camera() {
+    // try to move the camera such that all atoms are in view
+
+    let trials = 0;
+
+    const frustum = new THREE.Frustum()
+
+    camera.position.x = 0;
+    camera.position.y = 0;
+    camera.position.z = 0;
+
+    atomsGroup.children.forEach((atom) => {
+
+        while (true) {
+            const matrix = new THREE.Matrix4().multiplyMatrices(camera.projectionMatrix, camera.matrixWorldInverse)
+            frustum.setFromProjectionMatrix(matrix)
+            camera.updateMatrix();
+            camera.updateMatrixWorld();
+            if (frustum.containsPoint(atom.position)) {
+                break;
+            }
+            console.log('Atom out of view');
+            camera.position.z += 1;
+            trials += 1;
+            if (trials > 100) {
+                break;
+            }
+        }
+    });
+}
+
+update_materials();
+
 function halfCylinderGeometry(pointX, pointY) {
     // Make the geometry (of "direction" length)
     var direction = new THREE.Vector3().subVectors(pointY, pointX);
 
     var geometry = new THREE.CylinderGeometry(0.15 * config["bond_size"], 0.15 * config["bond_size"], direction.length() / 2, config["resolution"] * 2);
     // // shift it so one end rests on the origin
     geometry.applyMatrix4(new THREE.Matrix4().makeTranslation(0, direction.length() / 4, 0));
@@ -119,19 +199,20 @@
     return mesh;
 }
 
 // Setup Scene
 
 function addAtom(item) {
     const geometry = new THREE.SphereGeometry(item["radius"] * config["sphere_size"], config["resolution"] * 4, config["resolution"] * 2);
-    const material = new THREE.MeshPhongMaterial({
-        color: item["color"]
-    });
-    const particle = new THREE.Mesh(geometry, material);
+
+    const particle = new THREE.Mesh(geometry, materials[o_materialSelect.value].clone());
     atomsGroup.add(particle);
+    particle.material.color.set(item["color"]);
+    particle.material.wireframe = o_wireframe.checked;
+
     particle.position.set(...item["position"]);
     particle.userData["id"] = item["id"];
     particle.userData["color"] = item["color"];
     particle.userData["bond_ids"] = [];
 }
 
 function addBond(item) {
@@ -191,14 +272,17 @@
 
     }
 
 
 }
 
 async function build_scene(step) {
+    if (scene_building) {
+        return;
+    }
     const urls = ["atoms/" + step, "bonds/" + step];
     animation_frame = step;
     console.log("Updating scene");
 
     div_loading.style.visibility = 'visible';
     div_greyOut.style.visibility = 'visible';
 
@@ -224,18 +308,16 @@
 await load_config();
 
 build_scene(0);
 
 // interactions
 
 camera.position.z = 50;
-
 const controls = new OrbitControls(camera, renderer.domElement);
 
-// camera.position.set( 0, 20, 100 );
 controls.update();
 
 function onWindowResize() {
     camera.aspect = window.innerWidth / window.innerHeight
     camera.updateProjectionMatrix()
     renderer.setSize(window.innerWidth, window.innerHeight)
     renderer.render(scene, camera);
@@ -289,42 +371,49 @@
         "body": JSON.stringify(selected_ids),
     })
 
     div_lst_selected_ids.innerHTML = selected_ids.join(", ");
 }
 
 async function getAnimationFrames() {
-    frames = [];
+    if (data_loading) {
+        console.log("Animation read already in progress");
+        return;
+    }
+    console.log("Loading animation frames");
 
-    await fetch("atoms/1")
-    load_config();
+    data_loading = true;
+    if (frames.length < 2) {
+        fetch("load");
+    }
 
-    let step = 0;
+    let step = frames.length;
     while (true) {
-        let obj = await (await fetch("atoms/" + step + "&" + (parseInt(o_frames_per_post.value) + step))).json();
+        let obj = await (await fetch("positions/" + step + "&" + (parseInt(o_frames_per_post.value) + step))).json();
+        console.log("Read " + step + "-" + (parseInt(o_frames_per_post.value) + step) + " frames");
         if (Object.keys(obj).length === 0) {
             console.log("Animation read finished");
             break;
         }
-        frames = frames.concat(obj); // TODO: handle multiple frames at once
+        frames = frames.concat(obj);
         step += parseInt(o_frames_per_post.value);
+        await fetch("atoms/1").then(load_config());
     }
+    data_loading = false;
 }
 
 
 if (config["animate"] === true) {
     div_info.innerHTML = "Reading file...";
     getAnimationFrames();
 }
 if (config["restart_animation"] === true) {
     o_autoRestart.checked = true;
 }
 
-console.log(config);
-
 window.addEventListener('pointerdown', onPointerDown, false);
 window.addEventListener('resize', onWindowResize, false);
 
 o_selectAtoms.onclick = function() {
     if (o_selectAtoms.checked) {
         console.log("Selecting atoms");
         window.addEventListener('pointerdown', onPointerDown, false);
@@ -352,26 +441,24 @@
         let mesh = atomsGroup.getObjectByUserDataProperty("id", item);
         mesh.visible = false;
 
         mesh.userData["bond_ids"].forEach(function(item, index) {
             bondsGroup_1.getObjectById(item).visible = false;
             bondsGroup_2.getObjectById(item).visible = false;
         });
-
-        // bondsGroup_1.getObjectById(item).visible = false;
-        // bondsGroup_2.getObjectByUserDataProperty("id", item).visible = false;
     });
 }
 
 o_reset.onclick = function() {
     load_config();
+    animation_frame = 0;
     build_scene(0);
     selected_ids = [];
     update_selection();
-    camera.position.z = 50;
+    center_camera();
 }
 
 o_sphere_plus.onclick = function() {
     config["sphere_size"] += 0.1;
     build_scene(animation_frame);
 }
 
@@ -396,40 +483,84 @@
 }
 
 o_resolution_minus.onclick = function() {
     config["resolution"] -= 1;
     build_scene(animation_frame);
 }
 
+o_materialSelect.onchange = function() {
+    build_scene(animation_frame);
+}
+
+o_wireframe.onchange = function() {
+    build_scene(animation_frame);
+}
+
+o_spotLightIntensity.oninput = function() {
+    document.getElementById("spotLightIntensity_output").value = o_spotLightIntensity.value;
+    spotLight.intensity = o_spotLightIntensity.value;
+}
+
+o_hemisphereLightIntensity.oninput = function() {
+    document.getElementById("hemisphereLightIntensity_output").value = o_hemisphereLightIntensity.value;
+    hemisphereLight.intensity = o_hemisphereLightIntensity.value;
+}
+
+o_help_btn.onmouseover = function() {
+    div_help_container.style.display = "block";
+}
+
+o_help_btn.onmouseout = function() {
+    div_help_container.style.display = "none";
+}
+
 window.addEventListener("keydown", (event) => {
     if (event.isComposing || event.key === " ") {
         event.preventDefault();
-        animation_running = !animation_running;
+        if (animation_running && animation_frame == frames.length - 1) {
+            animation_frame = 0;
+        } else {
+            animation_running = !animation_running;
+        }
     }
     if (event.isComposing || event.key === "ArrowLeft") {
         event.preventDefault();
         animation_frame = Math.max(0, animation_frame - 1);
     }
     if (event.isComposing || event.key === "ArrowRight") {
         event.preventDefault();
         animation_frame = Math.min(frames.length - 1, animation_frame + 1);
     }
     if (event.isComposing || event.key === "ArrowUp") {
-        animation_frame = frames.length - 1;
+        animation_frame = parseInt(Math.min(frames.length - 1, animation_frame + (frames.length / 10)));
     }
     if (event.isComposing || event.key === "ArrowDown") {
-        animation_frame = 0;
+        animation_frame = parseInt(Math.max(0, animation_frame - (frames.length / 10)));
+    }
+    if (event.isComposing || event.key === "l") {
+        spotLight.position.x = camera.position.x;
+        spotLight.position.y = camera.position.y;
+        spotLight.position.z = camera.position.z;
+    }
+    if (event.isComposing || event.key === "r") {
+        center_camera();
+    }
+    if (event.isComposing || event.key === "q") {
+        getAnimationFrames();
     }
 });
 
 if (config["update_function"] !== null) {
     window.addEventListener("keydown", (event) => {
         if (event.isComposing || event.key === "Enter") {
             div_info.innerHTML = "Processing...";
             fetch("update/" + animation_frame).then((response) => getAnimationFrames());
+            if (!data_loading) {
+                getAnimationFrames();
+            }
         }
     });
 }
 
 
 
 let move_atoms_clock = new THREE.Clock();
@@ -441,20 +572,14 @@
     }
     if (move_atoms_clock.getElapsedTime() < (1 / o_max_fps.value)) {
         return;
     }
     if (scene_building === true) {
         return;
     }
-    console.log("Animation (" + animation_frame + "/" + (frames.length - 1) + ")");
-    if (frames.length < parseInt(o_frame_buffer.value)) {
-        div_info.innerHTML = "Buffering...";
-        div_progressBar.style.width = (((frames.length - 1) / parseInt(o_frame_buffer.value)) * 100).toFixed(2) + "%";
-        return;
-    }
     div_progressBar.style.visibility = "hidden";
 
     if (animation_running === true) {
         if (animation_frame < frames.length - 1) {
             animation_frame += 1;
         } else if (o_autoRestart.checked === true) {
             animation_frame = 0;
@@ -473,17 +598,18 @@
     if (frames[animation_frame].length != atomsGroup.children.length) {
         // we need to update the scene
         build_scene(animation_frame);
         scene_building = true;
         return; // we need to wait for the scene to be updated
     }
 
+
+
     frames[animation_frame].forEach(function(item, index) {
-        atomsGroup.getObjectByUserDataProperty("id", item["id"]).position.set(...item["position"]);
-        // atomsGroup.children[item["id"]].position.set(...item["position"]);
+        atomsGroup.getObjectByUserDataProperty("id", index).position.set(...item);
     });
 
     div_info.innerHTML = "Frame (" + animation_frame + "/" + (frames.length - 1) + ")";
 
     if (config["bond_size"] > 0) {
         scene.updateMatrixWorld();
 
@@ -508,16 +634,25 @@
             bond_1.position.copy(node1);
             bond_2.position.copy(node2);
 
             bond_1.lookAt(node2);
             bond_2.lookAt(node1);
         }
     }
-    let fps = 1 / move_atoms_clock.getElapsedTime();
-    div_FPS.innerHTML = fps.toFixed(2) + " FPS";
+
+    fps.push(move_atoms_clock.getElapsedTime());
+
+    if (fps.length > 10) {
+        fps.shift();
+    }
+    if (!data_loading) {
+        getAnimationFrames();
+    }
+
+    div_FPS.innerHTML = (1 / (fps.reduce((a, b) => a + b, 0) / fps.length)).toFixed(2);
     move_atoms_clock.start();
 }
 
 function animate() {
 
     renderer.render(scene, camera);
     controls.update();
@@ -525,12 +660,10 @@
     if (frames.length > 0) {
         move_atoms();
     }
 
     // animation loop
 
     requestAnimationFrame(animate);
-
 }
 
-
 animate();
```

### Comparing `zndraw-0.1.1/zndraw/templates/index.html` & `zndraw-0.1.2/zndraw/templates/index.html`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 <!DOCTYPE html>
 <html>
 
 
 <head lang="en">
   <meta charset="utf-8">
   <title>ZnDraw</title>
+  <link rel="icon" type="image/x-icon" href="{{ url_for('static', filename='favion-192x192.png') }}">
   <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha3/dist/css/bootstrap.min.css" rel="stylesheet"
     integrity="sha384-KK94CHFLLe+nY2dmCWGMq91rCGa5gtU4mk92HdvYe+M/SXH301p5ILy+dN9+nJOZ" crossorigin="anonymous">
   <link rel="stylesheet" href="{{ url_for('static', filename='main.css') }}">
   <script async src="https://unpkg.com/es-module-shims@1.6.3/dist/es-module-shims.js"></script>
   <script type="importmap">
   {
     "imports": {
@@ -33,88 +34,97 @@
     </label>
 
     <ul class="menu__box">
       <h1 class="menu__header">ZnDraw</h1>
       <div class="accordion" id="accordionPanelsStayOpenExample">
         <div class="accordion-item">
           <h2 class="accordion-header" id="panelsStayOpen-headingOne">
-            <button class="accordion-button" type="button" data-bs-toggle="collapse"
-              data-bs-target="#panelsStayOpen-collapseOne" aria-expanded="true"
+            <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse"
+              data-bs-target="#panelsStayOpen-collapseOne" aria-expanded="false"
               aria-controls="panelsStayOpen-collapseOne">
               Settings
             </button>
           </h2>
-          <div id="panelsStayOpen-collapseOne" class="accordion-collapse collapse show"
+          <div id="panelsStayOpen-collapseOne" class="accordion-collapse collapse"
             aria-labelledby="panelsStayOpen-headingOne">
             <div class="container">
-              <div class="row">
-                <div class="col-sm">
-
-                  <div class="accordion-body">
+              <div class="accordion-body">
+                <div class="row">
+                  <div class="col-sm">
                     <div class="form-check form-switch">
                       <input class="form-check-input" type="checkbox" value="" id="selectAtoms" checked>
                       <label class="form-check-label" for="selectAtoms">
                         Select Atoms
                       </label>
                     </div>
                     <div class="form-check form-switch">
                       <input class="form-check-input" type="checkbox" value="" id="autoRestart">
                       <label class="form-check-label" for="autoRestart">
                         Auto Restart
                       </label>
                     </div>
 
+                    <select class="form-select" aria-label="Default select example" id="materialSelect">
+                      <option selected>Select Material</option>
+                    </select>
+
+                    <div class="form-check form-switch">
+                      <input class="form-check-input" type="checkbox" value="" id="wireframe">
+                      <label class="form-check-label" for="wireframe">
+                        Wireframe
+                      </label>
+                    </div>
+                  </div>
+                  <div class="col-sm">
                     <div class="row">
-                      <div class="col-auto">
-                        <label for="max_fps" class="form-label">Max FPS</label>
-                        <output id="max_fps_output">{{ config.max_fps }}</output>
+                      <div class="col-sm-3">
+                        <div class="row">Max FPS</div>
+                        <div class="row">POST</div>
+
+                        <div class="row">1. Light</div>
+                        <div class="row">2. Light</div>
                       </div>
-                      <div class="col-auto">
-                        <input type="range" class="form-range" min="1" max="100" step="0.5" id="max_fps"
-                          value="{{ config.max_fps }}" , oninput="max_fps_output.value = this.value">
+                      <div class="col-sm-2">
+                        <div class="row"><output id="max_fps_output">{{ config.max_fps }}</output></div>
+                        <div class="row"><output id="frames_per_post_output">{{ config.frames_per_post }}</output></div>
+
+                        <div class="row"><output id="spotLightIntensity_output">1</output></div>
+                        <div class="row"><output id="hemisphereLightIntensity_output">0.1</output></div>
                       </div>
-                    </div>
-                  </div>
+                      <div class="col-sm">
+                        <div class="row"><input type="range" class="form-range" min="1" max="100" step="0.5"
+                            id="max_fps" value="{{ config.max_fps }}" , oninput="max_fps_output.value = this.value">
+                        </div>
+                        <div class="row"><input type="range" class="form-range" min="1" max="500" id="frames_per_post"
+                            value="{{ config.frames_per_post }}" , oninput="frames_per_post_output.value = this.value">
+                        </div>
+
+                        <div class="row"><input type="range" class="form-range" min="0" max="1" step="0.01"
+                            id="spotLightIntensity" value="1"></div>
+                        <div class="row"><input type="range" class="form-range" min="0" max="1" step="0.01"
+                            id="hemisphereLightIntensity" value="0.1"></div>
+                      </div>
+                      <div class="col-sm-1"><!-- Padding on the right --></div>
 
-                </div>
-                <div class="col-sm">
-                  <div class="row">
-                    <div class="col-auto">
-                      <label for="frame_buffer" class="form-label">Initial Buffer Size</label>
-                      <output id="frame_buffer_output">{{ config.frame_buffer }}</output>
-                    </div>
-                    <div class="col-auto">
-                      <input type="range" class="form-range" min="1" max="1000" id="frame_buffer"
-                        value="{{ config.frame_buffer }}" , oninput="frame_buffer_output.value = this.value">
-                    </div>
-                  </div>
-                  <div class="row">
-                    <div class="col-auto">
-                      <label for="frames_per_post" class="form-label">POST Request Size</label>
-                      <output id="frames_per_post_output">{{ config.frames_per_post }}</output>
-                    </div>
-                    <div class="col-auto">
-                      <input type="range" class="form-range" min="1" max="100" id="frames_per_post"
-                        value="{{ config.frames_per_post }}" , oninput="frames_per_post_output.value = this.value">
                     </div>
                   </div>
                 </div>
               </div>
             </div>
           </div>
         </div>
         <div class="accordion-item">
           <h2 class="accordion-header" id="panelsStayOpen-headingTwo">
-            <button class="accordion-button" type="button" data-bs-toggle="collapse"
-              data-bs-target="#panelsStayOpen-collapseTwo" aria-expanded="true"
+            <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse"
+              data-bs-target="#panelsStayOpen-collapseTwo" aria-expanded="false"
               aria-controls="panelsStayOpen-collapseTwo">
               Controls
             </button>
           </h2>
-          <div id="panelsStayOpen-collapseTwo" class="accordion-collapse collapse show"
+          <div id="panelsStayOpen-collapseTwo" class="accordion-collapse collapse"
             aria-labelledby="panelsStayOpen-headingTwo">
             <div class="accordion-body">
 
               <div class="container">
                 <div class="row">
                   <div class="col-sm">
 
@@ -124,32 +134,28 @@
                       <button type="button" class="btn btn-secondary" id="reset_selection">Reset Selection</button>
                       <button type="button" class="btn btn-secondary" id="hide_selection" disabled>Hide
                         Selection</button>
                       <button type="button" class="btn btn-secondary" id="reset">Reset Scene</button>
                     </div>
                   </div>
                   <div class="col-sm">
-                    <div class="text-center">
-                      <div class="btn-group" role="group" aria-label="Basic example">
-                        <button type="button" class="btn btn-primary" id="sphere_plus">+</button>
-                        <button type="button" class="btn btn-primary" disabled>Particles</button>
-                        <button type="button" class="btn btn-primary" id="sphere_minus">-</button>
-                      </div>
-                      <p></p>
-                      <div class="btn-group" role="group" aria-label="Basic example">
-                        <button type="button" class="btn btn-primary" id="bond_plus">+</button>
-                        <button type="button" class="btn btn-primary" disabled>Bonds</button>
-                        <button type="button" class="btn btn-primary" id="bond_minus">-</button>
-                      </div>
-                      <p></p>
-                      <div class="btn-group" role="group" aria-label="Basic example">
-                        <button type="button" class="btn btn-primary" id="resolution_plus">+</button>
-                        <button type="button" class="btn btn-primary" disabled>Resolution</button>
-                        <button type="button" class="btn btn-primary" id="resolution_minus">-</button>
-                      </div>
+                    <div class="btn-group-vertical" role="group" aria-label="Basic example">
+                      <button type="button" class="btn btn-outline-dark" id="sphere_plus">+</button>
+                      <button type="button" class="btn btn-outline-dark" id="bond_plus">+</button>
+                      <button type="button" class="btn btn-outline-dark" id="resolution_plus">+</button>
+                    </div>
+                    <div class="btn-group-vertical" role="group" aria-label="Basic example">
+                      <button type="button" class="btn btn-outline-dark" disabled>Particles</button>
+                      <button type="button" class="btn btn-outline-dark" disabled>Bonds</button>
+                      <button type="button" class="btn btn-outline-dark" disabled>Resolution</button>
+                    </div>
+                    <div class="btn-group-vertical" role="group" aria-label="Basic example">
+                      <button type="button" class="btn btn-outline-dark" id="sphere_minus">-</button>
+                      <button type="button" class="btn btn-outline-dark" id="bond_minus">-</button>
+                      <button type="button" class="btn btn-outline-dark" id="resolution_minus">-</button>
                     </div>
                   </div>
                 </div>
               </div>
             </div>
           </div>
         </div>
@@ -161,14 +167,16 @@
               Info
             </button>
           </h2>
           <div id="panelsStayOpen-collapseThree" class="accordion-collapse collapse show"
             aria-labelledby="panelsStayOpen-headingThree">
             <div class="accordion-body">
               <dl class="row">
+                <dt class="col-sm-3">File</dt>
+                <dd class="col-sm-9"><code>{{ config.file }}</code></dd>
                 <dt class="col-sm-3">FPS</dt>
                 <dd class="col-sm-9" id="FPS">-</dd>
                 <dt class="col-sm-3">Particles</dt>
                 <dd class="col-sm-9" id="n_particles">-</dd>
                 <dt class="col-sm-3">Bonds</dt>
                 <dd class="col-sm-9" id="n_bonds">-</dd>
                 <dt class="col-sm-3">Selected IDs</dt>
@@ -198,11 +206,40 @@
       </div>
     </div>
   </div>
   <div id="info"></div>
   <div id="progressBar"></div>
   <div id="bufferBar"></div>
   <div id="greyOut"></div>
+  <img id="help_btn" src="https://openmoji.org/data/color/svg/2139.svg" />
+
+  <div class="container py-4" id="help_container" style="display: none; opacity: 0.9;">
+    <div class="h-100 p-5 bg-light rounded-3 border border-primary">
+      <h2>ZnDraw Help</h2>
+      <br>
+      <div class="rounded-3 bg-white" , style="padding-left: 10px;">
+        <dl class="row">
+          <dt class="col-sm-3">move light to camera position</dt>
+          <dd class="col-sm-9"><code>keypress L</code></dd>
+          <dt class="col-sm-3">play / pause</dt>
+          <dd class="col-sm-9"><code>keypress space</code></dd>
+          <dt class="col-sm-3">frame forwards / backwards</dt>
+          <dd class="col-sm-9"><code>keypress &#9654;\&#9664; </code></dd>
+          <dt class="col-sm-3">jump forwards / backwards</dt>
+          <dd class="col-sm-9"><code>keypress &#9650;\&#9660; </code></dd>
+          <dt class="col-sm-3">run update function</dt>
+          <dd class="col-sm-9"><code>keypress enter</code></dd>
+          <dt class="col-sm-3">reset camera position</dt>
+          <dd class="col-sm-9"><code>keypress R</code></dd>
+          <dt class="col-sm-3">reload animation</dt>
+          <dd class="col-sm-9"><code>keypress Q</code></dd>
+
+        </dl>
+      </div>
+    </div>
+  </div>
+
+
 
 </body>
 
 </html>
```

#### html2text {}

```diff
@@ -1,20 +1,47 @@
 
+
 ⁰
 ****** ZnDraw ******
 *****  Settings  *****
 *  Select Atoms
 ⁰  Auto Restart
-Max FPS {{ config.max_fps }}
+[One of: Select Material]
+⁰  Wireframe
+Max FPS
+POST
+1. Light
+2. Light
+{{ config.max_fps }}
+{{ config.frames_per_post }}
+1
+0.1
  oninput="max_fps_output.value = this.value">
-Initial Buffer Size {{ config.frame_buffer }}
- oninput="frame_buffer_output.value = this.value">
-POST Request Size {{ config.frames_per_post }}
  oninput="frames_per_post_output.value = this.value">
+[Unknown INPUT type]
+[Unknown INPUT type]
 *****  Controls  *****
 % if config.update_function %} disabled {% endif %}>Load Animation Reset
 Selection Hide Selection Reset Scene
-+ Particles -
-+ Bonds -
-+ Resolution -
++ + +
+Particles Bonds Resolution
+- - -
 *****  Info  *****
 ●
+[https://openmoji.org/data/color/svg/2139.svg]
+***** ZnDraw Help *****
+
+ style="padding-left: 10px;">
+  move light to camera position
+      keypress L
+  play / pause
+      keypress space
+  frame forwards / backwards
+      keypress ▶\◀
+  jump forwards / backwards
+      keypress ▲\▼
+  run update function
+      keypress enter
+  reset camera position
+      keypress R
+  reload animation
+      keypress Q
```

### Comparing `zndraw-0.1.1/PKG-INFO` & `zndraw-0.1.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: zndraw
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 License: Apache-2.0
 Author: zincwarecode
 Author-email: zincwarecode@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ase (>=3.22.1,<4.0.0)
 Requires-Dist: flask (>=2.2.3,<3.0.0)
 Requires-Dist: networkx (>=3.1,<4.0)
+Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
 Project-URL: repository, https://github.com/zincware/ZnDraw
 Description-Content-Type: text/markdown
 
 [![zincware](https://img.shields.io/badge/Powered%20by-zincware-darkcyan)](https://github.com/zincware)
 [![PyPI version](https://badge.fury.io/py/zndraw.svg)](https://badge.fury.io/py/zndraw)
 !['Threejs](https://img.shields.io/badge/threejs-black?style=for-the-badge&logo=three.js&logoColor=white)
@@ -37,13 +38,13 @@
 - atom_ids: list[int], the ids of the currently selected atoms
 - atoms: ase.Atoms, the configuration as `ase.Atoms` file where atom_ids where selected.
 
 and as an output:
 - list[ase.Atoms], a list of ase Atoms objects to display.
 
 ```python
-def function(atom_ids: list[int], atoms: ase.Atoms) -> list[ase.Atoms]:
+def function(atom_ids: list[int], atoms: ase.Atoms) -> list[ase.Atoms]|Generator[ase.Atoms, None, None]:
     ...
 ```
 
 ![Alt text](https://raw.githubusercontent.com/zincware/ZnDraw/main/misc/zndraw_ui.png "ZnDraw UI")
```

