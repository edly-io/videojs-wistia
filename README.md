# Wistia playback technology for [Video.js](https://github.com/videojs/video.js)

## Install
You can use npm (`npm install videojs-wistia-tech`) or the source and build it using `npm run-script build`

## Example
```html
<!DOCTYPE html>
<html>
<head>
  <link type="text/css" rel="stylesheet" href="https://vjs.zencdn.net/7.11.4/video-js.css" />
</head>
<body>
  <video
    class="video-js vjs-default-skin vjs-big-play-centered"
    controls
    width="640" height="360"
    data-setup='{ "techOrder": ["Wistia"], "sources": [{ "type": "video/wistia", "src": "29b0fbf547"}], "wistia": { "playback_css_class": "wistia_embed wistia_async_29b0fbf547", "autoplay": true } }'
  >
  </video>

  <script src="https://vjs.zencdn.net/7.11.4/video.min.js"></script>
  <script src="dist/Wistia.min.js"></script>
</body>
</html>
```

Don't forget to set `playback_css_class` attribute it should be combinition of two css classes `wistia_embed` and `wistia_async_{videoid}`.