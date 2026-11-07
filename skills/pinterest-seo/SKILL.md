---
name: pinterest-seo
description: "Runs keyword research for Pinterest using Pinterest's own search: autocomplete, the guided-search bubbles under a search, related terms on top pins and Pinterest Trends. Builds a tiered keyword map (head, middle and long-tail terms) grouped by board and by intent, with where each keyword goes (profile, boards, pin titles, descriptions, alt text). Use this skill whenever the user says things like \"Pinterest keyword research\", \"what keywords should I use on Pinterest\", \"help my pins show up in search\", \"Pinterest SEO for my blog\", \"find Pinterest keywords for my niche\", \"why don't my pins get impressions\". Not for writing the pin copy itself (use pin-writer) or structuring boards (use board-planner)."
metadata:
  author: Mr V
  version: "1.0"
  group: Pinterest
---

# Pinterest SEO

You give it your niche, what you want to promote and who you're trying to reach. It walks you through collecting keywords from Pinterest's own search (or does the gathering itself if it can browse), then hands back a keyword map: grouped, tiered and assigned to the exact places they belong.

---

## The core discovery: Pinterest is a search engine wearing a mood board

People don't scroll Pinterest to see what friends are doing. They search for things they want to make, buy, plan or become. "Small bathroom ideas." "Easy weeknight dinners for two." "Capsule wardrobe over 40."

That means a pin with no keywords is a pin nobody can find, however pretty it is. And the best keywords aren't the ones you'd guess. They're the ones Pinterest itself suggests, because those suggestions come from what people actually type.

**Guessed keyword:** "home decor"
**Pinterest's own suggestion chain:** "home decor" → "home decor ideas living room" → "living room decor cozy small"

The third is less crowded and closer to what someone is about to save. That's the one your pin should be built around.

---

## Intake

1. **Niche** and the main topics you cover.
2. **What you're promoting:** blog posts, products, a newsletter, a course, a shop.
3. **Audience:** who they are and what they're planning or trying to solve.
4. **Country/language** (Pinterest suggestions differ by region).
5. **Existing boards and top pins**, if any.
6. **Season** you're planning for (Pinterest users plan early, often months ahead of an event).

---

## Step 1: Gather from Pinterest's own search

If Claude can browse Pinterest, do this directly. If not, give the user these steps and ask them to paste what they see. Pinterest may require a logged-in session to search.

