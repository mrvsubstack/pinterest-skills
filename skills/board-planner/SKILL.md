---
name: board-planner
description: "Designs a Pinterest board structure that ranks in search and organises your niche: 8 to 15 keyword-named boards built from what people search, a description for each, section plans, board order on the profile, which existing boards to merge, rename or archive, and where every new pin belongs. Use this skill whenever the user says things like \"plan my Pinterest boards\", \"what boards should I create\", \"organise my Pinterest\", \"rename my boards for SEO\", \"Pinterest board names\", \"set up a new Pinterest account for my business\", \"my boards are a mess\". Not for keyword research from scratch (use pinterest-seo) or writing individual pins (use pin-writer)."
metadata:
  author: Mr V
  version: "1.0"
  group: Pinterest
---

# Board Planner

You give it your niche, what you sell or publish, and your current boards if you have any. It hands back a board map: names, descriptions, sections, profile order, a cleanup list and a rule for where each future pin goes.

---

## The core discovery: boards are the table of contents Pinterest reads

Pinterest uses boards to understand what a pin is about and what your account is an authority on. A pin saved to "Easy Vegan Dinners" gets context. A pin saved to "Yummy!!" gets none.

Boards also tell a visitor in two seconds whether to follow you. A profile with 40 vague boards looks like a junk drawer. A profile with 12 sharply named ones looks like an expert.

**Junk drawer:** "Stuff I Love", "Ideas", "Yum", "Home", "Misc 2", "Christmas!!!"
**Table of contents:** "Small Living Room Ideas", "Budget Home Decor", "Rental-Friendly Upgrades", "Cozy Bedroom Decor", "Christmas Decor Ideas"

Every board name is a search phrase. Every board is a promise of what's inside.

---

## Intake

1. **Niche** and what you're promoting (blog, shop, service, newsletter).
2. **Audience** and what they search for.
3. **Keyword map** from `pinterest-seo`, if you have one. If not, this skill builds a light one from Pinterest autocomplete and labels it as such.
4. **Current boards:** names, rough pin counts and which drive traffic (Pinterest analytics, if available).
5. **Content library:** what you've already made that can be pinned.
6. **Business or personal account.**

---

## Board architecture

| Board type | Share of boards | Purpose | Example |
|---|---|---|---|
| Core boards | 50–60% | Your main topics, each a middle keyword | "Easy Weeknight Dinners" |
| Supporting boards | 20–30% | Adjacent topics your audience also searches | "Kitchen Organisation Ideas" |
| Seasonal boards | 10–20% | Events and seasons, brought forward when relevant | "Christmas Dinner Recipes" |
| Brand board | 1 | Only your own content, for a clear home base | "[Brand] Recipes" |

Start with 8 to 15 boards. Enough to show range, few enough to fill properly. A board with 3 pins looks abandoned. Aim for a healthy number of relevant pins before showing it near the top.

---

## Rules

1. **Name boards the way people search.**
   - Bad → "Food Glorious Food"
   - Good → "Healthy Lunch Ideas for Work"
2. **One topic per board.** If a board needs "and" in its name, it's probably two boards.
   - Bad → "Recipes and Home and Garden"
   - Good → "Easy Dinner Recipes" + "Small Garden Ideas"
3. **Descriptions in 2 to 3 natural sentences** using related keywords. Say who it's for and what they'll find.
4. **Sections for depth, not a substitute for boards.** Use sections inside a broad board ("Easy Dinner Recipes" → "Chicken", "Vegetarian", "One-Pan") when the subtopics are too small for their own board.
5. **Your best boards go first on the profile.** Lead with the boards most connected to what you sell or publish.
6. **Seasonal boards rotate.** Move them up the profile ahead of the season. Pinterest users plan early, so check Pinterest Trends for when interest starts rising.
7. **Clean up before you build.** Rename vague boards (keeps their pins and followers), merge thin duplicates, make irrelevant ones secret or archive them.
8. **Covers matter.** Pick a clear, on-brand cover pin per board so the profile looks intentional.
9. **Don't promise what you won't fill.** Only create a board you can add relevant pins to regularly.

---

## Steps

1. **Collect keywords.** Use the keyword map or gather autocomplete suggestions for 3 to 5 seed terms.
2. **Cluster.** Group keywords into topics. Each cluster with enough content becomes a board candidate.
3. **Assign board types** (core, supporting, seasonal, brand).
4. **Name each board** with its strongest middle keyword.
5. **Write descriptions** and plan sections.
6. **Audit current boards:** keep, rename, merge, make secret or archive.
7. **Order the profile.**
8. **Write the pin routing rule:** for each content type, which board gets the first save and which other boards are relevant.

---

## Worked example

**Input:** Interior design blogger, rentals and small spaces, UK. Current boards: "Home Inspo" (340 pins), "Ideas" (90), "Living room" (60), "Xmas" (25), "Recipes" (40).

**Cleanup:**
| Current | Action | New name |
|---|---|---|
| Home Inspo | Rename + split | "Small Living Room Ideas" (living room pins move here) and "Rental-Friendly Home Decor" |
| Ideas | Sort into new boards, then archive | — |
| Living room | Merge into "Small Living Room Ideas" | — |
| Xmas | Rename | "Christmas Decor for Small Spaces" |
| Recipes | Make secret (off-niche) | — |

**New board map (excerpt):**
| Order | Board | Type | Sections | Description |
|---|---|---|---|---|
| 1 | Rental-Friendly Home Decor | Core | Walls, Lighting, Storage | Renter-friendly decor ideas that won't cost your deposit. Peel-and-stick, freestanding storage and lighting you can take with you. |
| 2 | Small Living Room Ideas | Core | Layouts, Cosy, Budget | Small living room ideas to make a tiny lounge feel bigger, cosier and more organised. |
| 3 | Small Bedroom Ideas | Core | — | |
| 4 | Studio Flat Layouts | Supporting | — | |
| 5 | [Blog name] Home Tours | Brand | — | |
| (Oct–Dec) | Christmas Decor for Small Spaces | Seasonal | — | |

**Routing rule:** a new rental decor blog post → first save to "Rental-Friendly Home Decor", later saves to the most specific matching core board.

---

## Output format

```
## Board plan: [account]

### Cleanup
| Current board | Action | New name / destination |

### Board map
| Order | Board name | Type | Sections | Description |

### Pin routing rules
[content type] → first board → other relevant boards

### Seasonal rotation
[board] → move up by [month] (Trends checked: yes/no)
```

---

## Sibling skills

- `pinterest-seo`: the keyword research behind the board names.
- `pin-writer`: copy for the pins that fill each board.
- `pin-design-brief`: on-brand covers and pin images.
- `pinterest-content-planner`: the weekly schedule that keeps boards filled.

---

## Pre-flight checklist

- [ ] Every board name is a real search phrase.
- [ ] One topic per board.
- [ ] Descriptions written for every board.
- [ ] 8 to 15 boards, each fillable.
- [ ] Existing boards audited with a clear action each.
- [ ] Profile order leads with what drives the business.
- [ ] Pin routing rules written.
