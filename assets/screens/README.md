# Screenshots

All twelve slots are filled. They were captured on an **iPhone 17 Pro simulator**
(1206×2622), downscaled to 1800px tall and saved as JPEG.

The page checks whether each image actually loaded — if a file is missing or renamed,
a dashed placeholder with the expected filename appears in its place. So to swap one,
just overwrite the file with the same name. No HTML change needed.

| File | Where it appears | What it shows |
| --- | --- | --- |
| `hero-1.jpg` | Hero, left phone (tilted) | The animated cover, caught as it starts to open |
| `hero-2.jpg` | Hero, centre phone | The diary with entries and photo thumbnails |
| `hero-3.jpg` | Hero, right phone (tilted) | Mood Insights, 30D — metrics and trend |
| `step-1.jpg` | How it works, step 1 | Diary Style → Cover, with the Pro badges |
| `step-2.jpg` | How it works, step 2 | New mood note, filled in |
| `step-3.jpg` | How it works, step 3 | Mood Insights, 7D |
| `gallery-1.jpg` | Screens, 1 | The diary list, scrolled |
| `gallery-2.jpg` | Screens, 2 | A finished entry page with a photo |
| `gallery-3.jpg` | Screens, 3 | Calendar with the day's agenda: an entry and a reminder |
| `gallery-4.jpg` | Screens, 4 | Mood mix — the donut and the distribution |
| `gallery-5.jpg` | Screens, 5 | Cover objects (ornaments), all Pro-badged |
| `gallery-6.jpg` | Screens, 6 | Settings in dark mode |

The diary content in these shots is fictional, written in English for the site.

Still missing, and not a placeholder: **`../og.jpg`** — a 1200×630 image used as the link
preview on WhatsApp, iMessage, X and LinkedIn. Until it exists, shared links show no image.

## If you re-shoot

- **JPEG**, portrait, straight from an iPhone simulator or device.
- The page draws its own iPhone bezel — send the **raw screen capture**, not one already
  placed inside a device mockup. It does *not* draw a Dynamic Island over a real capture,
  because the capture already contains one.
- **Keep the 1206×2622 ratio.** The screen inside the frame is set to exactly that, and the
  image is fitted with `object-fit: contain`, so a whole app screen shows with nothing cropped.
  A capture from a different device will letterbox instead of filling the frame — if you move
  to another iPhone, update `aspect-ratio` on `.phone .screen` in `styles.css` to match.
- Fill the app with believable content first. Empty states look like a broken app in a
  screenshot, and identical entries look fake.
- Keep each file under ~600 KB; run them through ImageOptim or TinyPNG before committing.
- The status-bar clock differs between these shots. Apple cares about that for App Store
  screenshots; for a website it just reads as real. Worth aligning if you re-shoot in one pass.
