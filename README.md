# Kingdom Project Design

One look for the apps and tools we build for Kingdom work: meetings, the ministry, Kingdom Hall care,
personal study, sound and video.

Calm pages, plenty of white space, original artwork, and colours that stay easy on the eyes in light and dark.
Working name: **Steward**.

## See it

Online: **https://symbobingo12.github.io/kingdom-project-design/**

Or open these in a browser:

- [brand/index.html](brand/index.html): the brand guide
- [brand/desktop.html](brand/desktop.html): desktop screens
- [brand/slides.html](brand/slides.html): a 5-slide overview
- [examples/components/index.html](examples/components/index.html): every component, light and dark
- [examples/motion/index.html](examples/motion/index.html): how the artwork moves

## Use it

1. Link [tokens/tokens.css](tokens/tokens.css), then [components/index.css](components/index.css).
2. Build with the `st-` components. See [components/](components/) for the list.
3. Follow [guidelines/](guidelines/): principles, accessibility, wording, and what we never copy.

## What's inside

| Folder | What it holds |
|---|---|
| `brand/` | The brand pages and the original artwork |
| `tokens/` | Colours, fonts, sizes and spacing, light and dark |
| `guidelines/` | The rules every app follows |
| `components/` | Buttons, cards, lists, switches, banners, the stage display and more |
| `motion/` | Animation timing, artwork motion and the reduced-motion rule |
| `examples/` | Real screens built with the system |

## Help with it

Changes go through a pull request, so we can look at them together before they reach `main`.

1. Make a branch for your change: `git checkout -b short-name`.
2. Check it in a browser: light, dark (add `?theme=dark` to the page address) and phone width.
3. Push the branch and open a pull request. Say what changed and why; a screenshot helps.

A few rules keep the design ours and keep it consistent:

- **Original art only.** Never use JW.ORG or JW Library logos, names, fonts or artwork.
- **Screenshots of other apps stay on your computer.** Put them in `reference/`, which is never pushed.
- **Colours and sizes come from `tokens/tokens.css`.** Add a token there rather than a new colour in a component.
- **Motion follows [motion/motion.md](motion/motion.md),** and every animation respects reduced motion.

## Status

Draft. The colours will be fine-tuned before version 1.

## Independent

This project is not affiliated with, endorsed by, or connected to Jehovah's Witnesses, JW.ORG, JW Library or the
Watch Tower Bible and Tract Society. No logos, icons, names or font files of theirs are used. All artwork is original.
See [guidelines/brand-boundaries.md](guidelines/brand-boundaries.md).

## Licence

MIT © 2026 SymboBingo12. Designed and created by SymboBingo12.
