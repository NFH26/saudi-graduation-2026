# Saudi Graduation Ceremony 2026, Brisbane

Live page for the Saudi Students Association in Brisbane graduation ceremony, Wednesday 25 November 2026, 1.00 pm Brisbane time (6.00 am Saudi time), UQ Centre (Building 27A), St Lucia.

Live at https://grad.nfh.sa

## Pages

- `index.html`: main page with countdown, Brisbane and Saudi times, calendar buttons, venue map, program, FAQ and live links.
- `frames.html`: photo frame tool (I'm attending, I'll watch live, I graduated, proud of you, Class of 2026).
- `event.ics`: calendar file in Brisbane time.
- `status-story.jpg`: ready-made status image with a QR code to the page.

## Adding the live links

Open `index.html` and find these lines near the top of the script:

```js
const PRIMARY = 'zoom';
const ZOOM_URL = ''; // Zoom Webinar join link for attendees
const YOUTUBE_ID = ''; // the part after watch?v= or /live/
```

- Paste the Zoom Webinar attendee link into `ZOOM_URL`.
- Paste the YouTube video ID into `YOUTUBE_ID` if there is a YouTube stream.
- To make YouTube the main link, change `PRIMARY` to `'youtube'`.

The live section appears at the top of the page 30 minutes before the start. After the ceremony, the YouTube recording plays there if `YOUTUBE_ID` is set.

## Hosting

GitHub Pages from the `main` branch, custom domain `grad.nfh.sa` (see `CNAME`).
