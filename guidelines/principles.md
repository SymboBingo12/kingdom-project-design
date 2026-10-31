# Design principles

Our users range from young brothers running OBS to older publishers holding a tablet with shaky hands. Design for the
hardest case first.

## The UX laws we follow

| Law | What it means for us |
|---|---|
| **Jakob's Law**: people prefer apps that work like apps they know | Follow the patterns JW Library users already know (see `brand-boundaries.md` for the limits) |
| **Fitts's Law**: big, close targets are faster and easier to hit | Main buttons at least 48 px tall; the most-used button is the biggest |
| **Hick's Law**: more choices, slower decisions | Few choices per screen; rare settings go behind an "Advanced" section |
| **Miller's Law**: people hold only a few things in mind | Group items in short lists with clear headings |
| **Doherty Threshold**: answers under 0.4 s feel instant | Every tap shows a response immediately, even while work continues |
| **Aesthetic-Usability Effect**: beautiful things feel easier to use | Polish matters: spacing, alignment and calm colours are not optional |
| **Law of Common Region**: things inside one box belong together | Use cards to group related controls |

## When we break a rule for looks

Breaking a rule for the sake of beauty is allowed on **decorative** things, such as a header, an empty screen or a
transition, as long as we write down why.

It is **never** allowed on:

- anything the speaker sees on stage
- warnings and alerts
- the main action on a screen (Start, Stop, Save)
- anything in `accessibility.md`

## Tone of the design

Calm, clean and respectful. Lots of white space, one brand colour, no clutter, no loud gradients.
