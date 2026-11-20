# Own Your AI — website

Static site for [Own Your AI](https://github.com/Own-Your-AI/events), an engineering
group in Vienna for sovereign, efficient AI.

**One file. No build step. No external requests.**

`index.html` is the entire site — no fonts, images, scripts, trackers or analytics are
fetched from anywhere. It renders identically from a CDN, a GitHub Pages branch, an
Nginx box in Vienna, or a USB stick with no network at all.

## Deploy

**Cloudflare Pages** — connect this repo, no build command, output directory `/`.

**GitHub Pages** — Settings → Pages → deploy from `main` / root.

**Anything else** — copy `index.html` to the web root. That's the whole deployment.

## Design

Colours are taken from the group's logo, which contains zero saturated pixels: the
palette runs `#060606` to `#F0F0F0` and nothing else. Depth comes from translucency
(`backdrop-filter` desaturated to zero) rather than colour. The corner crop marks on
the cards are the logo's own motif.

| Token | Value |
| :--- | :--- |
| `--bg` | `#080808` |
| `--surface` | `#101010` |
| `--raised` | `#181818` |
| `--fg` | `#F0F0F0` |
| `--fg-muted` | `#A0A0A0` |
| `--fg-dim` | `#6E6E6E` |
| `--hairline` | `rgba(255,255,255,.09)` |
| `--glass` | `rgba(255,255,255,.045)` |

## Content

Event and speaker data is hardcoded from the
[events repository](https://github.com/Own-Your-AI/events). Slide links point back at
that repo, which stays the source of truth — this site never hosts a copy of anyone's deck.

## Status

Unofficial. Built as a contribution to the group, not published on its behalf.

## Links

- Events — [luma.com/ownyourai](https://luma.com/ownyourai)
- Discord — [discord.gg/J2XzvVND66](https://discord.gg/J2XzvVND66)
- Archive — [github.com/Own-Your-AI/events](https://github.com/Own-Your-AI/events)
