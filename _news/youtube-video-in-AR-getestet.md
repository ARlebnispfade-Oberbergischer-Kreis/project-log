---
layout: simple
title: Versuch, Youtube in ARjs zu präsentieren
subtitle: 12.10.2023
---
Um eventuell bereits bestehende Videos zu AR-Spots in der Augmnented Reality zu präenstieren, wurden verschiede Möglichkeiten getestet, das [CORS](https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS) Problem zu lösen.

```html
<video id="video" preload="auto" src="https://youtu.be/uDjJPtmBcmY?si=FpyMBX274-DAx30c" width="160" height="90" autoplay loop="true" crossOrigin="anonymous" muted>></video>

<video crossOrigin="anonymous" id="video1" controls src="https://www.youtube.com/embed/uDjJPtmBcmY?si=japZwtlh16alDnu_" loop></video>

<video crossOrigin="anonymous" id="video2" controls src="https://www.youtube.com/watch?v=uDjJPtmBcmY" loop></video>

<video id="videoCORS" preload="auto" src="https://youtu.be/uDjJPtmBcmY?si=FpyMBX274-DAx30c&origin=https://www.arlebnisobk.de/" width="160" height="90" autoplay loop="true" crossOrigin="anonymous" muted>></video>

<video crossOrigin="anonymous" id="video1CORS" controls src="https://www.youtube.com/embed/uDjJPtmBcmY?si=japZwtlh16alDnu_&origin=https://www.arlebnisobk.de/" loop></video>

<video crossOrigin="anonymous" id="video2CORS" controls src="https://www.youtube.com/watch?v=uDjJPtmBcmY&origin=https://www.arlebnisobk.de/" loop></video>
```

Leider war keiner der Versuche erfolgreich, daher wurde, falls ein Youtube-Video verwendet werden soll, dieses in der Card eingebunden:

```html
<iframe id="iframeVideo" src="https://www.youtube.com/embed/uDjJPtmBcmY?si=japZwtlh16alDnu_" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
```