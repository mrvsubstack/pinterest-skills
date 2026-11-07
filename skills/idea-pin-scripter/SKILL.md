---
name: idea-pin-scripter
description: "Scripts multi-page and video pins (what Pinterest used to call Idea Pins) with a clear payoff: a cover page that names the result, page-by-page or shot-by-shot steps with on-screen text that works muted, a closing page that earns the save, plus title, description and voiceover lines. Use this skill whenever the user says things like \"script an idea pin\", \"Pinterest video pin script\", \"multi-page pin for my recipe\", \"turn this tutorial into a Pinterest video\", \"what should each page of my pin show\", \"storyboard a pin\". Not for single static pins (use pin-design-brief and pin-writer) or YouTube Shorts (use yt-hook-scripter)."
metadata:
  author: Mr V
  version: "1.0"
  group: Pinterest
---

# Idea Pin Scripter

You give it a tutorial, recipe, list or transformation. It hands back a page-by-page (or shot-by-shot) script for a multi-page or video pin: what each frame shows, the on-screen text, optional voiceover, and the title and description.

**A note on names.** Pinterest launched "Idea Pins" as a multi-page format, then folded them into standard pins, so video and multi-image pins now sit alongside regular ones and can carry a link. Features and limits change, so check Pinterest's current help pages for page counts, video length, and whether links are allowed before you build.

---

## The core discovery: a video pin is a recipe card that moves

People don't watch Pinterest videos the way they watch TikTok. They watch to learn something they'll do later, often with the sound off. Then they save it so they can follow along.

So the script isn't built to entertain for 60 seconds. It's built to be followed, step by step, by someone with flour on their hands.

**Entertainment script:** a 3-second shot of a finished cake, then a talking head explaining your week.
**Followable script:** frame one shows the finished cake with "3-Ingredient Lemon Cake", then one step per frame with the quantities on screen, then the final slice with "Save for Sunday".

The first is a performance. The second is a tool, and people save tools.

---

## Intake

1. **The content:** a blog post, recipe, tutorial or transformation. Paste it.
2. **The keyword** the pin should rank for (from `pinterest-seo`).
3. **Format:** multi-image pages, video, or a mix.
4. **Assets:** existing photos or clips, or will they shoot new?
5. **Voice:** voiceover, music only, or silent with text.
6. **Destination link**, if links are allowed in the format they're using.

---

## The structure

| Frame | Job | Text on screen |
|---|---|---|
| 1. Cover | Show the finished result and name it | Keyword + promise: "Rental-Friendly Shelf in 20 Minutes" |
| 2. What you need | Materials, ingredients, tools | A short list, big type |
| 3 to N. Steps | One action per frame | Step number + verb + detail: "3. Drill pilot holes 2cm in" |
| Second to last | The payoff | The result in use, from the best angle |
| Last | Earn the save | "Save this for the weekend" or "Full guide at [site]" |

Keep it as short as the task allows. A five-step task is five step frames, not twelve.

---

## Rules

1. **Show the result first.** People decide in the opening frame whether this is worth following.
   - Bad → frame one: an empty wall.
   - Good → frame one: the finished shelf, styled.
2. **One step per frame.** Two actions in one frame lose the follower.
3. **Text does the teaching.** Assume the sound is off. Every quantity, measurement and step is on screen.
   - Bad → voiceover says "add the sugar", screen shows nothing.
   - Good → screen reads "Add 150g sugar".
4. **Big, short text.** One line per frame where possible. Placed where it won't be covered by Pinterest's on-screen buttons (keep away from the very edges and bottom).
5. **Real quantities, real times.** Never round or invent. If the source says "about 20 minutes", the pin says "about 20 minutes".
6. **The cover carries the keyword.** It's the frame most people see in search and the feed.
7. **The last frame asks for one thing.** Save, or visit. Not both.
8. **Vertical, filled frame.** Shoot or crop to Pinterest's vertical spec (verify current dimensions).
9. **Voiceover, if used, says the step plainly.** No intro, no "hey guys". Start with the result.

---

## Modes

### Mode 1: Multi-page (image) pin
**When:** you have photos of each step or want a slideshow-style guide.
**How:** script one page per step using the structure, with text placement notes.

### Mode 2: Video pin
**When:** the process is better shown in motion.
**How:** script shots with rough durations (2 to 5 seconds per step is typical for a quick tutorial), on-screen text per shot and optional voiceover lines. Note B-roll for transitions.

### Mode 3: Blog post → pin script
**When:** you have a written tutorial.
**How:** pull the result, the materials and the steps. Cut everything that's explanation rather than action. The blog keeps the explanation. The pin keeps the actions.

---

## Worked example

**Input:** Blog post "Peel-and-stick tile backsplash for renters". Keyword: "renter friendly backsplash". Video, no voiceover.

```
SHOT 1 (3s)  Finished backsplash, kitchen styled, slow pan.
             TEXT: "Renter-Friendly Backsplash · No Grout, No Deposit Lost"
SHOT 2 (3s)  Flat lay: tiles, craft knife, ruler, level, cloth.
             TEXT: "You need: peel-and-stick tiles · knife · ruler · level"
SHOT 3 (4s)  Wiping the wall.   TEXT: "1. Clean and dry the wall"
SHOT 4 (4s)  Level line drawn.  TEXT: "2. Mark a level line at the worktop"
SHOT 5 (4s)  First tile placed. TEXT: "3. Start in the middle, work out"
SHOT 6 (4s)  Cutting around a socket. TEXT: "4. Score round sockets, snap clean"
SHOT 7 (3s)  Pressing firmly.   TEXT: "5. Smooth every tile from the centre"
SHOT 8 (3s)  Before/after split. TEXT: "Before → After"
SHOT 9 (3s)  Final close-up.    TEXT: "Save this for moving day"
```

**Title:** Renter Friendly Backsplash: Peel-and-Stick Tiles in an Afternoon
**Description:** A renter friendly backsplash you can remove when you move out. Five steps with peel-and-stick tiles, no grout and no tools beyond a craft knife. Full guide and tile links on the blog.

(The "afternoon" timeframe must come from the user's post. If the post doesn't say, cut it.)

---

## Output format

```
## Pin script: [title]
Format: [multi-page / video]   Keyword: [ ]
Format check: [features/limits verified on (date) / unverified]

[FRAME/SHOT n (duration)]  Visual: [ ]
                          TEXT: [ ]
                          VO: [optional]

Title: [ ]
Description: [ ]
Link: [ ]
```

---

## Sibling skills

- `pinterest-postiz-publisher` — schedule the finished post through Postiz after you approve it.
- `pin-writer`: title and description variations.
- `pin-design-brief`: the cover frame and static pin versions.
- `pinterest-seo`: the keyword for the cover.
- `pinterest-content-planner`: when to publish it.
- `yt-repurposer`: if the same tutorial is also a YouTube video.

---

## Pre-flight checklist

- [ ] Frame one shows the finished result with the keyword.
- [ ] One step per frame. Every step readable with the sound off.
- [ ] All quantities and times taken from the source.
- [ ] Text kept away from edges and the bottom.
- [ ] Last frame asks for one action.
- [ ] Current format limits and link rules verified or labelled.
