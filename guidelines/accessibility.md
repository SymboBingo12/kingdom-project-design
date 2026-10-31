# Accessibility checklist

Check every screen before release. These rules are never broken, not even for looks.

## Seeing

- [ ] Body text is at least 16 px; nothing a user must read is under 12 px
- [ ] Text contrast is at least 4.5 : 1 (7 : 1 for anything on a stage screen)
- [ ] The app still works when the text size is set to 200 %
- [ ] Both light and dark themes pass these checks

## Colour blindness

- [ ] Colour is never the only signal: warnings also flash, change wording, or show an icon
- [ ] Amber and red warnings are also different in brightness, not only in hue

## Hands and touch

- [ ] Every tap target is at least 44 × 44 px (48 px for main actions)
- [ ] At least 8 px between tap targets
- [ ] Nothing important needs a long press, a swipe or a double tap

## Motion

- [ ] Every animation respects the system "reduce motion" setting (see `motion/`)
- [ ] Nothing flashes more than 3 times a second

## Keyboard and screen readers

- [ ] Everything can be reached and used with the keyboard, with a visible focus ring
- [ ] Buttons and switches have clear labels for screen readers
- [ ] Pages have a real title and a logical heading order

## Language

- [ ] Plain words, short sentences (see `voice.md`)
- [ ] Error messages say what happened and what to do next
