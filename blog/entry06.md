# Entry 6: Building a Wireless Communication website
##### 5/11/2025

## Choosing My Topic

For this project I made a one-page website about wireless communication. I have always liked how fast new messaging apps and wireless gadgets are made. I wanted to create something fun to show these cool ideas. At first, I thought about doing smart home devices or wearable technology, but I chose wireless communication because it is a big part of our daily lives. It includes things like texting and new ideas like sending messages with our thoughts.

## Engineering Design Process

### Define the Problem

A lot of people do not know how many different types of wireless communication there are. My goal was to make a clear page that shows both popular apps like TextNow and Telegram, new gadgets like AirFly adapters and the Runaway Alarm Clock, and possible future inventions like a Mindlink Messaging Device, a Smart Translator, and a Holo chat Projector.

### Research & Ideation

I explored:

* [**Bootstrap**](https://getbootstrap.com) for responsive layout
* **CSS custom properties** for easy theming
* [**A-Frame**](https://aframe.io) for embedding simple 3D models

I sketched a three‐section layout:

1. **Current Tech** – Bootstrap cards
2. **Timeline** – Vertical CSS timeline
3. **Future Innovations** – A-Frame iframe

## Challenges & How I Fixed Them

### 1. Timeline Line Didn’t Stretch Full Height

**Problem:** My `.timeline::before` element wasn’t extending down the full container.

```css
.timeline::before {
  content: '';
  position: absolute;
  left: 7px;
  width: 2px;
  /* height: 100%; was collapsing */
}
```

**Fix:** I added `top: 0; bottom: 0;` instead of `height` so that the line spans dynamically:

```css
.timeline::before {
  top: 0;
  bottom: 0;
  left: 7px;
  width: 2px;
  background: var(--secondary);
}
```

### 2. Hero Text Hidden Behind Navbar

**Problem:** The fixed navbar was covering my hero title when links scrolled.
**Fix:** I updated the smooth-scroll script to subtract the navbar height:

```js
function scrollToSection(e) {
  e.preventDefault();
  const href = this.getAttribute("href");
  const targetTop = document.querySelector(href).offsetTop;
  const navHeight = document.querySelector('.navbar').offsetHeight;
  window.scroll({ top: targetTop - navHeight, behavior: 'smooth' });
}
```

### 3. A-Frame Embed Overflow

**Problem:** The 3D iframe overflowed its container on mobile.
**Fix:** I wrapped it in a responsive div with a 16:9 ratio:

```css
.aframe-container {
  position: relative;
  width: 100%;
  padding-bottom: 56.25%;
  height: 0;
  overflow: hidden;
}
.aframe-container iframe {
  position: absolute;
  width: 100%;
  height: 100%;
  top: 0; left: 0;
  border: 0;
}
```

## Skills

- I learned to combine `.row` and `.col-md-4` in Bootstrap to create fluid grids for responsive layouts.
- I used `:root` properties like `--primary` and `--secondary` in CSS to easily switch colors for theming.
- I built a vertical timeline using `::before` pseudo-elements and positioned markers with CSS.
- I created and embedded 3D scenes using `<a-box>`, `<a-sphere>`, and animations with WebVR and A-Frame.

## Next Steps

For my next project or if I have time on this one, I plan to add a 360 degree rotation so users can move the devices around. I will also add a zoom feature to help users see the parts of the devices better. A view of the components will let users look at the details of the devices. I also want to add a dark mode option for easier use. Finally, I will include smooth scroll animations to make the website feel nicer to use.


[Previous](entry05.md) | [Next](entry07.md)

[Home](../README.md)
