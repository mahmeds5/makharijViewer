# Makharij Viewer

An interactive 3D model of the mouth and throat for teaching the **makharij al-huruf** (articulation points of the Arabic letters) in tajweed.

Most tajweed material uses flat 2D diagrams. This lets a teacher move the tongue, open the jaws, fade parts in and out, and look from inside the mouth, so students can actually see where each letter comes from.

> **Important:** the model is stylized and the tongue positions are approximate. Have a qualified teacher verify each point before using this for instruction.

## Features

- **17 makharij presets**, grouped as jawf, halq, lisan, shafatain and khayshum. Each preset moves the tongue, highlights the exact point and shows the letters.
- **Independent controls** for four tongue regions (back, middle, blade, tip), tip forward/back, lower jaw and upper jaw. Each control moves only its own part.
- **Per-part opacity** for upper and lower jaw skin, teeth, gums, tongue, palate, mouth floor, throat wall and nasal passage.
- **Optional cutaway** that slices the head down the middle.
- **Camera views:** outside, front, inside the mouth, on the tongue, palate, throat and tongue close-up. You can also drag to rotate and scroll or pinch to zoom.

## Run it

1. Download `makharij-viewer.html`.
2. Open it in any modern browser.

There is no build step and no install. It loads [three.js](https://threejs.org/) (r128) from a CDN, so you need an internet connection the first time.

## How to use it

- Pick a letter group on the left. The tongue moves and the point lights up.
- Adjust any slider on the right to fine-tune the view. Selecting a letter doesn't lock the controls.
- Use the buttons at the bottom of the 3D view to switch camera angles.
- Turn down skin opacity (or individual part opacity) to see inside.

## Known limitations

- The model is code-built geometry, not a medical-grade anatomical scan.
- Dad is hard to show from a side view, since it involves the side of the tongue.
- Tongue poses are approximations and haven't been formally reviewed.
- Scholars count the makharij differently (17 is the common count, but some use 14 or 29). This uses 17.
- On phones the layout stacks vertically and scrolls. It's designed for a laptop or projector screen.

## Roadmap

- Teacher-verified poses for every point
- Drag handles to move the tongue directly
- More realistic head and teeth model
- Saved custom presets
- Side-of-tongue and top-down views for dad and similar points

## Tech

- Plain HTML, CSS and JavaScript in a single file
- [three.js](https://threejs.org/) for 3D rendering

## Contributing

Feedback from tajweed teachers is the most valuable thing here. If you spot a wrong or misleading position, please open an issue with the letter and what should change.

## License

MIT. See the `LICENSE` file.
