# Bilal & Fatima — Shalima Invitation (Shalima-only variant)

Static site: open `index.html` in a browser, or deploy the folder to Vercel. Keep your existing `assets/hero.jpg` in `assets/`.

## Verified content (do not change)
- Couple: Bilal Aslam with Fatima Waheed
- Shalima: Sunday, 17 January 2027, 1:00 PM, Lubaba Marquee
- This variant is Shalima-only — no Mehndi anywhere.

## Where to edit
Everything configurable is in the `CONFIG` block at the top of `script.js`:
- `music`: path to a licensed audio file (e.g. `assets/music.mp3`). The music button stays hidden until this is set. Music starts when the guest taps "Open Invitation".
- `venues.*.location`: exact address or GPS pin (lat,lng) for each venue. Drives the embedded Google Map and the "Open in Google Maps" button. Currently set to the venue name only. Replace before sharing.
- `gallery`: add real photos. With a single image the arrows and dots hide automatically. Swipe and arrow keys work once you have 2+ images.
- `events`: calendar end times (11 PM and 5 PM) are estimates that only affect calendar entries.

## After deploying
In `index.html`, set `og:image` to the absolute image URL so WhatsApp and Facebook show a preview card.

## Behaviour notes
- Opening cover appears once per browser session (sessionStorage).
- Save the Date offers the Shalima Google Calendar link plus a Shalima .ics (Apple/Outlook).
- Countdown targets 17 Jan 2027 1:00 PM PKT, then switches to "The celebrations have begun", then to "Thank you for celebrating with us".
- All motion is disabled under `prefers-reduced-motion`.
- Tested at 320, 375, 390, 430px with no horizontal overflow.
