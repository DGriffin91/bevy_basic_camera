# Basic Bevy Camera

Based on: https://github.com/bevyengine/bevy/pull/4458

Currently depends on bevy main.

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