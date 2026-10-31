# Components

Shared building blocks, made only from `tokens/tokens.css`. See them all, in light and dark, in
[examples/components/index.html](../examples/components/index.html).

## Use them

```html
<link rel="stylesheet" href="tokens/tokens.css">
<link rel="stylesheet" href="components/index.css">   <!-- or only the files you need, after base.css -->
<body class="st-page">
```

Every class starts with `st-`, so the components won't clash with an app's own CSS.

| File | What it gives you |
|---|---|
| `base.css` | Page font and colours (`st-page`), focus ring, steady numbers (`st-num`), screen-reader text (`st-sr`), reduced motion |
| `button.css` | `st-btn` with `--primary`, `--secondary`, `--soft`, `--quiet`, `--danger`; sizes `--main`, `--block`, `--round` |
| `card.css` | `st-card`, `--raised`, a title, a hint and an optional artwork strip |
| `list.css` | `st-list` and `st-row`: meeting parts, people, settings. Current row: `aria-current="step"`. Finished: `.is-done` plus a tick |
| `switch.css` | `st-switch` (`role="switch"`) and the `st-option` setting row |
| `segmented.css` | `st-seg`: pick one of 2–4 views |
| `pill.css` | `st-pill` status labels: `--ok`, `--warn`, `--danger`, `--brand` |
| `banner.css` | `st-banner` notices and problems, always with an icon |
| `progress.css` | `st-progress`, set with `--value` from 0 to 1 |
| `topbar.css` | `st-topbar`: app name, subtitle, status and time |
| `stage.css` | `st-stage`: the big countdown, with `data-state` = `run`, `warn`, `over` or `between` |

## Rules built in

- Tap targets are at least 44 px; main actions 56 px.
- State never depends on colour alone: ticks, icons, words and position carry it too.
- Small coloured text uses the `--ok-text`, `--warn-text` and `--danger-text` tokens, which pass 4.5 : 1.
- The stage display is always dark, reaches 7 : 1, and never uses coral.
- Motion uses `transform` and `opacity` only and stops when the system asks for reduced motion.
