# Petaluma Swim Center schedule — Pool Relay embed preview

An unofficial replica of the City of Petaluma **Swim Center Updates & Schedule** page with a
live [Pool Relay](https://www.poolrelay.com) calendar in place of the typed schedule, its
footnotes, and the schedule poster.

**This is not a City of Petaluma website.** The official page is
<https://cityofpetaluma.org/swim-center-updates/>. This is a working preview of one proposed
change to it, and the page says so in a ribbon across the top.

## What it replaces

The live page publishes the same schedule **twice** — as typed hours with footnotes, and as
a poster image whose filename is `psc-schedule-new-8.25.26.png`, the day it was last
redrawn. Both have to be edited together, and can disagree in between.

And the footnotes are really dates:

- `**4:15pm - 7pm (Long Course, beginning 9/4, NO LCM 9/11 & 9/18)`
- `**6:30am - 10am (Long Course, beginning 9/5, NO LCM 9/12 & 9/19)`
- `*12pm - 4pm (closing at 1pm beginning 9/12. closing at 12pm beginning 10/10)`
- `12pm - 4pm (through 9/6 only, closed on Sundays as of 9/13)`

Each is a date on which the schedule stops being what the paragraph above it says. A
calendar has dates in it already, so those are simply what the week shows — look at Friday
and Saturday of the current week in the embed.

The page also asks readers to *"sign up for our email updates to receive monthly lane
availability updates"*. The calendar is the update.

## Fidelity

Checked against the city's published schedule before building: the modelled week matches,
including the swim-team lane split (8 × 25 yd plus 3 × 20 yd, Monday–Thursday 4:15pm) and
both September closures — Labor Day, and the private swim-team event on Saturday 9–11am.

A **Week** view rather than a lane-by-lane Day view, because this pool changes shape
mid-week: Long Course on Friday evenings and Saturday mornings, Short Course otherwise. A
Day view has to pick one configuration; the week shows every booking with its lane count,
which is what the page's *"minimum of 6 lanes available"* promise is about.

```html
<iframe src="https://www.poolrelay.com/embed/wYsFZYXYvYNpNxXSPbMecE"
        width="100%" height="800" style="border:0"
        title="Petaluma Swim Center schedule"></iframe>
```

## Notes

- The poster is hotlinked from the city's own storage so the comparison stays honest.
- The Petaluma wordmark is a CSS approximation, not the city's artwork.
- Navigation links point at the live site. `noindex` is set.

## Local preview

```
python3 -m http.server 8808
```
