---
name: pin-design-brief
description: "Writes a design brief for Pinterest pins built to be saved: vertical layout, one hero image, a text overlay that names the keyword or promise, colour and font choices, and a small-screen read test, delivered as 2 to 3 concepts plus a reusable template set for your brand. Use this skill whenever the user says things like \"design brief for my pins\", \"what should my Pinterest pins look like\", \"pin layout ideas\", \"text overlay for Pinterest\", \"make my pins look better\", \"Canva brief for Pinterest\", \"pin templates for my brand\". Not for the pin title and description (use pin-writer) or for video pins (use idea-pin-scripter)."
metadata:
  author: Mr V
  version: "1.0"
  group: Pinterest
---

# Pin Design Brief

You give it the pin's keyword, its promise and what images you have. It hands back 2 to 3 pin concepts, each a brief you (or a designer, or Canva) can build without guessing, plus a template set so every future pin looks like yours.

This skill writes the brief. It doesn't draw the pin.

---

## The core discovery: people save what they'll need later

A Facebook post asks "will you react now?" A pin asks "will you want this again?" The save is the action that matters. It tells Pinterest the pin is worth showing to more people, and it keeps your link in the saver's boards for months.

So a pin's design has one job: make the future value obvious in a glance.

**Pretty but vague:** a beautiful kitchen photo, no text.
**Saveable:** the same photo, top third reads "Small Kitchen Storage: 11 Ideas Under £20", a list icon in the corner.

The first gets admired. The second gets saved, because the viewer knows exactly what they'll find when they come back.

---

## Intake

1. **The pin's keyword and promise** (from `pin-writer` if available).
2. **Images available:** your own photos, product shots, screenshots, stock.
3. **Brand:** colours, fonts, logo or URL.
4. **Pin type:** single image, infographic/checklist, before/after, product, collage. (Video and multi-page pins → `idea-pin-scripter`.)
5. **Tool** they'll build in (Canva, Figma, Photoshop, an image AI).

Verify current recommended pin dimensions in Pinterest's help centre when web search is available. At the time of writing, the standard is a 2:3 vertical ratio (for example 1000 × 1500 pixels).

---

## The six pin layouts

| Code | Layout | Best for |
|---|---|---|
| L1 | Photo + text band | Most blog posts. Image with a solid band holding the headline. |
| L2 | Full-bleed + overlay | Strong photos with clear space for text. |
| L3 | Checklist / infographic | "How to", steps, printables. Text-led. |
| L4 | Before / after split | Makeovers, transformations, results. |
| L5 | Collage grid | Roundups ("15 ideas"). 3–4 images max. |
| L6 | Product hero | Shop pins. Product on clean background, price or benefit text. |

---

## Rules

1. **Vertical, always.** Horizontal pins shrink in the feed. Very tall pins may get cut off.
2. **One hero.** One image or one idea owns the pin.
   - Bad → 9 tiny photos and 4 lines of text.
   - Good → one clear photo, one headline.
3. **Text names the keyword or the promise.** Pinterest can read text on images, and people skim it first.
   - Bad → "So Pretty!"
   - Good → "Rental-Friendly Wall Ideas"
4. **3 to 8 words of headline, maximum two fonts.** A bold readable font for the headline, a simple one for any subline.
5. **Contrast for small screens.** Dark text on light, or light on dark. Never text over a busy part of the photo without a band or shadow.
6. **Brand it quietly.** Small logo or URL at the bottom. It protects against your pin being re-uploaded and builds recognition. Never let it compete with the headline.
7. **Show the payoff.** Numbers ("11 Ideas"), formats ("Free Checklist"), outcomes ("Before & After").
8. **Fresh beats repeated.** Each pin for the same link uses a new image or a new layout. Pinterest favours new creative.
9. **Honest images.** Show what's actually on the page. No stock image of a dish that isn't in the recipe.

---

## The small-screen test

Shrink the design to roughly the size of a phone feed thumbnail. Check:
- Can you read the headline?
- Can you tell what the image shows?
- Does one thing grab you first?

If any answer is no, simplify: bigger text, fewer words, one image.

---

## Steps

1. Intake.
2. Pick 2 to 3 layouts that fit the content.
3. Write a brief for each (template below).
4. Run the rules and the small-screen test.
5. Recommend which to publish first.
6. Optionally, build a template set: 3 to 5 reusable layouts in the brand's colours and fonts so every new pin takes minutes.
7. If they're using an image AI, write the image prompt without text. Add text afterwards in a design tool, because image models still mangle lettering.

---

## Brief template

```
CONCEPT [A/B/C] — Layout [L1–L6]
Size: 2:3 vertical (verify current spec)

HERO IMAGE
[what it shows, angle, crop, mood]

HEADLINE (3–8 words)
"[text]"   Position: [top band / centre / bottom third]
Font: [bold sans / serif], colour [ ], size [large]

SUBLINE (optional)
"[text]"

BRANDING
[logo/URL, bottom centre, small]

COLOURS
[background / text / accent]

SMALL-SCREEN CHECK
[what must read; what to drop if it doesn't]
```

---

## Worked example

**Input:** Keyword "small kitchen storage ideas". Blog post with 11 ideas, all under £20. Own photos of 6 of them. Brand: sage green and cream, Playfair + Montserrat.

**Concept A — L1 Photo + text band**
- Hero: overhead shot of the over-the-sink shelf, bright daylight.
- Headline: "Small Kitchen Storage Ideas" in a cream band, top third, Montserrat Bold, sage.
- Subline: "11 fixes under £20".
- Branding: URL bottom centre.
- Small-screen: headline and shelf must read. Drop the subline if cramped.

**Concept B — L5 Collage**
- Hero: 4-photo grid, the best 4 ideas.
- Headline: "11 Small Kitchen Storage Ideas" on a sage band across the middle.
- Small-screen: risk of clutter. Keep to 4 photos, no more.

**Concept C — L3 Checklist**
- Hero: cream background, sage icons, 5 of the ideas listed.
- Headline: "Small Kitchen? Start Here".
- Best for: saves from people who want a quick reference.

**Publish first:** A (clearest keyword and image). Then C a week later as a fresh pin.

---

## Output format

```
## Pin design brief: [keyword]

[Concept A brief]
[Concept B brief]
[Concept C brief]

Publish first: [ ], because [ ]
Template set (optional): [3–5 layouts with colour/font specs]
Image AI prompt (optional, no text): [ ]
```

---

## Sibling skills

- `pin-writer`: the title, description and overlay wording.
- `pinterest-seo`: the keyword the headline carries.
- `idea-pin-scripter`: video and multi-page pins.
- `board-planner`: board covers that match the template set.
- `carousel-generator` (in this library): when you need multi-slide graphics.

---

## Pre-flight checklist

- [ ] Vertical, dimensions verified or labelled.
- [ ] One hero, one headline of 3 to 8 words.
- [ ] Headline names the keyword or the promise.
- [ ] Two fonts maximum, strong contrast.
- [ ] Quiet branding.
- [ ] Small-screen test passed.
- [ ] Images honestly represent the page.
