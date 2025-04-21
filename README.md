
# GSAP RESUBALE ANIM

A brief description of what this project does and who it's for


## Features

- Light/dark mode toggle
- Live previews
- Fullscreen mode
- Cross platform


## Installation

Install GSAP with CDN

```bash
<!-- GSAP Core -->
<script src="https://cdnjs.cloudflare.com/ajax/libs/gsap/3.12.2/gsap.min.js"></script>

<!-- Optional Plugins -->
<script src="https://cdnjs.cloudflare.com/ajax/libs/gsap/3.12.2/ScrollTrigger.min.js"></script>

```
    


Install GSAP with npm

```bash
npm install gsap
```
    
## ✨ Animation Catalog



 ###   Text Animations
 ```HTML
        <div class="text fade-up">Fade Up</div>
        <div class="text slide-in">Slide In</div>
        <div class="text pop-in">Pop In</div>
        <div class="text wave-text">Wave Motion</div>
        <div class="text stretch">Stretch Effect</div>
```
```javascript
        gsap.from(".fade-up", { opacity: 0, y: 30, duration: 1, ease: "power2.out" });
        gsap.from(".slide-in", { opacity: 0, x: -50, duration: 1, ease: "power2.out" });
        gsap.from(".pop-in", { scale: 0.5, opacity: 0, duration: 0.8, ease: "back.out(1.7)" });
        gsap.to(".wave-text", { rotation: 5, duration: 1.5, repeat: -1, yoyo: true, ease: "power1.inOut" });
        gsap.from(".stretch", { scaleX: 0.5, opacity: 0, duration: 1, ease: "power2.out" });
 ```










### Fade in
```javascript
  gsap.from(element, {
    opacity: 0,
    duration: 1,
    delay: 0,
    ease: "power2.out"
  });

```
### Slide in Left
```javascript
  gsap.from(element, {
    x: -100,
    opacity: 0,
    duration: 1,
    delay: 0,
    ease: "back.out(1.7)"
  });

```
### Slide in Right
```javascript
 gsap.from(element, {
    x: 100,
    opacity: 0,
    duration: 1,
    delay: 0,
    ease: "back.out(1.7)"
  });
 
```
### Bounce In
```javascript
 gsap.from(element, {
    y: -100,
    opacity: 0,
    duration: 1,
    delay: 0,
    ease: "bounce.out"
  });
 
```

### Scale Up
```javascript
gsap.from(element, {
    scale: 0,
    opacity: 0,
    duration: 1,
    delay: 0,
    ease: "elastic.out(1, 0.5)"
  });
 
```

### Rotate In
```javascript
gsap.from(element, {
    rotation: -180,
    opacity: 0,
    duration: 1,
    delay: 0,
    ease: "back.out(1.7)"
  });
 ```

 ### Staggered List Items
```javascript
gsap.from(container.children, {
    opacity: 0,
    y: 20,
    duration: 0.5,
    delay: 0,
    stagger: 0,
    ease: "power2.out"
  });
 ```

  ### Text Reveal
```javascript
gsap.from(element, {
    y: "100%",
    duration: 1,
    delay: 0,
    ease: "power3.out"
  });
 ```

   ### Flip In
```javascript
gsap.from(element, {
    rotationX: 90,
    opacity: 0,
    duration: 1,
    delay: 0,
    ease: "back.out(1.7)",
    transformOrigin: "50% 50%"
  });
 ```

   ###  Color Change
```javascript
gsap.to(element, {
    color:"#eeeeee" newColorNameInHexacode,
    duration: 1,
    delay: 0,
    ease: "power2.inOut"
  });
}
 ```

   ###  Background Color Change
```javascript
gsap.to(element, {
    backgroundColor: "#eeeeee" newColorNameInHexacode ,
    duration: 1,
    delay: 0,
    ease: "power2.inOut"
  });
 ```


   ###  Hover Pulse
```javascript
element.addEventListener("mouseenter", () => {
    gsap.to(element, {
      scale: 1.05,
      duration: 0.3,
      ease: "power2.out"
    });
  });
  
  element.addEventListener("mouseleave", () => {
    gsap.to(element, {
      scale: 1,
      duration: 0.3,
      ease: "power2.out"
    });
  });
 ```

  ###  Infinite Float
```javascript
gsap.to(element, {
    y: 10,
    duration: 3,
    repeat: -1,
    yoyo: true,
    ease: "sine.inOut"
  });
 ```

  ###  Infinite Rotation
```javascript
gsap.to(element, {
    rotation: 360,
    duration: 5,
    repeat: -1,
    ease: "none"
  });
 ```

  ###  Parallax Scroll
```javascript
function parallaxScroll(element, speed = 0.5) {
  gsap.to(element, {
    yPercent: speed * 100,
    ease: "none",
    scrollTrigger: {
      trigger: element,
      scrub: true
    }
  });
}
 ```

   ###  Scroll Triggered Fade In
```javascript
gsap.from(element, {
    opacity: 0,
    y: 50,
    duration: 1,
    scrollTrigger: {
      trigger: element,
      start: "top 80%",
      toggleActions: "play none none none"
    }
  });
 ```

 ###  Sequential Card Reveal
```javascript
function cardReveal(cards, stagger = 0.1, duration = 0.5) {
  return gsap.from(cards, {
    opacity: 0,
    y: 50,
    duration: duration,
    stagger: stagger,
    scrollTrigger: {
      trigger: cards[0].parentElement,
      start: "top 70%",
      toggleActions: "play none none none"
    }
  });
}
 ```
