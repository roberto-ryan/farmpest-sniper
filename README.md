# FarmPest Sniper // Digital IR Optics

Night-vision pest control through a digital IR scope. Rats break cover across a farm at night, and you have a rifle, ten rounds and a sixty second window.

**Play:** https://roberto-ryan.github.io/farmpest-sniper/

## How to play

Two modes. **60s Clearance** gives you one minute to score as much as possible. **Endless Night Watch** keeps going until you stop.

Everything is scored through the optic. Rats are worth **100** points, headshots **150**. Accuracy is tracked, so spraying costs you.

### Desktop

- **Left click** fire
- **Right click or mouse wheel** zoom
- **Shift** hold breath, which steadies the scope and drains the breath bar
- **R** reload, ten rounds a magazine
- **F** cycle IR level
- **H** toggle the raw HUD on and off

### Touch

The screen buttons do the same thing: **ZOOM**, **IR**, **RAW**, **HOLD BREATH**, **RELOAD** and a large **FIRE** button. Drag to aim.

## About the optic

The scope is modelled as an 850 nm digital IR sight, so the world renders white-hot rather than in colour. You get zoom, an IR gain level, a breath meter that punishes holding too long, a magazine counter with an empty-mag hint, hit markers and a kill feed. Turning the raw HUD off leaves only the glass, which is how it is meant to be played once you know the controls.

## What is in the box

One file. `index.html` is the whole game, all of the markup, styling and logic inline.

It loads three dependencies from public CDNs, so it needs a network connection the first time: **three.js 0.160.0** as an ES module, **Tailwind CSS** for the interface, and **Inter** and **JetBrains Mono** from Google Fonts. Nothing is bundled, so there is no build step.

## Running locally

It is a single file, but it uses ES modules, so it needs to be served rather than opened off disk.

```
python3 -m http.server 8000
```

Then open http://127.0.0.1:8000/index.html
