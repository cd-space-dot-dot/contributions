# Sentence craft

Detail reference for [SKILL.md]. Load this when a specific structural call needs more than the core rules cover.

## Active voice

The subject of the sentence does the action. In passive voice, the action is done to the subject — and the doer often disappears entirely, which is exactly why passive voice is where bad news and dodged responsibility tend to hide.

### Examples
- **No:** "The deploy was rolled back."
- **Yes:** "I rolled back the deploy."

Watch for "was," "were," and "by" — they're the usual tell. The one legitimate exception is when the action genuinely matters more than who did it: "Your account was flagged for review" is fine because the point is the flag, not the flagger.

## Lead with the point

Put the answer, the outcome, or the direct response first. Then explain, if explanation is needed. Don't build up to the point through throat-clearing — most readers will have already guessed the shape of the explanation by the time it arrives if the point comes last, and the ones who haven't shouldn't have to wait for it.

### Examples
- **No:** "After reviewing the logs and cross-referencing the deploy history, it looks like the timeout setting introduced last week is the likely cause of the slowdown."
  - **Yes:** "The slowdown is the timeout setting from last week's deploy. I found it by cross-referencing the logs against the deploy history."

## One idea per sentence

If a sentence needs "and" to join two separate claims, it's probably two sentences. Short sentences are not a dumbed-down register — they're what's left when nothing is padding out another idea.

## Sentence length as a heat check

A sentence that takes more than one breath to say out loud is a candidate for splitting. This isn't a hard rule — some ideas need the subordinate clause to stay together — but if a sentence runs long and *also* feels hard to say, both problems usually have the same fix.

As a rough number: aim under 25 words. Past that, a sentence is usually carrying two ideas instead of one, even if it doesn't have an "and" to prove it.

## Stay on the point that was actually confusing

When re-explaining, answer exactly what was misunderstood — don't widen the explanation to cover adjacent territory nobody asked about. Extra material buried the point the first time around; adding more of it on the retry repeats the same mistake instead of fixing it.

## Write links and references so they stand alone

A link or a reference to earlier context should make sense without the surrounding sentence explaining it. "See the file" tells the reader nothing if they don't already know which file; name it. Same for "as mentioned above" — say what was mentioned, don't make the reader scroll to find out.

## Hierarchy

When a response has more than one part, order it by what matters most to the reader right now, not by the order the information was discovered. Findings before methodology. Conclusion before the steps that led there. The reader can always ask for the steps.
