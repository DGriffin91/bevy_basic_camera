# Basic Bevy Camera

Based on: https://github.com/bevyengine/bevy/pull/4458

Depends on bevy 0.8

`cargo run --example 3d_scene`

## Usage:

```rust
use bevy_basic_camera::{CameraController, CameraControllerPlugin};
```

```rust
app.add_plugin(CameraControllerPlugin)
```

```rust
// camera
commands.spawn_bundle(Camera3dBundle::default()).insert(CameraController::default());
```
