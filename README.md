# Basic Bevy Camera

## Bevy now has a very similar built-in camera controller. I recommend using it instead:
```rs
use bevy::camera_controller::free_camera::{FreeCamera, FreeCameraPlugin};
```
```rs
app.add_plugins(FreeCameraPlugin);
```
```rs
commands.spawn((Camera3d::default(), FreeCamera::default()));
```


## bevy_basic_camera:

Based on: https://github.com/bevyengine/bevy/pull/4458

`cargo run --example 3d_scene`

Alternatively, consider using bevy's built in [free camera plugin](https://github.com/bevyengine/bevy/blob/a88af6573810f27c2f9d3fcf17b2543d0e379d18/examples/gizmos/3d_gizmos.rs#L55).

## Usage:

```toml
[dependencies]
bevy_basic_camera = { git = "https://github.com/DGriffin91/bevy_basic_camera" }
```

```rust
use bevy_basic_camera::{CameraController, CameraControllerPlugin};
```

```rust
app.add_plugin(CameraControllerPlugin)
```

```rust
// camera
commands.spawn(Camera3dBundle::default()).insert(CameraController::default());
```
