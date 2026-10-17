# Gradient descent: learning rate explorer

An interactive, single-file HTML demo that shows how the learning rate changes the way gradient descent moves across a loss curve.

> **Inspiration:** This project was inspired by the Medium post [“Andrej Karpathy’s New suggestion- Ask AI output in ASD-STE100 format and not in Text format”](https://medium.com/neuralnotions/andrej-karpathys-new-suggestion-ask-ai-output-in-asd-ste100-format-and-not-in-text-format-b7b753f52f32) by Nikhil (Neural Notions). The post discusses asking AI for diagrams, interactive HTML pages and explanatory animations instead of plain text.

## What it shows

A ball sits on a loss curve with two valleys, one deep and one shallow. The learning-rate slider runs on a log scale from 0.001 to 1. Before each step, an arrow shows how far the ball will move (η × slope) and a dashed tangent line shows the slope it’s using. The panel shows the update with real numbers filled in, for example `w ← 3.60 − 0.050 × 11.86 = 3.01`. A small chart tracks the loss over time.

## Presets for lecturing

There are four, chosen so each one teaches something:

- “Too small” crawls toward the bottom.
- “Steady” settles in the shallow valley, which shows a local minimum.
- “Bold” hops over the hill into the deeper valley.
- “Too large” diverges and the ball flies off the chart.

## Controls

You can click anywhere on the curve to set a new starting point. Keyboard shortcuts work too:

| Key | Action |
| --- | --- |
| `Space` | Play or pause |
| `→` | Take one step |
| `R` | Reset |
| `1`–`4` | Pick a preset |

## Running it

Open `index.html` in any modern browser, or visit the GitHub Pages site for this repository. Tailwind CSS and the web font load from a CDN; if you are offline, built-in fallback styles keep the layout working.
