# Blog Entry: Trying A-Frame for 3D Web Development
#### Date: 03/02/2025

---

## Choosing A-Frame
For this project, I chose to try A-Frame, a tool for creating 3D and virtual reality experiences on the web. I decided to try it because it seemed like an easy way to add 3D elements to a webpage.

I found out that A-Frame works by using special tags like `<a-scene>`, `<a-box>`, and `<a-camera>`. This made me feel like I could start making 3D scenes without getting overwhelmed by complicated code.

## How I Tried A-Frame
To start, I created a simple 3D scene. I added a box and a camera (which is like the viewer’s eyes in the 3D world). Here is the first code I tried:

```html
<a-scene>
  <a-box position="0 1 -3" color="red"></a-box>
  <a-camera position="0 1.6 0"></a-camera>
</a-scene>
```
`<a-scene>` is the whole 3D world.

`<a-box>` creates a box, and I made it red and placed it at (0, 1, -3).

`<a-camera>` is where you look from in the scene, set at (0, 1.6, 0) to make it at eye level.

## What I Tried/Changed/Created
After that, I tried moving the box. I changed its position and color. Here is the updated code where I moved the box:

```html
<a-scene>
  <a-box position="2 1 -4" color="blue"></a-box>
  <a-camera position="0 1.6 0"></a-camera>
</a-scene>
```
In this version, I moved the box to the position (2, 1, -4), making it further to the right and further from the camera. I also changed its color to blue.

Then, I added another box:

```html
<a-scene>
  <a-box position="2 1 -4" color="blue"></a-box>
  <a-box position="-2 1 -4" color="green"></a-box>
  <a-camera position="0 1.6 0"></a-camera>
</a-scene>
```
Now, there are two boxes: one blue and one green. This shows how you can add more objects in the scene.

# Engineering Design Process

Right now, I am in the development stage of the engineering design process. I have started experimenting with basic A-Frame components. My next step is to add more objects to the scene and make it more interactive. I also plan to explore adding textures and lighting to make it look better.

## Skills

Through this project, I have learned two important skills:

1. **Creating 3D Objects**: I have learned how to make 3D objects in a web page, which is a new skill for me. This will be useful in the future for making more hard projects.
   
2. **Using HTML for 3D**: I have become more comfortable with using HTML to create and control 3D elements. This is a big step forward for me, especially because I did not know much about 3D content before.
