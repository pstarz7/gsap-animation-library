
# workkkkk innnnnn progreeeeeeessssssssssssssssssssssssssssssssssssssss

this doucs not ready yet


## Features

- Installation
- Basic Animation Properties
- Quick Start Example
- Animation Catalog


## Installation

Install GSAP with CDN

```javascript
//GSAP Core 
<script src="https://cdnjs.cloudflare.com/ajax/libs/gsap/3.12.2/gsap.min.js"></script>

//Optional Plugins
<script src="https://cdnjs.cloudflare.com/ajax/libs/gsap/3.12.2/ScrollTrigger.min.js"></script>

```
    


Install GSAP with npm

```bash
npm install gsap


```

## Basic Animation Properties
#### Summary Cheat Sheet

```http
 https://gsap.com/
```

|
Property | Example  | What It Does             |
| :-------- | :------- | :------------------------- |
| **duration** | `duration: 2` | Animation length (seconds) |
| **delay**    | `delay: 1` | Pause before starting |
| **ease**     | `ease: "power2.out"` | Speed curve |
| **stagger**  | `stagger: 0.2` | Delay between elements |
| **x, y**     | `x: 100, y: "50%"` | Movement |
| **rotation**    | `rotation: 360` | Spin effect |
| **scale**    | `scale: 1.5` | Resize |
| **opacity**    | `opacity: 0` | Fade in/out |
| **scrollTrigger**    | `scrollTrigger: { trigger: ".box" }` |Scroll-based animation  |
| **scrub**    | `scrub: true` | Smooth scroll sync |
| **element**    | ` #element, .element  or h1 ,p, div & all tags` |  |


## GSAP Easing Functions Reference

### Basic Power Eases
| Type | Description |
|------|-------------|
| `"power0"` / `"linear"` | Constant speed (no easing) |
| `"power1.in"` | Starts slow, ends fast |
| `"power1.out"` | Starts fast, ends slow |
| `"power1.inOut"` | Smooth acceleration & deceleration |
| `"power2.in"` | Stronger slow start |
| `"power2.out"` | Stronger fast finish |
| `"power2.inOut"` | More pronounced smooth easing |
| `"power3.in"` | Very slow start |
| `"power3.out"` | Very fast end |
| `"power3.inOut"` | Dramatic smooth easing |
| `"power4.in"` | Extremely slow start |
| `"power4.out"` | Extremely fast end |
| `"power4.inOut"` | Most intense smooth easing |

### Special Effect Eases
| Type | Description |
|------|-------------|
| `"bounce.in"` | Bouncy start |
| `"bounce.out"` | Bouncy ending |
| `"bounce.inOut"` | Bounces at both start and end |
| `"elastic.in(1, 0.5)"` | Springy start |
| `"elastic.out(1, 0.5)"` | Elastic spring effect |
| `"elastic.inOut(1, 0.5)"` | Springy both directions |
| `"back.in"` | Pulls back before starting |
| `"back.out"` | Overshoots at end |
| `"back.inOut"` | Overshoots both directions |

### Smooth Motion Eases
| Type | Description |
|------|-------------|
| `"sine.in"` | Gentle slow start |
| `"sine.out"` | Gentle slow end |
| `"sine.inOut"` | Gentle wave-like motion |
| `"circ.in"` | Circular slow start |
| `"circ.out"` | Circular fast end |
| `"circ.inOut"` | Smooth circular motion |
| `"expo.in"` | Extremely slow start |
| `"expo.out"` | Extremely fast end |
| `"expo.inOut"` | Sharp acceleration/deceleration |

### Customizable Parameters
| Type | Parameters | Description |
|------|------------|-------------|
| `"elastic"` | `(intensity, period)` | `(1, 0.5)` = default spring effect |
| `"back"` | `(overshoot)` | `(1.7)` = default overshoot amount |

> **Note**: All eases work with `gsap.to()`, `gsap.from()`, and `gsap.fromTo()`.  
> Try them in the [GSAP Ease Visualizer](https://greensock.com/docs/v3/Eases).

```javascript
// Bounce example
gsap.to(".box", { 
  x: 100, 
  ease: "bounce.out" 
});
```

## Quick Start Example

#### Besic  gsap  syntax

```javascript
gsap.to("element", {
  duration: 2, // Takes 2 seconds to complete
  x: 200,
});
```


#### gsap with scrollTrigger syntax

```javascript
// Fade in and slide up on scroll
gsap.from("element", {
  duration: 1,
  delay: 0.2,
  y: 50,
  opacity: 0,
  ease: "power2.out",
  stagger: 0.1,
  scrollTrigger: {
    trigger: "element",
    start: "top 90%", //scrollTriggring pont. you can adjust
    toggleActions: "play none none none",
  },
});
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






##  Animations For All element's

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
