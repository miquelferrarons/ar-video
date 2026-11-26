# AR Video

Point a phone camera at the picture (`target.jpg`, the first frame of the video) and the video plays on top of it.

Runs in the browser on iPhone (Safari, Chrome) and Android (Chrome) using [MindAR](https://github.com/hiukim/mind-ar-js) image tracking and three.js. It must be served over HTTPS because it uses the camera.

- `index.html` – the page
- `targets.mind` – precompiled tracking data for `target.jpg`
- `video.mp4` – the demo video (480×272, 8 s, generated for this demo)
- `vendor/` – MindAR 1.2.5 and three.js 0.160

## Using your own video

Replace `video.mp4`, save its first frame as `target.jpg`, and recompile `targets.mind` from that picture with the [MindAR image target compiler](https://hiukim.github.io/mind-ar-js-doc/tools/compile).

## Choosing a picture that tracks well

The tracker needs a picture with crisp, distinctive detail: text, hard edges, varied shapes. Soft or repetitive imagery (foliage, grass, sky, blur) can make it lock on in the wrong place. If you change the files, bump the `?v=` number in `index.html` so phones do not reuse cached copies.

## Credits

Tracking by [MindAR](https://github.com/hiukim/mind-ar-js) (MIT), rendering by [three.js](https://threejs.org) (MIT). The demo clip is original to this repository.
