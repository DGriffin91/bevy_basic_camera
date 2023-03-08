# Basic Bevy Camera

Based on: https://github.com/bevyengine/bevy/pull/4458

Depends on bevy 0.10

`cargo run --example 3d_scene`

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
