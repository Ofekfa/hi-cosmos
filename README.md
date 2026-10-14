# ✦ Hi Cosmos

A voice-controlled gravity sandbox that runs entirely in the browser. Say **"Hi Cosmos, create the solar system"** and watch it happen.

**▶ Live demo: https://ofekfa.github.io/hi-cosmos/**

No server, no backend, no API keys — a single `index.html` with plain HTML, CSS and JavaScript.

## Features

- **N-body gravity simulation** — every body pulls on every other body; colliding bodies merge (momentum is conserved) with a burst of sparks.
- **Voice commands** — say "Hi Cosmos" followed by a command. Uses the browser's built-in Web Speech API and picks the best of several recognition guesses, so common mishearings still work.
- **Audio visualizer** — a ring of frequency bars reacts to your voice, and stars pulse with the sound.
- **Spoken replies** — Cosmos answers out loud (toggle with 🔊).
- **Auto camera** — the view follows and frames whatever you create; drag and zoom to explore on your own.

## Voice commands

| Say "Hi Cosmos…" | What happens |
| --- | --- |
| create the solar system | Sun with seven orbiting planets |
| create a galaxy | Black hole with two spiral arms of stars |
| big bang | Particles explode outward and clump into worlds |
| binary stars | Two stars orbiting each other, with planets |
| add 5 planets / add a star / add a black hole / launch a comet | Add bodies to the current scene |
| stop / start | Pause or resume |
| reverse time | Run the simulation backwards |
| faster / slower | Change simulation speed |
| more gravity / less gravity | Change the strength of gravity |
| trails on / trails off | Show or hide orbit trails |
| zoom in / zoom out / show everything | Control the camera |
| clear | Empty the universe |
| help | Show the command list |

You can also type any command in the box, or click it in the command list.

## Mouse, touch and keyboard

| Action | Effect |
| --- | --- |
| Click | Add a planet in orbit |
| Drag | Move the view |
| Scroll / pinch | Zoom |
| Shift + drag or right-drag | Throw a planet |
| `Space` | Pause / resume |
| `+` / `-` / `F` | Zoom in / zoom out / auto view |

## Browser support

Voice commands need **Chrome, Edge or Safari** (Firefox doesn't support speech recognition — typing commands still works there). The microphone requires HTTPS or `localhost`.

## Run locally

```bash
python3 -m http.server 8000
```

Then open http://localhost:8000. (Opening `index.html` directly from disk may block the microphone.)
