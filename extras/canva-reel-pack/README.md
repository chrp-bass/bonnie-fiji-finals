# Canva Reel Pack — Fiji

Every brand element from the v2 reel, sized for a 1080×1920 Canva reel page.

## Read this first

**The Fiji Reel could not be built inside Canva through the MCP.** All four reel
templates — `DAHRo7qMU_E`, `DAHRo9OPXZA`, `DAHRt9ooNk8` and the project's own
`DAHRqzpxkns` — return their single page as `(UNSUPPORTED)`. Canva's API exposes
no elements on video-format pages, so there is nothing to `replace_text` or
`update_fill` against. On top of that, the MCP cannot upload local media, so even
an editable page could not receive the Fiji photos.

The three templates were still read for their design language, and it is what the
finished reels follow: a solid color band carrying a small tracked eyebrow above
a large centered display title, sparkle ornaments above and below, and the photo
holding the rest of the frame.

So this pack is the Canva route: drag these onto a reel page instead of rebuilding
them there.

## What's here

| Folder | Use |
|---|---|
| `01-title-cards/` | Five finished full-frame cards. Drop one on a page as the whole frame — no editing needed. |
| `02-title-overlays/` | Transparent PNGs, one per spoken line, already positioned. Lay over a photo page at 100% size, 0,0. |
| `03-lower-thirds/` | The location/registration strips, emerald and ivory. Place at x=64, y=1320. |
| `04-brand-marks/` | Sparkle, VB monogram, wordmark, lockup, tagline, roundel — in ivory, emerald, sand and sage. |
| `05-frames/` | Scrims (soft and strong), the sand/ivory/emerald top band frame, and the corner monogram in position. |

Everything is 1080×1920 or a loose mark on transparency. Nothing needs resizing.

## Build order on a Canva reel page

1. Photo or video fills the page.
2. `05-frames/scrim-soft.png` (or `scrim-strong.png` over a bright shot) at 0,0.
3. The matching `02-title-overlays/` PNG at 0,0.
4. A `03-lower-thirds/` strip if the shot names a place or an aircraft.
5. `05-frames/corner-monogram-placed.png` at 0,0 — same position on every page.

Between sections, drop in the matching `01-title-cards/` frame as its own page.

## Animation, if you rebuild in Canva

The FFmpeg cuts animate titles by staggering each line up 40px over 0.26s, ~0.09s
apart. The nearest Canva equivalent is **Rise**, applied per text block, with the
delay stepped down the lines. Cards use the same Rise on the eyebrow, then the
title lines, then the sub.

For the section transitions, Canva's **Color wipe** in `#135443` or `#E1D9CC`
matches the graphic wipes. Do not use Dissolve — the wipes are doing brand work,
not just hiding a cut.

## Palette

`#135443` emerald · `#7A9E93` sage · `#C7D2D2` mist · `#B6A696` taupe ·
`#E1D9CC` sand · `#F7F5F2` ivory

## Type

Coconat for display, Baskervville for the one serif beat ("Dinner."), Mulish Bold
for on-screen titles, Mulish Medium for eyebrows and captions. All four are in
`reference/Vacations Booked/Type Suite & Font Files/` and need uploading to Canva
under Brand Kit → Fonts if they are not already there.
