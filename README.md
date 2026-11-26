# AR Video

Point a phone camera at the picture (`target.jpg`, the first frame of the video) and the video plays on top of it.

Runs in the browser on iPhone (Safari, Chrome) and Android (Chrome) using [MindAR](https://github.com/hiukim/mind-ar-js) image tracking and three.js. It must be served over HTTPS because it uses the camera.

- `index.html` – the page
- `targets.mind` – precompiled tracking data for `target.jpg`
- `video.mp4` – the demo video (640×360, 10 s)
- `vendor/` – MindAR 1.2.5 and three.js 0.160

## Using your own video

Replace `video.mp4`, save its first frame as `target.jpg`, and recompile `targets.mind` from that picture with the [MindAR image target compiler](https://hiukim.github.io/mind-ar-js-doc/tools/compile).

## Credits

Demo video and picture: *Big Buck Bunny* © Blender Foundation, [peach.blender.org](https://peach.blender.org), licensed under [CC BY 3.0](https://creativecommons.org/licenses/by/3.0/).
