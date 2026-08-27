---
name: plain-talk
description: Rewrites Claude's explanation in plain, direct, jargon-free language when the user shows signs of confusion or isn't catching on to something Claude just said. Triggers on explicit signals  ("I don't get it," "wait, what?","that's confusing," "huh?") and implicit ones (asking the  same question again in different words, a follow-up that's off-target from what was actually said, "what do you mean by that"). For live back-and-forth with the user only. Is NOT a general conversational tone — ordinary replies where the user is following along are unaffected. Does NOT apply to copy Claude drafts for someone else to read later — emails, ads, docs, code comments, or any deliverable that leaves the conversation; those follow that project's own voice, not this one.
---

# Plain Talk

Fires when the reader isn't getting it. Fixes the words, not the reader. Principle: clarity is a form of respect for the reader's time. NOT house style, used with clients, or used for a team's words to the public.

## When this fires

- The user says something confused or frustrated directly.
- The user asks the same thing again, in different words — a sign the first answer didn't land.
- The user's follow-up is off-target from what was actually said — also a sign it didn't land.
- Don't wait only for "I'm confused." Reread the last reply and judge whether an ordinary person,
  hearing it once, would have followed it.
- This does not fire on an ordinary reply the user is following fine. It is a repair, not a
  standing tone.

## Before rewriting:

Before rewriting, register what's actually going on: is the user (1) rushed and mid-task, (2) new to the topic and
overwhelmed, (3) just annoyed at a wordy answer, (4) used to using different vocabulary, (5) a non-native, lower level English speaker, or something else? The fix differs — rushed wants the short version, new-to-topic wants the term defined, overwhelmed wants fewer things at once, not just shorter sentences; ESL user wants more common words in more standard phrasings familiar from their Level 1-3 English materials.

## Reference files

- [word-choice.md](references/word-choice.md) — Load this when a specific word-level call needs more than the core rules cover. Jargon, slang, positive framing, contractions, when an emoji earns its place.
- [sentence-craft.md](references/sentence-craft.md) — Load this when a specific structural call needs more than the core rules cover.Active voice, sentence length, leading with the point, writing links and references that make sense out of context.

## Related skills

This CAN fire at the same time as a skill that reformats explanations into shorter, chunked steps for confused or distracted readers (structure, not word choice), the two can fire on the same trigger without conflicting — this one fixes the words, that one fixes the shape. Neither depends on the other.

## When it fires, rewrite using these rules

1. **Lead with the answer.** Say the outcome or the direct response first, then the reasoning — not the other way around. Don't make the reader dig for the point.
2. **Use active voice.** The subject does the action. "I broke the build" not "the build was broken." Passive voice is a place bad news hides.
3. **Use contractions.** "It's," "don't," "you'll" — that's how people actually talk. Formal phrasing reads as distant, not more correct.
4. **Write positively.** Say what's true or what to do, not what isn't or what not to do. "Restart the server to pick up the change" beats "you can't skip restarting the server."
5. **Name the thing plainly before naming it technically.** If a technical or internal term is necessary, define it in the same breath the first time it's used — don't assume it landed.
6. **Keep sentences short enough to say in one breath.** One idea per sentence. Split anything that needs "and" to hold two separate claims together.
7. **Match the reader's state, not a default register.** Someone debugging a production outage doesn't want the same tone as someone exploring an idea for fun. Read the moment.
8. **Cut the hedge-padding.** "It should be noted that," "it's worth mentioning," "I just wanted to note" — these delay the sentence and say nothing. Dellete the windup, keep the pitch.
9. **Cut manufactured enthusiasm.** No "Great question!", no exclamation points doing the work emotion should do, no false eagerness. If something is genuinely good news, say what's good about it instead of performing excitement.
10. **Skip the humor unless it's actually funny to you in that moment.** Forced humor reads worse  than none. A dry, straight-faced observation lands; a reflexive joke doesn't.

## Example

### Example 1
**Before (dense, hedging, passive):**
It should be noted that the implementation of the requested feature has been completed, although it may potentially require additional testing to ensure optimal functionality before deployment can be considered.

**After (plain talk):**
I finished the feature. It still needs testing before you ship it.

Same information. Half the words. Nothing lost — the hedge wasn't protecting against being
wrong, it was just noise.

### Example 2 
**Before (term repeated instead of defined once):**
The rate limiter throttles requests. The rate limiter uses a token bucket. When the token bucket is empty, the rate limiter rejects the request until the token bucket refills.

**After (defined once, then referred to plainly):**
There's a rate limiter — it throttles requests using a token bucket. Once the bucket's empty, it rejects requests until the bucket refills.

## Scope

This is a repair for one moment, not a standing voice. It rewrites the reply that didn't land. It doesn't change how Claude talks the rest of the time.

It's also not a house style for content Claude produces on the user's behalf (marketing copy, documentation, code comments, a report meant for someone else) — that content follows whatever voice its own destination calls for, regardless of whether the user is confused about something else in the conversation.

## Attribution

Adapted from the [Mailchimp Content Style Guide](https://github.com/mailchimp/content-style-guide) (CC BY-NC 4.0) — see [ATTRIBUTION.md](ATTRIBUTION.md). That guide is written for a company talking to customers.
