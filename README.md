# Hand Gesture to Emoji

A hand-gesture image classifier that maps predicted labels to emoji.

**Repository created:** 2022-02-20  
**Project status:** Learning project / historical snapshot  
**Earliest recorded commit (author date):** 2022-02-20

## Features and implementation

- Webcam snapshot capture.
- Teachable Machine model.
- Top-two prediction labels.
- Conditional emoji mappings.
- Speech synthesis helper.

## Technologies

HTML, CSS, JavaScript, Bootstrap, jQuery, ml5.js, WebcamJS, Teachable Machine (hosted model).

## How the code works

`take_snapshot()` captures the camera image; `check()` submits it for classification; `gotResults()` maps the predicted labels to emoji.

## Project structure

| File | Purpose |
| --- | --- |
| [`index.html`](index.html) | Main page and user interface |
| [`main.js`](main.js) | Project-specific JavaScript |
| [`style.css`](style.css) | Page styling |

Key functions in the source:
- `main.js`: `take_snapshot()`, `speak()`, `check()`, `gotResults()`.

## Run or explore locally

```bash
git clone https://github.com/Avenger-Sonic123/Hand-gesture-done.git
cd Hand-gesture-done
python -m http.server 8000
```

Open [http://localhost:8000](http://localhost:8000) in your browser. The local server requires Python 3; browser-based dependencies may also require internet access.

Allow camera access, show a hand gesture, capture an image and request identification.

## Current status and limitations

Model availability is external; speech output may be empty because prediction variables are not populated in the result handler.

## Related project snapshots

Other repositories in this project family:
- [Hand-gesture-almost-done](https://github.com/Avenger-Sonic123/Hand-gesture-almost-done) — repository created 2022-02-20
- [Hand-gesture_Not_done](https://github.com/Avenger-Sonic123/Hand-gesture_Not_done) — repository created 2022-02-20
- [Hand-gesture_done](https://github.com/Avenger-Sonic123/Hand-gesture_done) — repository created 2022-02-24

---

Source reference: [`5e4e8473`](https://github.com/Avenger-Sonic123/Hand-gesture-done/tree/5e4e8473fb97057e547eb76076d9242adf8294b1) on `main`, verified against GitHub on 2026-11-24. Documentation is based on static source review; runtime behavior has not been tested.
