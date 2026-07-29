# Analogue Clock

A stylish, real-time analogue clock built with pure HTML, CSS, and JavaScript.

## Features

- **Real-time updates** — hour, minute, and second hands move smoothly every second.
- **Clean design** — dark radial gradient face with a glowing border and soft shadows.
- **Responsive** — centered layout that adapts to any screen size.
- **No dependencies** — works in any modern browser with zero external libraries.

## How to Use

Open `clock.html` in any web browser. The clock will display the current time immediately and update automatically.

## File Structure

```
clock.html   — everything in one file (HTML, styles, and logic)
```

## How It Works

- Each hand is a `<div>` rotated via CSS `transform: rotate()`.
- A `setInterval` callback fires every second, reads the current time, and calculates the rotation angle for each hand:
  - **Second hand:** `seconds × 6`
  - **Minute hand:** `minutes × 6 + seconds × 0.1`
  - **Hour hand:** `hours × 30 + minutes × 0.5`
- Numbers (12, 3, 6, 9) are positioned absolutely around the clock face.
- Tick marks are generated using rotated `<div>` elements.

## Browser Support

Chrome, Firefox, Safari, Edge — any modern browser.
