# A-Frame Learning Log

### How an A-Frame Scene Works
A basic scene contains:
- `<a-scene>` → The container for everything in the 3D world.
- `<a-entity>` → A general object that can be anything (box, sphere, light, camera, etc.).
- `<a-camera>` → The viewer’s perspective.

### Example of a Simple Scene
```html
<a-scene>
  <a-box position="0 1 -3" color="red"></a-box>
  <a-camera position="0 1.6 0"></a-camera>
</a-scene>
```

### Explanation of Code
- `<a-scene>` → The 3D world where objects exist.
- `<a-box>` → A cube with a set position and color.
  - `position="0 1 -3"` → Places it 0 left/right, 1 up, 3 units away from the camera.
  - `color="red"` → Makes it red.
- `<a-camera>` → Sets the point of view.
  - `position="0 1.6 0"` → Places it at eye level (1.6 meters high).

## Positioning Objects in 3D Space

### Understanding Coordinates (x, y, z)
- `x` → Moves left (-) or right (+).
- `y` → Moves down (-) or up (+).
- `z` → Moves closer (+) or farther away (-).
- Default position of any object is `0 0 0` (center of the scene).

### Example of Moving Objects
```html
<a-box position="2 1 -5" color="blue"></a-box>
<a-sphere position="-2 2 -3" color="green"></a-sphere>
```
- The box is 2 right, 1 up, and 5 units away.
- The sphere is 2 left, 2 up, and 3 units away.

## Shapes and Objects

### A-Frame Built-in Shapes
- **Box**: `<a-box>` (Attributes: depth, height, width)
- **Sphere**: `<a-sphere>` (Attributes: radius)
- **Cylinder**: `<a-cylinder>` (Attributes: radius, height)
- **Plane**: `<a-plane>` (Attributes: width, height)
- **Cone**: `<a-cone>` (Attributes: radius-bottom, radius-top, height)

### Example: Adding Different Shapes
```html
<a-scene>
  <a-box position="-1 1 -3" color="red"></a-box>
  <a-sphere position="1 2 -4" radius="1.25" color="blue"></a-sphere>
  <a-cylinder position="0 0.75 -5" radius="0.5" height="1.5" color="green"></a-cylinder>
</a-scene>
```

## Changing Size of Objects

### Example: Changing Size
```html
<a-box position="0 1 -3" width="2" height="2" depth="2" color="purple"></a-box>
<a-sphere position="2 2 -4" radius="0.5" color="yellow"></a-sphere>
```
- The box is now twice its normal size (2x2x2).
- The sphere has a smaller radius (0.5 instead of default 1).

## Rotating Objects

- Use `rotation="x y z"` attribute.
- Rotation is measured in degrees.
  - `rotation="0 45 0"` → Rotates 45° around the y-axis.
  - `rotation="90 0 0"` → Rotates 90° forward (x-axis).

### Example of Rotation
```html
<a-box position="0 1 -3" rotation="45 45 0" color="orange"></a-box>
```
- The box is tilted 45° on x and y axes.

## Using Colors and Textures

### Basic Colors
```html
<a-sphere color="blue"></a-sphere>
```

### Using Image Textures
- Textures make objects look more detailed.
- Use `src="image.jpg"` inside material.

#### Example: Adding a Texture
```html
<a-box src="wood.jpg" position="0 1 -3"></a-box>
```
- This applies a wood texture to the box.

## Adding a Sky (Background)

### Example: Sky with a Color
```html
<a-sky color="lightblue"></a-sky>
```

### Example: Sky with an Image
```html
<a-sky src="sky.jpg"></a-sky>
```

## Lighting in A-Frame

### Types of Lights
- **Ambient Light**: `<a-light type="ambient">` (Soft overall light)
- **Directional Light**: `<a-light type="directional">` (Sunlight effect)
- **Point Light**: `<a-light type="point">` (Light from a single spot)

### Example: Adding a Light
```html
<a-light type="directional" position="1 3 1"></a-light>
```
- This light shines from above and to the right.

## Parent-Child Positioning
- Objects inside another object move with it.
- Useful for grouping things together.

### Example: Parent-Child Objects
```html
<a-entity position="1 2 -3">
  <a-box position="0 0 0" color="red"></a-box>
  <a-sphere position="1 0 0" color="blue"></a-sphere>
</a-entity>
```
- The box and sphere follow the parent’s position `(1,2,-3)`.

## Camera and Viewing Perspective

### Moving the Camera
- Default camera is at `0 1.6 0` (eye level).
- Can move it using `position="x y z"`.

#### Example: Changing Camera Position
```html
<a-camera position="0 2 5"></a-camera>
```
- This moves the camera higher and farther back.

