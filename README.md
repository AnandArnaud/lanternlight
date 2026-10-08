# lanternlight

Lanternlight is a tiny reading/blog site — open a post, subscribe, get in touch.

**Stack:** Plain HTML / CSS / JS (no build step)

It is intentionally small.

## Key user actions

open post · subscribe · contact

## Running it

```bash
# static site — no build
python3 -m http.server 8000   # then open http://localhost:8000
```

## Recordings and heatmaps

Hotjar is loaded in `index.html` (recordings, heatmaps, feedback). The newsletter email field and the whole contact form are suppressed from recordings with `data-hj-suppress`; `app.js` sends `post_opened`, `newsletter_subscribed` and `contact_submitted` as Hotjar events and a `stateChange` per post. The site id is set at the top of `app.js`.
