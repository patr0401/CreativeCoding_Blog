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


Based on my discussions, I decided to focus on color interpolation (lerpColor()), which Emma suggested was key to Rozendaal’s smooth transitions.

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


## This is h2

*This is italic.*[^1]

[^1]: This is a footnote, *which can also be italic*.

**This is bold.**

Hyperlinks can be written like this: `[text](https://URL)`

You can find a markdown cheat-sheet [here](https://www.markdownguide.org/cheat-sheet/).

## Maths:

... which can be written inline, like this: $\{ x, y, z \} \in \N$

... or block, like this:

$$ x^2 + y^2 = z^2 $$

Visit [ $\KaTeX$ ](https://katex.org/docs/supported#fractions-and-binomials) for more information about writing maths.

## Embedding video:

<iframe id="coding_train_video" src="https://www.youtube.com/embed/rI_y2GAlQFM?si=RDgjkpunxk1mQzMI" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

<script type="module">

    console.log (`hello world! 🚀`)

    const iframe  = document.getElementById (`coding_train_video`)
    iframe.width  = iframe.parentNode.scrollWidth
    iframe.height = iframe.width * 9 / 16

</script>

## Embedding p5 sketches:

<iframe id="falling_falling" src="https://editor.p5js.org/capogreco/full/Fkg05m7aA"></iframe>

<script type="module">

    const iframe  = document.getElementById (`falling_falling`)
    iframe.width  = iframe.parentNode.scrollWidth
    iframe.height = iframe.width * 9 / 16 + 42

</script>

## Canvas API

<canvas id="canvas_example"></canvas>

<script type="module">
    const cnv = document.getElementById (`canvas_example`)
    cnv.width = cnv.parentNode.scrollWidth
    cnv.height = cnv.width * 9 / 16

    const ctx = cnv.getContext (`2d`)
    const pos = {
        x: -100,
        y: cnv.height / 2 - 50
    }
    
    function draw_frame () {
        ctx.fillStyle = `turquoise`
        ctx.fillRect (0, 0, cnv.width, cnv.height)

        ctx.fillStyle = `hotpink`
        ctx.fillRect (pos.x, pos.y, 100, 100)

        pos.x += 2

        if (pos.x > cnv.width) {
            pos.x = -100
        }

        requestAnimationFrame (draw_frame)
    }

    draw_frame ()
</script>


