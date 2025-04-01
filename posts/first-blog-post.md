---
title: Creative Coding Blog
published_at: 2025-03-04
snippet: Document for assignment 1
disable_html_sanitization: true
allow_math: true
---

# Homework 1a

<iframe id="Rozendaal Alternation" src="https://editor.p5js.org/panh/sketches/v3u2F78lq"></iframe>

<script type="module">

    const iframe  = document.getElementById (`Rozendaal Alternation`)
    iframe.width  = iframe.parentNode.scrollWidth
    iframe.height = iframe.width * 9 / 16 + 42

</script>

**2**

For this analysis, I’ve chosen “Into Time” by Rafaël Rozendaal.

**Observations:**

The artwork consists of smoothly shifting gradient colors.

It appears to be a grid-based composition.

The color transitions seem dynamic and continuous over time.

It gives a sense of infinite movement even though the shapes remain static.

**HOW IT MIGHT WORK**

**Grid Structure:**

The artwork likely uses nested loops to create a grid of rectangular shapes.

**Color Transitions:**

The colors smoothly transition between two or more hues.

This could be achieved using lerpColor() to interpolate between colors over time.

**Animation:**

The colors change continuously, suggesting they are updated using frameCount.

A time-based function (sin(), cos(), or noise()) could control color variation.

**Interaction:**

Some of Rozendaal’s works react to mouse movements.

This might involve using mouseX or mouseY to modify colors or grid placement.

**📌 Step 5: Useful Resources**

🔹 p5.js Reference


for loops – for creating a grid.

lerpColor() – for gradual color transitions.

sin() & cos() – for smooth animations.

🔹 p5.js Community


OpenProcessing – to explore similar sketches.

p5.js Discord – for feedback & debugging.

The Coding Train – great video tutorials.


## Homework 1b

🎯 Implementing a Concept: lerpColor() in a Grid


Based on my discussions, I decided to focus on color interpolation (lerpColor()), which was key to Rozendaal’s smooth transitions.

Here’s my p5.js sketch implementing this concept:

<iframe id="lerpColor" src="https://editor.p5js.org/panh/sketches/f4a6UMjxX"></iframe>

<script type="module">

    const iframe  = document.getElementById (`lerpColor`)
    iframe.width  = iframe.parentNode.scrollWidth
    iframe.height = iframe.width * 9 / 16 + 42
    </script>

   **How the Code Works:**

✔ Nested for loops create the grid of squares.

✔ lerpColor() smoothly blends colors from pink to blue.

✔ The time variable (t) controls the color shift, ensuring each square updates uniquely.

## Homework 2a

My AT1 project is a digital emotional support companion designed to be visually soft, playful, and interactive.

**Cute Visuals:** Soft & Expressive

Example: Blobby characters with big, blinking eyes.

Technique: Rounded shapes, smooth gradients, and eye movement for expressiveness.

**Cute Sounds:** Playful & Gentle

Example: Tiny "boop" sounds when clicked.

Technique: High-pitched, short sound effects using p5.sound.

**Cute Interactions:** Fun & Engaging

Example: Blobs wobble when clicked and follow the cursor.

Technique: Subtle size changes and smooth movement animations.

**Plan for AT1**

A friendly, responsive creature that reacts to clicks, blinks, and moves softly—offering a comforting digital presence.

## Homework 2b

**Who is My Kindred Spirit?**

My kindred spirit is an emotional support animal—not a physical one, but a digital presence. Just like real support animals bring comfort and joy, my p5.js project is designed to be an interactive, playful, and soothing experience.

**Context of Our Kinship**

We share a bond of care and companionship. Whether through soft movements, vibrant colors, or responsive interactions, this digital creature exists to bring a sense of warmth and ease.

**Our Common Purpose**

To create a calming, interactive digital companion that engages through motion, sound, and playfulness—bringing small moments of joy, just like an emotional support animal would.


## Homework 3a

**Analyzing Rafaël Rozendaal's Cute Aesthetic**

For this analysis, I chose another work by Rafaël Rozendaal and explored how it achieves a cute aesthetic.

*🌈 Visual Cuteness*

Soft pastels, gradients, and rounded shapes create a playful vibe.

Smooth, floating animations add a sense of lightness and joy.

*🎵 Sonic Cuteness*

If sound is present, it’s often bubbly, high-pitched, or chime-like.

These sounds enhance the feeling of whimsy and delight.

*🖱️ Interactive Cuteness*

Elements react playfully—bouncing, wiggling, or squishing.

Simple interactions make everything feel fun and alive!

**✨ Achieving Cuteness in My AT1 Project**

*🎨 Visuals:* Soft colors, blob-like shapes, and smooth motions.

*🔊 Sounds:* Playful clicks, gentle chimes, and bubbly tones.

*🕹️ Interactions:* Wiggly, bouncy responses to user input.

