# Youtube Video Privacy Overlay
## ebrains-yt-video

Displays an overlay warning the user about Youtube/Google privacy if s.he loads/watches the video. Clicking on "watch video" button makes the embedded iframe created in the document

### Attributes

| name  | description                           | mandatory |
|-------|---------------------------------------|-----------|
| url   | "Embed" youtube video url             | x         |
| title | Video title                           |           |
| cover | URL to image used as background cover |           |

### Style

CSS custom properties

--ebrains-yt-video-overlay-fgcolor
    Overlay text color
--ebrains-yt-video-overlay-bgcolor
    Overlay background color: if opaque, the cover is not visible
--ebrains-yt-video-overlay-gradient-from
    Overlay background gradient start color: if opaque, the cover is not visible
--ebrains-yt-video-overlay-gradient-to
    Overlay background gradient to color: if opaque, the cover is not visible

| property                                 | description                                               | default                            |
|------------------------------------------|-----------------------------------------------------------|------------------------------------|
| --ebrains-yt-video-overlay-fgcolor       | Overlay text color                                        | #FFF                               |
| --ebrains-yt-video-overlay-bgcolor       | Overlay background color. If opaque, cover is not visible | rgba(0, 0, 0, .7)                  |
| --ebrains-yt-video-overlay-gradient-from | Overlay vertical gradient start color                     | --ebrains-yt-video-overlay-bgcolor |
| --ebrains-yt-video-overlay-gradient-to   | Overlay vertical gradient end color                       | --ebrains-yt-video-overlay-bgcolor |

Usage

Reference component

```
<script src="http://ebrains.bind.run/components/ebrains-yt-video.js"></script>
```

Use in HTML
			
```
<ebrains-yt-video
	url="https://www.youtube.com/embed/lyQfZZiBQVk?autoplay=1"
	cover="https://strapi-prod.sos-ch-dk-2.exo.io/ebrains_ssd_call_ebrains_website_3a68136980.jpg">
</ebrains-yt-video>
```
			
⚠️ You have to style ebrains-yt-video on your side. If you don't define css width and height properties, component should be not visible. 