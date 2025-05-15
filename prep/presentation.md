# Presentation Plan

## Hook
<<<<<<< HEAD
*

## Product
*

## Process
*

## Conclusion
*
=======
* **Title**: “Imagine Communicating With Just a Thought”
* **Visual**: A quick animation or still of your MindLink headset hovering in 3D
* **One-liner**: “What if you could send a text without typing?”

## Product
* **Slide Title**: “Wireless Communication”
* **Embed**: **clickable demo link** or screenshot
  (https://dereks3396.github.io/sep10-freedom-project/)
* **Quick Tour**:
  * MindLink Messaging
  * Smart Translator
  * Holo Chat Projector

## Process

* Tool Learning & Coding**
  * **Tool Learning**:
    * Bootstrap for navbar and cards
    * A-Frame for 3D entities and animations
  * **Key Code Snippets**:
  ```html
  <!-- Smooth scroll JS -->
  <script>
    document.querySelectorAll('.nav-link').forEach(link =>
      link.addEventListener('click', e => {
        e.preventDefault();
        const tgt = document.querySelector(link.getAttribute('href'));
        window.scrollTo({ top: tgt.offsetTop - 70, behavior: 'smooth' });
      })
    );
  </script>


```html
<!-- A-Frame animated ring -->
<a-ring
  position="0 1 -0.5"
  radius-inner="0.6"
  radius-outer="0.7"
  animation="property: scale; to: 1.5 1.5 1.5; loop: true; dir: alternate; dur:1200"
></a-ring>
```

* **Challenges & Fixes**:

  * Aligning text panels on 3D objects → precise `position` offsets
  * Ensuring responsive design → Bootstrap grid and media queries

## Conclusion

* **Wrap-Up**: “From wireframes to an interactive website with 3D models, I built a showcase of futuristic inventions.”
* **Key Lessons**:

  1. **Wireframe first** avoids layout headaches
  2. **Modular CSS variables** simplify theming
* **Final Thought**: “Next step: exploring multiplayer VR chat rooms—imagine collaborating in 3D!”

>>>>>>> 54dbc401737b9cedb2e0f9e64ebb54e3ae6e26db

<!-- EXAMPLE

## Hook
* Verbal riddle of GGD

## Product
* GIF/Demo of example/non-example

## Process
* Flowchart of plan
  * MVP: noun -> door -> yes/no
  * Beyond MVP: noun -> word relation API -> noun API -> yes/no, with counterexample
* Code snippets of:
  * MVP
  * Both APIs
  * Challenge with API keys

## Conclusion
* [URL to project]
* Takeaways
  * Less = more: the heart of the riddle was one line of code; it obviously took more to make the entire thing work, but one complicated line of regular expressions was essentially the solution to the riddle
  * Expect the unexpected: it’s important to budget time for things you don’t account for; for example, I didn’t consider the fact that I would need another entire API to detect nouns
  * Determination is key: ironically enough, I had to make my API keys private. At first, it didn’t seem like it was possible, which meant I couldn’t publish my app. But after all of that hard work, I was determined to find a solution, and I found it in config variables.
* "Presentation can’t, but a speech can"


-->
