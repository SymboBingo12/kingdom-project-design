# Motion

Calm, quick and purposeful. Motion explains what changed; it never decorates for its own sake.

| Use | Duration | Easing |
|---|---|---|
| Button press, switch, small change | 120–150 ms | `ease-out` |
| Card or panel appearing | 200–250 ms | `cubic-bezier(0.2, 0.9, 0.3, 1)` |
| Screen change | 250–300 ms | `cubic-bezier(0.2, 0.9, 0.3, 1)` |
| Pop-up message entering | 300–350 ms | `cubic-bezier(0.2, 0.9, 0.3, 1.2)` (a slight overshoot) |
| Stage warning flash | 0.7–1 s loop | `ease-in-out` |

## Rules

- Animate only `transform` and `opacity`, so motion stays smooth on older computers and tablets.
- Nothing flashes more than 3 times a second.
- Exits are faster than entrances.
- **Reduced motion:** when the system asks for less motion, replace movement with a simple fade, and replace
  flashing warnings with a steady colour plus text.

## Artwork motion

The artwork moves at four moments and stays still the rest of the time. Each moment has one job.

| Moment | Where | What the art does | Timing | Class |
|---|---|---|---|---|
| **Arrive** | A screen opens | Fades in and rises 8 px, once. Several pieces follow each other 30–80 ms apart | 300 ms, `--ease-out` | `st-arrive` |
| **Wait** | Connecting, loading | Two slow rings spread out from the art circle | 2.4 s loop | `st-wait` |
| **Celebrate** | Saved, finished | The sheet slides up, the art bounces once, small dots pop around it | 0.5 s, `--ease-pop` | `st-sheet` |
| **Rest** | Welcome and empty screens only | One layer moves very slowly, like light shifting on paper | 6–9 s, `ease-in-out`, back and forth | `st-rest` |

Each artwork has its own resting movement, set by a class on one layer in `brand/art.js`:

| Artwork | Resting movement |
|---|---|
| Platform | The light rings breathe |
| Clock | The outer rings breathe |
| Book | The two ribbons of light drift up and fade |
| Sound | The sound waves breathe out from the microphone |
| Street | The sun and its rings breathe |
| Hall | The tree sways |

**Keep it calm**
- Movement stays small: at most 4 % bigger, 1.2° of turn, 8 px of travel. If you notice it straight away, it's too much.
- Only one thing rests on a screen. A row of small discs never rests.
- No moving art on stage screens, on working screens (timer controls, counting) or behind text people are reading.
- Arrive plays when a screen opens, not on every tap or tab switch.

**Reduced motion:** arrive becomes a plain 200 ms fade, the waiting rings stop, celebrate appears without
bouncing, and resting art stands still.

See all four in [examples/motion/index.html](../examples/motion/index.html).

## Reduced motion for everything

```css
@media (prefers-reduced-motion: reduce) {
  *, *::before, *::after {
    animation-duration: 0.01ms !important;
    animation-iteration-count: 1 !important;
    transition-duration: 0.01ms !important;
  }
}
```
