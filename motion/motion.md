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

```css
@media (prefers-reduced-motion: reduce) {
  *, *::before, *::after {
    animation-duration: 0.01ms !important;
    animation-iteration-count: 1 !important;
    transition-duration: 0.01ms !important;
  }
}
```
