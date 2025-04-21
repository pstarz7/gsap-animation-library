 GSAP ANIMATION LIBARARY (easy to use for developers just copy and paste)


work in progressssssssssssssssssssss


![image alt](https://github.com/pstarz7/gsap-animation-library/blob/d4e209677802cd6ec0159ce6e2974de009ce077b/istockphoto-508408464-612x612.jpg)


# GSAP Animation Library 🚀

A collection of 20+ reusable GSAP animations for your web projects. Easy to implement, customizable, and production-ready.

## Table of Contents
- [Installation](#installation)
- [Usage](#usage)
  - [Via CDN](#via-cdn)
  - [Via NPM](#via-npm)
- [Animation List](#animation-list)
- [Contributing](#contributing)
- [License](#license)

## Installation

### Via CDN

Add these scripts to your HTML file's `<head>` section:

```html
<!-- GSAP Core -->
<script src="https://cdnjs.cloudflare.com/ajax/libs/gsap/3.12.2/gsap.min.js"></script>

<!-- ScrollTrigger (optional, for scroll-based animations) -->
<script src="https://cdnjs.cloudflare.com/ajax/libs/gsap/3.12.2/ScrollTrigger.min.js"></script>

<!-- MorphSVG (optional, for SVG morphing) -->
<script src="https://cdnjs.cloudflare.com/ajax/libs/gsap/3.12.2/MorphSVGPlugin.min.js"></script>
Via NPM
bash
npm install gsap
Then import in your JavaScript file:

javascript
import { gsap } from "gsap";
import { ScrollTrigger } from "gsap/ScrollTrigger";
import { MorphSVGPlugin } from "gsap/MorphSVGPlugin";

// Register plugins
gsap.registerPlugin(ScrollTrigger, MorphSVGPlugin);
Usage
Include GSAP (see installation above)

Copy the animation functions you need into your project

Call them with your target elements:

javascript
// Basic usage
fadeIn(".my-element");

// With custom parameters
slideInLeft("#header", 1.5, 0.3);
Animation List
1. fadeIn
Description: Smooth fade-in effect
Parameters:

element (Selector or DOM element) - Target element(s)

duration (Number, default: 1) - Animation duration in seconds

delay (Number, default: 0) - Delay before animation starts

javascript
fadeIn(".hero-section", 1.5, 0.2);
2. slideInLeft
Description: Slides element in from left with bounce
Parameters:

element (Selector or DOM element)

duration (Number, default: 1)

delay (Number, default: 0)

javascript
slideInLeft(".feature-card", 1, 0.3);
3. slideInRight
Description: Slides element in from right with bounce
Parameters: Same as slideInLeft

javascript
slideInRight(".sidebar", 0.8);
4. bounceIn
Description: Drops element with playful bounce
Parameters:

element (Selector or DOM element)

duration (Number, default: 1)

delay (Number, default: 0)

javascript
bounceIn(".notification", 1.2);
5. scaleUp
Description: Scales element up with elastic effect
Parameters:

element (Selector or DOM element)

duration (Number, default: 1)

delay (Number, default: 0)

javascript
scaleUp(".modal", 1.5);
6. rotateIn
Description: Rotates element into view
Parameters:

element (Selector or DOM element)

duration (Number, default: 1)

delay (Number, default: 0)

javascript
rotateIn(".logo", 1.2);
7. staggerListItems
Description: Animates list items sequentially
Parameters:

container (Selector or DOM element) - Parent of list items

duration (Number, default: 0.5) - Duration per item

delay (Number, default: 0) - Initial delay

stagger (Number, default: 0.1) - Delay between items

javascript
staggerListItems(".nav-menu", 0.3, 0, 0.15);
8. textReveal
Description: Reveals text like it's being uncovered
Parameters:

element (Selector or DOM element)

duration (Number, default: 1)

delay (Number, default: 0)

javascript
textReveal(".headline", 1.5);
9. flipIn
Description: 3D flip animation
Parameters:

element (Selector or DOM element)

duration (Number, default: 1)

delay (Number, default: 0)

javascript
flipIn(".product-card", 1.2);
10. colorChange
Description: Smooth color transition
Parameters:

element (Selector or DOM element)

newColor (String) - Target color

duration (Number, default: 1)

delay (Number, default: 0)

javascript
colorChange(".button", "#ff5733", 0.8);
11. bgColorChange
Description: Smooth background color transition
Parameters: Same as colorChange

javascript
bgColorChange(".section", "#f8f8f8", 1);
12. hoverPulse
Description: Pulse effect on hover
Parameters:

element (Selector or DOM element)

scale (Number, default: 1.05) - Scale amount

duration (Number, default: 0.3) - Animation duration

javascript
hoverPulse(".btn", 1.1, 0.2);
13. infiniteFloat
Description: Continuous floating up/down
Parameters:

element (Selector or DOM element)

distance (Number, default: 10) - Pixels to move

duration (Number, default: 3) - Duration per cycle

javascript
infiniteFloat(".floating-icon", 15, 4);
14. infiniteRotate
Description: Continuous rotation
Parameters:

element (Selector or DOM element)

rotation (Number, default: 360) - Degrees per cycle

duration (Number, default: 5) - Duration per cycle

javascript
infiniteRotate(".loading-spinner", 360, 2);
15. morphSVG
Description: Morphs SVG shape to another
Parameters:

element (Selector or DOM element) - SVG path

newPath (String) - Target path data

duration (Number, default: 1)

delay (Number, default: 0)

javascript
morphSVG("#shape", "M10,10 L90,10 L90,90 L10,90 Z", 1.5);
16. drawSVG
Description: Draws SVG path progressively
Parameters:

element (Selector or DOM element) - SVG path

duration (Number, default: 1)

delay (Number, default: 0)

javascript
drawSVG("#path", 2);
17. parallaxScroll
Description: Creates parallax scroll effect
Parameters:

element (Selector or DOM element)

speed (Number, default: 0.5) - 0 to 1 (0=no move, 1=fast)

javascript
parallaxScroll(".parallax-bg", 0.3);
18. scrollFadeIn
Description: Fades in element when scrolled to
Parameters:

element (Selector or DOM element)

duration (Number, default: 1)

javascript
scrollFadeIn(".section", 1.2);
19. cardReveal
Description: Sequential reveal of card elements
Parameters:

cards (Selector or DOM elements)

stagger (Number, default: 0.1) - Delay between cards

duration (Number, default: 0.5) - Duration per card

javascript
cardReveal(document.querySelectorAll(".card"), 0.15, 0.6);
20. typingEffect
Description: Simulates typing text
Parameters:

element (Selector or DOM element)

duration (Number, default: 1)

delay (Number, default: 0)

javascript
typingEffect(".typewriter", 2, 0.5);
Contributing
Fork the repository

Create your feature branch (git checkout -b feature/AmazingFeature)

Commit your changes (git commit -m 'Add some AmazingFeature')

Push to the branch (git push origin feature/AmazingFeature)

Open a Pull Request

License
Distributed under the MIT License. See LICENSE for more information.


This documentation includes:
1. Clear installation instructions for both CDN and NPM
2. Usage examples
3. Detailed documentation for each animation with:
   - Description of what it does
   - All parameters with defaults
   - Example usage
4. Contribution guidelines
5. License information

The formatting uses proper Markdown syntax for GitHub readability with:
- Clear section headers
- Code blocks with syntax highlighting
- Consistent parameter documentation
- Visual separation between different animations
