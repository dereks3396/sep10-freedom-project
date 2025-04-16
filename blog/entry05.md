# **Entry 5: Learning Aframe Blog**

04/15/25

---

## **Context:**
For this part of the project, I explored how to use A-Frame to build 3D scenes. My goal was to understand how rotation and positioning work in A-Frame. I used different shapes like boxes, circles, and cylinders to build creative 3D models. This helped me learn how objects can be placed and rotated in space. One of the big takeaways was seeing how child entities follow the rotation of their parent entity.

## **Content:**
**Tinker #1: Rotation and Parenting**
In my first test, I added a box that rotated 90 degrees and put a circle inside it. The circle followed the box's rotation. Here is a part of the code:

```html
<a-scene>
  <!-- Parent box with rotation -->
  <a-box color="#689F38" width="4" height="2" depth="0.2" position="0 1 -7" rotation="90 0 0">
    <!-- Circle inside the box -->
    <a-circle color="#333" side="double" position="2 0 0" rotation="90 0 0"></a-circle>
  </a-box>

  <!-- Another circle -->
  <a-circle color="#FFC107" side="double" position="-2 1 -7"></a-circle>

  <!-- Cylinder -->
  <a-cylinder color="#616161" height="2" radius="2" segments-radial="6" open-ended="true" side="double"></a-cylinder>
</a-scene>
```


**Tinker #2: Making a House**
I wanted to build a basic 3D house using simple shapes. I used a box for the base, a cone for the roof, and added windows and a door using thin boxes.

```html
<a-scene>
  <!-- Ground -->
  <a-plane position="0 0 -5" rotation="-90 0 0" width="10" height="10" color="#AED581"></a-plane>

  <!-- House Base -->
  <a-box position="0 1 -5" depth="4" height="2" width="4" color="#FFCC80"></a-box>

  <!-- Roof -->
  <a-cone position="0 2.5 -5" radius-bottom="3" radius-top="0" height="1" color="#8D6E63"></a-cone>

  <!-- Door -->
  <a-box position="0 0.5 -3.01" height="1" width="0.8" depth="0.1" color="#5D4037"></a-box>

  <!-- Windows -->
  <a-box position="-1 1.2 -3.01" height="0.5" width="0.5" depth="0.1" color="#90CAF9"></a-box>
  <a-box position="1 1.2 -3.01" height="0.5" width="0.5" depth="0.1" color="#90CAF9"></a-box>

  <!-- Chimney -->
  <a-box position="1 2.5 -5.5" depth="0.5" height="2" width="0.5" color="#BCAAA4"></a-box>
</a-scene>
```

This was a fun challenge. It made me think about how to use simple shapes in creative ways to make something more realistic.

## **EDP:**
During this step of the engineering design process, I explored how to model and test ideas using A-Frame. My goal was to see how wireless inventions could be imagined in 3D. I created different shapes and adjusted their positions, colors, and angles to practice building scenes. This hands-on tinkering helped me practice how to design and test digital models. I am learning how 3D tools can help us imagine new ideas, especially in the future of wireless communication.

## **Skills:**
This week, I practiced breaking down a big idea into small parts. Each tinker section was like a small challenge that helped me focus on just one skill, like rotation or building shapes. I also used creative thinking to imagine how I could turn simple shapes into something meaningful like a house or a pyramid. It helped me build my spatial thinking and grow my 3D design skills.

## **Next**
For the next step of my project, I plan to use A-Frame to create detailed 3D models of the wireless communication inventions I have imagined, using shapes that look more realistic and precise. For MindLink Messaging, I will design a futuristic headset with smooth, curved shapes and realistic textures, showing how thoughts turn into messages with floating text. The Smart Translator will be a portable device with clear, simple shapes like a screen and microphone, and users can click on it to see how it translates languages in real time. For the Holo Chat Projector, I will create a small, detailed device with buttons and ports, and show how it projects a 3D image of a person who moves with your hand gestures. These 3D models will let users interact with the inventions and understand how they work.