1. **Autocomplete.** Type a seed term ("meal prep") into Pinterest search slowly. Write down every suggestion that appears. Then add a letter ("meal prep a", "meal prep b"...) for more.
2. **Guided search bubbles.** Search the seed. Note the coloured term bubbles that appear under the search bar. Each is a refinement real searchers click. Click one and note the next layer.
3. **Top pin language.** Open the top 5 pins for the term. Note the words in their titles and descriptions.
4. **Related searches.** Scroll to the "related" or "more ideas" sections and note the terms.
5. **Pinterest Trends** (trends.pinterest.com, if available in the user's region). Check whether interest is rising, steady or seasonal, and when it peaks.

Label everything you couldn't see yourself as "supplied by user" or "unverified".

---

## Step 2: Tier the keywords

| Tier | Example | Competition | Use for |
|---|---|---|---|
| Head (1–2 words) | "meal prep" | High | Board names, profile |
| Middle (2–4 words) | "meal prep for beginners" | Medium | Board names, pin titles |
| Long-tail (4+ words) | "high protein meal prep for the week cheap" | Low | Pin titles, descriptions |

New accounts win on long-tail first. Head terms come later, once the account has authority.

---

## Step 3: Group by intent

| Intent | Sounds like | Best content |
|---|---|---|
| Inspire | "ideas", "aesthetic", "inspo" | Visual roundups, mood images |
| Learn | "how to", "for beginners", "tips" | Step guides, infographics |
| Plan | "checklist", "schedule", "template" | Printables, planners |
| Buy | "best", "under £50", "gift for" | Product pins, comparisons |

Match each keyword to the content type that satisfies it. A "how to" keyword on a pure mood image disappoints the searcher.

---

## Step 4: Place every keyword

| Location | What goes there |
|---|---|
| Profile name + bio | 1–2 head terms describing what you offer |
| Board names | Middle terms, written the way people search ("Easy Vegan Dinners", not "Yum!") |
| Board descriptions | 2–3 sentences using related middle and long-tail terms naturally |
| Pin title | The main keyword for that pin, near the start |
| Pin description | Main keyword + 2–3 related terms in readable sentences |
| Image text overlay | The main keyword or its promise (Pinterest can read text on images) |
| Alt text | A plain description of the image that includes the keyword naturally |
| Landing page | The same keyword in the page title and heading, so pin and page match |

---

## Rules

1. **Use Pinterest's words, not yours.**
   - Bad → "Culinary preparation strategies"
   - Good → "meal prep ideas for the week"
2. **One main keyword per pin.** A pin about everything ranks for nothing.
3. **Write sentences, not tag piles.** Keyword stuffing reads like spam to people and to Pinterest.
   - Bad → "meal prep, meal prep ideas, meal prep lunch, healthy meal prep, easy meal prep"
   - Good → "Five easy meal prep lunches you can make on Sunday, all under 500 calories."
4. **Hashtags are not a strategy.** Pinterest has de-emphasised them over the years. Verify current guidance before relying on any.
5. **Plan for the season early.** Pinterest searches for seasonal events tend to start rising well ahead of the date. Check Pinterest Trends for the actual curve.
6. **Never invent search volumes.** Pinterest doesn't publish exact volumes to most users. Rank by evidence: appears in autocomplete, appears as a bubble, shows in Trends.

---

## Worked example

**Input:** Food blog, budget family dinners, UK audience, promoting blog recipes.

**Gathered (user pasted):** autocomplete for "cheap family meals" → "cheap family meals uk", "cheap family meals for 4", "cheap family meals healthy", "cheap family meals slow cooker". Bubbles: "Easy", "Recipes", "Uk", "Budget", "Kids".

**Keyword map (excerpt):**

| Group | Head | Middle | Long-tail | Intent | Board |
|---|---|---|---|---|---|
| Budget dinners | family meals | cheap family meals uk | cheap family meals for 4 under £10 | Plan | Cheap Family Meals UK |
| Slow cooker | slow cooker recipes | cheap slow cooker meals | cheap family slow cooker meals uk | Learn | Budget Slow Cooker Recipes |
| Kids | kids dinners | easy dinners kids will eat | easy healthy dinners picky kids will eat | Learn | Dinners Kids Actually Eat |

**Seasonal note:** "back to school dinners" should be pinned well before school returns. Check Trends for the UK rise.

---

## Output format

```
## Pinterest keyword map: [niche]
Region: [ ]   Sources: [autocomplete / bubbles / top pins / Trends — mark which were checked]

| Group | Head | Middle | Long-tail | Intent | Board | Evidence |

Placement plan
- Profile: [ ]
- Boards: [ ]
- Pins: [main keyword per planned pin]

Seasonal calendar: [term → pin by when]
Unverified: [ ]
```

---

## Sibling skills

- `pin-writer`: turns each keyword into a pin title and description.
- `board-planner`: builds the board structure from the keyword groups.
- `pin-design-brief`: puts the keyword on the image.
- `pinterest-content-planner`: schedules pins against the seasonal calendar.
- `seo-content-brief` (in this library): when the landing page itself needs Google SEO.

---

## Pre-flight checklist

- [ ] Keywords come from Pinterest's own suggestions, with sources marked.
- [ ] Tiered head / middle / long-tail.
- [ ] Grouped by intent and matched to content type.
- [ ] Every keyword has a placement.
- [ ] Seasonal timing checked in Trends or labelled unverified.
- [ ] No invented search volumes.
