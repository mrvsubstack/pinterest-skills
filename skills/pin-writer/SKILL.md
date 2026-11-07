---
name: pin-writer
description: "Writes Pinterest pin titles, descriptions, image overlay text and alt text that get found in search and earn the click to your site. Builds each pin around one keyword, front-loads it, writes descriptions as readable sentences with a reason to click, and gives 3 to 5 fresh variations of the same link so you can pin it again with new copy. Use this skill whenever the user says things like \"write pin descriptions\", \"Pinterest titles for my blog post\", \"pin copy for my product\", \"make 5 pins for this link\", \"what should my pin say\", \"text overlay for my pin\". Not for keyword research (use pinterest-seo) or the visual layout (use pin-design-brief)."
metadata:
  author: Mr V
  version: "1.0"
  group: Pinterest
---

# Pin Writer

You give it the page you're sending people to and the keyword you're targeting. It hands back finished pin copy: title, description, overlay text and alt text, plus fresh variations so one link can become several pins.

---

## The core discovery: a pin has two readers

Every pin is read twice. First by Pinterest, which decides what searches it should appear in. Then by a person, who decides in a second whether to save it or tap through.

Most pin copy serves only one. Keyword piles please nobody. Pretty copy with no keyword never gets shown.

**For the machine only:** "Easy dinner recipes | quick dinner | family dinner ideas | dinner recipes easy"
**For the person only:** "This changed our Tuesday nights forever! 💛"
**For both:** "Easy 20-Minute Dinner Recipes for Busy Weeknights. Six one-pan meals the whole family will eat, with a free printable shopping list."

The third has the keyword up front and a reason to tap at the end.

---

## Intake

1. **The destination:** blog post, product page, freebie, course. Paste the URL and the page's main points, or the text itself.
2. **The main keyword** (from `pinterest-seo` if available). If none, suggest 3 from the content and label them as unverified until checked in Pinterest search.
3. **2 to 3 related keywords.**
4. **Audience** and what they're trying to do.
5. **What's on the page that makes the tap worth it:** a printable, a full recipe, a checklist, a price.
6. **How many variations** (default 3).

Verify current Pinterest character limits when web search is available. At the time of writing: titles up to 100 characters, descriptions up to 500, with only the first part of a description showing in most views.

---

## The four parts of a pin

| Part | Job | Length guide |
|---|---|---|
| Title | Rank + promise | Keyword in the first ~40 characters. Under 100. |
| Description | Context + more keywords + reason to click | 2–3 sentences. Key point in the first ~50 characters. |
| Overlay text | Stop the scroll on the image | 3–8 words. Keyword or its promise. |
| Alt text | Describe the image for accessibility and search | One plain sentence. |

---

## Title formulas

| Code | Formula | Example |
|---|---|---|
| P1 | Keyword + benefit | "Small Bathroom Ideas That Make It Feel Twice the Size" |
| P2 | Number + keyword | "15 Cheap Family Meals Under £10" |
| P3 | How to + keyword + qualifier | "How to Start a Bullet Journal (Even If You Can't Draw)" |
| P4 | Keyword + for + audience | "Capsule Wardrobe for Women Over 40" |
| P5 | Keyword + free resource | "Weekly Meal Planner Printable (Free PDF)" |
| P6 | Problem + keyword fix | "Messy Entryway? 9 Small Entryway Storage Ideas" |

---

## Rules

1. **Keyword first in the title.**
   - Bad → "You'll Love These Amazing Ideas for Your Small Bathroom"
   - Good → "Small Bathroom Ideas: 12 Tricks That Add Space"
2. **One main keyword per pin.** Related terms go in the description.
3. **Descriptions are sentences a person would write.** No hashtag tails, no keyword lists.
4. **Give the reason to tap.** Name what's on the page: the full list, the free printable, the step-by-step, the price.
   - Bad → "Check it out!"
   - Good → "Get the full shopping list and prep schedule on the blog."
5. **Match the page.** The pin promises what the page delivers. A pin that misleads gets saved less, clicked less and can hurt how Pinterest treats your account.
6. **Overlay text ≠ title.** The overlay is the hook, the title is the searchable label. They agree but don't repeat word for word.
7. **Every variation is genuinely different.** New angle, new formula, new overlay. Pinterest favours fresh pins over the same image re-uploaded.
8. **No unverifiable claims.** "Lose 10 lbs in a week" or "guaranteed" claims break Pinterest's policies and your credibility.

---

## Steps

1. Intake. Confirm the main keyword.
2. Pick 3 to 5 title formulas that suit the content.
3. Write one full pin per formula: title, description, overlay, alt text.
4. Check each against the rules and character limits.
5. Suggest which variation to pin first (usually the clearest keyword match) and spacing between the rest (a few days to a week apart, to different relevant boards).

---

## Worked example

**Input:** Blog post "6 one-pan dinners for busy weeknights", free printable shopping list. Keyword: "easy weeknight dinners". Related: "one pan meals", "family dinner ideas". Audience: working parents.

**Pin 1 (P2)**
- Title: Easy Weeknight Dinners: 6 One-Pan Meals in 30 Minutes
- Description: Easy weeknight dinners for busy families, all cooked in one pan with less washing up. Includes a free printable shopping list so you can shop once for the whole week.
- Overlay: 6 One-Pan Dinners · 30 Minutes
- Alt text: Overhead shot of a sheet pan with roasted chicken thighs, peppers and potatoes.

**Pin 2 (P4)**
- Title: Easy Weeknight Dinners for Working Parents
- Description: Six family dinner ideas that are on the table in half an hour. One pan each, kid-tested, with a free shopping list on the blog.
- Overlay: Dinner Sorted by 6:30
- Alt text: A family table with a one-pan pasta bake and four plates.

**Pin 3 (P5)**
- Title: One Pan Meals + Free Weekly Shopping List Printable
- Description: Plan a week of one pan meals in five minutes. Grab the free printable shopping list and six easy weeknight dinners to go with it.
- Overlay: Free Shopping List Inside
- Alt text: A printed shopping list on a kitchen counter next to fresh vegetables.

Pin first: Pin 1. Then Pin 2 four days later, Pin 3 the following week.

---

## Output format

```
## Pins for: [page title]
Main keyword: [ ]   Related: [ ]

### Pin 1 — [formula]
Title: [ ] ([n] chars)
Description: [ ] ([n] chars)
Overlay: [ ]
Alt text: [ ]
Suggested board: [ ]

### Pin 2 ...

Posting order: [ ]
```

---

## Sibling skills

- `pinterest-postiz-publisher` — schedule the finished post through Postiz after you approve it.
- `pinterest-seo`: find the keyword before writing.
- `pin-design-brief`: lay out the image the overlay sits on.
- `board-planner`: decide which board each pin goes to.
- `idea-pin-scripter`: when the pin is a video or multi-page pin.
- `pinterest-content-planner`: schedule the variations.

---

## Pre-flight checklist

- [ ] Keyword in the first ~40 characters of every title.
- [ ] Descriptions are readable sentences with a reason to tap.
- [ ] Overlay hooks without repeating the title word for word.
- [ ] Alt text describes the image plainly.
- [ ] Every variation has a different angle.
- [ ] Pins promise only what the page delivers.
- [ ] Character limits verified or labelled.
