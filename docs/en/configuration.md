# Configuration Guide
Note: It is highly recommended to use the in-game interface rather than configuration files to modify settings.

## Configuration File Location
Configuration file is located at `.minecraft/config/pushdozer.json`

## Basic Configuration

### Work Mode Configuration
| Config Item | Description | Values | Default |
|------------|-------------|---------|---------|
| workMode | Work mode | "DESTROY"/"PLACE"/"SMOOTH" | "DESTROY" |
| displayMode | Display mode | "WIREFRAME"/"SURFACE"/"NONE" | "WIREFRAME" |

### Shape Configuration
| Config Item | Description | Values | Default |
|------------|-------------|---------|---------|
| shape | Shape type | "Box"/"Sphere" | "Box" |
| radius | Sphere radius | 1-32 | 5 |
| length | Box length | 1-32 | 5 |
| width | Box width | 1-32 | 5 |
| height | Box height | 1-32 | 5 |

### Operation Configuration
| Config Item | Description | Values | Default |
|------------|-------------|---------|---------|
| maxUndoSteps | Maximum undo steps | 1-30 | 30 |

## Advanced Configuration

### Block Filtering
```json
{
  "breakableBlockIds": [
    "minecraft:stone",
    "minecraft:dirt",
    "minecraft:grass_block"
  ],
  "ignoredBlockIds": [
    "minecraft:water",
    "minecraft:lava",
    "minecraft:air"
  ]
}
```

### Keybinding Configuration
```json
{
  "keyBindings": {
    "openConfig": "K",
    "toggleDisplay": "V",
    "changeMode": "G",
    "changeShape": "U",
    "undo": "CTRL+Z",
    "redo": "CTRL+Y",
    "increaseRange": "UP",
    "decreaseRange": "DOWN"
  }
}
```

## Configuration Example

### Complete Configuration File Example
```json
{
  "workMode": "DESTROY",
  "displayMode": "WIREFRAME",
  "maxOperationDistance": 30,
  "shape": "Box",
  "radius": 5,
  "length": 5,
  "width": 5,
  "height": 5,
  "maxUndoSteps": 30,
  "breakableBlockIds": ["minecraft:stone", "minecraft:dirt"],
  "ignoredBlockIds": ["minecraft:water", "minecraft:air"]
}
``` 