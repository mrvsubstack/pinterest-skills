---
name: pinterest-content-planner
description: "Turns the content you already have (blog posts, products, videos, freebies) into a weekly Pinterest schedule: an inventory of what's pinnable, fresh-pin variations per link, board routing, a seasonal look-ahead and a realistic daily pin count. Use this skill whenever the user says things like \"Pinterest posting schedule\", \"plan my pins for the week\", \"how often should I pin\", \"turn my blog into Pinterest content\", \"Pinterest content calendar\", \"I don't know what to pin\", \"plan seasonal pins\". Not for writing pin copy (use pin-writer) or designing pins (use pin-design-brief)."
metadata:
  author: Mr V
  version: "1.0"
  group: Pinterest
---

# Pinterest Content Planner

You give it a list of what you've already made and how much time you have. It hands back a weekly pinning schedule: which link, which new pin angle, which board, which day, with seasonal content pulled forward in time.

---

## The core discovery: Pinterest runs on your back catalogue

On most platforms a post lives for a day. On Pinterest a good pin can bring visits for months, sometimes years, because people find it through search long after it went up.

That flips planning. You don't need new content every day. You need new **pins** pointing at content you already have. One strong blog post can carry five or six different pins over a few months, each with a fresh image and angle.

**Content-treadmill plan:** "Write a new post every day so I have something to pin."
**Back-catalogue plan:** "20 existing posts × 4 fresh pins each = 80 pins. That's months of pinning without writing a word."

---

## Intake

1. **Content inventory:** URLs or titles of blog posts, products, videos, freebies. Paste a list or a sitemap.
2. **Top performers**, if Pinterest or Google Analytics shows which pages get traffic.
3. **Keyword map and boards** (from `pinterest-seo` and `board-planner`), if available.
4. **Time per week** for making pins.
5. **Upcoming seasons, launches or events.**
6. **Region** (seasonality differs).

Default if no time is given: plan for 1 to 3 fresh pins a day, 5 days a week. Consistency beats bursts. Pinterest's own guidance has favoured steady, regular pinning of fresh content; check its current creator guidance if web search is available.

---

## Step 1: Inventory and score

For each piece of content, score 1 to 3 on:

| Factor | Question |
|---|---|
| Search fit | Does it match something people search on Pinterest? |
| Visual | Can it make a strong vertical image? |
| Evergreen | Will it still be useful in a year? |
| Business value | Does it lead to a sale, sign-up or key page? |

Total 10 to 12 = priority. 7 to 9 = regular rotation. Under 7 = skip or improve the content first.

---

## Step 2: Plan fresh pins per link

For each priority link, plan 3 to 6 distinct pins over time. Vary:
- **Angle:** different benefit, audience or problem ("for beginners", "under £20", "for small spaces").
- **Layout:** photo band, checklist, collage, before/after, video (from `pin-design-brief`).
- **Keyword:** a different related term from the keyword map.

Space pins for the same link several days apart and save them to different relevant boards.

---

## Step 3: Seasonal look-ahead

Pinterest users plan ahead of events, often well before the date. Check Pinterest Trends for when interest in each seasonal term starts climbing in the user's region, and schedule pins to go live before that rise.

| Season / event | Pin from (example, verify in Trends) |
|---|---|
| Christmas | Several weeks to a couple of months before |
| Back to school | Several weeks before term |
| Summer | Late spring |
| Valentine's | Early January |

Label the timing as verified in Trends, or as a general rule of thumb.

---

## Step 4: Build the week

Mix each week:
- **Priority evergreen links:** about 60% of pins
- **Seasonal content:** about 20%, rising as the season approaches
- **New content:** about 20%

---

## Rules

1. **Fresh pins, not re-uploads.** A new image or layout for each pin.
2. **First save to the most relevant board.** Later pins of the same link go to other relevant boards.
3. **Consistency beats volume.** 1 to 3 fresh pins a day you can sustain beats 25 in one evening, then nothing for a month.
4. **Every pin links somewhere useful.** No dead or broken links. Check the inventory URLs.
5. **Seasonal content goes up early.** Check Trends for the actual curve.
6. **Review monthly.** Look at Pinterest analytics: which pins get saves and outbound clicks? Make more pins for those links. Retire angles that get impressions but no clicks.
7. **Batch the work.** Make a week's pins in one session using templates.

---

## Worked example

**Input:** Home organisation blog. 30 posts. Top 5 by traffic known. 2 hours a week. It's late September. Boards already planned.

**Scored (excerpt):**
| Post | Search | Visual | Evergreen | Business | Total |
|---|---|---|---|---|---|
| Small pantry organisation ideas | 3 | 3 | 3 | 2 | 11 |
| Christmas wrapping station | 3 | 3 | 1 | 2 | 9 |
| My 2023 goals | 1 | 1 | 1 | 1 | 4 → skip |

**Week of [date]:**
| Day | Link | Pin angle | Layout | Board |
|---|---|---|---|---|
| Mon | Small pantry ideas | "Small Pantry Organisation Under £30" | Photo band | Pantry Organisation Ideas |
| Mon | Christmas wrapping station | "Wrapping Station in a Cupboard" | Before/after | Christmas Organisation |
| Tue | Decluttering checklist (freebie) | "Free Declutter Checklist" | Checklist | Decluttering Tips |
| Wed | Small pantry ideas | "Pantry Labels That Actually Stick" | Close-up | Kitchen Organisation |
| Thu | Under-bed storage | "Under-Bed Storage for Renters" | Collage | Small Bedroom Storage |
| Fri | Christmas wrapping station | "Gift Wrap Storage Ideas" | Video | Christmas Organisation |

Time check: 8 pins × ~15 minutes with templates ≈ 2 hours ✓

---

## Output format

```
## Pinterest plan: [account] — week of [date]
Capacity: [pins/day]   Season focus: [ ] (Trends checked: y/n)

### Priority links
| Link | Score | Pins planned | Angles used so far |

### This week
| Day | Link | Pin angle | Layout | Keyword | Board |

### Coming up
[seasonal content to prepare and when]

### Monthly review prompts
[what to check in analytics]
```

---

## Sibling skills

- `pin-writer`: copy for each scheduled pin.
- `pin-design-brief`: layouts and templates.
- `idea-pin-scripter`: video pins in the plan.
- `pinterest-seo`: keyword angles for each pin.
- `board-planner`: where each pin goes.

---

## Pre-flight checklist

- [ ] Content inventory scored.
- [ ] Each priority link has several distinct pin angles.
- [ ] Seasonal pins scheduled ahead, timing verified or labelled.
- [ ] Daily count matches the user's real time.
- [ ] Every pin has a board.
- [ ] Monthly review step included.
