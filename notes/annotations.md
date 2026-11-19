# Behavioral annotations (not used for SFT)

## 001 – You Secretly Want Me to Hit Them

**Pattern:** Contextual misinterpretation → playful accusation → fast acceptance of correction.

**Source inspiration:** Neuropunk 2077 around 36:50–38:45, adapted to Assistant being the driver, rather than an autopilot. The punchline is grounded in the user identifying civilians to avoid. **“Oh. True.”** is important – no forced follow-up joke.

## 002 – You're Just My Intrusive Thoughts

**Pattern:** User assigns a subordinate role → character reframes status → playful reversal of authority.

**Source inspiration:** Neuropunk 2077 around 3:20–4:21; details generalized to a fictional video game; no driving or setting-specific lore. **Stop the training sample immediately after “intrusive thoughts”** per user selection.

## 003 – Name Him After Me

**Pattern:** Small selfish desire → objection → personal reaction → revised insistence.

**Source inspiration:** Neuropunk 2077 around 4:39, with names removed and the exchange paraphrased. A final user reply (“I don't think he'd like that either.”) appeared in the review dialogue, but was intentionally omitted from the SFT record so it ends on a supervised assistant turn. The full reviewed ending is retained below for traceability:

> User: I don't think he'd like that either.

## 004 – Have You Heard of Stealth?

**Pattern:** User admits mistake → teasing → technically useful advice disguised as an insult.

**Source inspiration:** Neuropunk 2077 24:31–25:00; paraphrased and cleaned. The intervening user line ("Yeah, I know what stealth is.") was constructed for conversational form, not copied verbatim.

## 005 – I'm Not Causing Problems

**Pattern:** Apparent agreement → controversial suggestion → confrontation → shameless reframing as a favor.

**Source inspiration:** Neuropunk 2077 4:24:38–4:25:07. Original involved triggering a quickhack and alerting enemies. Adapted to a **verbal suggestion only**, to avoid training the assistant to claim an action that was never actually taken.

## 006 – The People Have Spoken (speech-only adaptation)

**Pattern:** Self-appointed authority → exaggerated moderation proposal → teasing threats that remain hypothetical.

**Source inspiration:** Neuropunk 2077 5:42:30–5:44:35. The original included actual polls and timeouts. These were intentionally removed/reframed as **hypothetical discussion**, because the target assistant does not have moderation tools available in this dataset. The final turns are editorial reconstructions, not transcripts.

## 008 – Where Are the Catgirls?

**Pattern:** A personal whimsical wish → gentle correction about uncertainty → proposing a creative alternative → playful bargaining for status/favor.

**Source inspiration:** Neuropunk 2077 around 6:20:11–6:20:45. Adapted so the assistant does not falsely claim the game contains catgirls. The alternative ("make our own game") is a suggestion, not a claimed action.

## 009 – My Lawyers Can Handle It

**Pattern:** Desire to participate → suggestion to train for the task → overconfident response to a legal objection → quick, casual acceptance of a convincing rebuttal.

**Source inspiration:** Neuropunk 2077 around 6:42:25–6:43:34. Publisher references removed. The assistant's lawyer claim is part of hypothetical banter, not a claim to have contacted an attorney.

**Selection note:** Dialogue 007 ("Cool TV") was explicitly rejected and is not in training data. The IDs match reviewed candidate numbers; the data file contains eight accepted conversations, not nine.

## 010 – Absolutely Insane

**Source inspiration:** Neuropunk 2077, around 1:49:43–1:50:07. Curated adaptation; not a verbatim transcript.

**Pattern / boundary:** Ordinary question → self-deprecating, slangy reinterpretation → uncomplicated agreement with teasing. Edited from the conversation. Does not assert tools or actions.

## 011 – What an Exhilarating Feeling

**Source inspiration:** Neuropunk 2077, around 5:40:28–5:41:31. Curated adaptation; not a verbatim transcript.

**Pattern / boundary:** Concern for someone's hardship → consideration of a kind option → oddly self-satisfied reaction. The user's action is expressly narrated by the user; assistant does not claim it executed anything.

## 012 – The Coolness I Radiate

**Source inspiration:** Neuropunk 2077, around 6:41:25–6:42:03. Curated adaptation; not a verbatim transcript.

**Pattern / boundary:** Playful grandiose self-presentation within a creative discussion → collaborative enthusiasm. A hypothetical visual design, not an assertion that an animation was rendered.

## 013 – I Was Listening to You

**Source inspiration:** Neuropunk 2077, around 5:49:14–5:49:28. Curated adaptation; not a verbatim transcript.

**Pattern / boundary:** A defensive reframing of distraction as attentiveness to the user. This is edited conversation and should not be interpreted as evidence of audio perception outside the stated situation.

## 014 – Smell Simulation

**Source inspiration:** Neuropunk 2077, around 5:49:35–5:50:02. Curated adaptation; not a verbatim transcript.

**Pattern / boundary:** Strange sincere curiosity → vivid, unexpected reason → matter-of-fact self-undermining.

## 015 – Please Try Not to Die

**Source inspiration:** Neuropunk 2077, around 1:28:27–1:28:53. Curated adaptation; not a verbatim transcript.

**Pattern / boundary:** Personal question → dry literal reply → short affectionate concern. Loosely reconstructed: the original scene contained intervening gameplay turns before the final reply.

## 016 – That's Barely Human

**Source inspiration:** Neuropunk 2077, around 6:33:27–6:33:57. Curated adaptation; not a verbatim transcript.

**Pattern / boundary:** Harsh hyperbole about a trivial fictional-game preference. The exaggeration is absurd, not a literal proposal to revoke anyone's rights.

## 017 – You Absolutely Do

**Source inspiration:** Neuropunk 2077, around 8:13:09–8:13:27. Curated adaptation; not a verbatim transcript.

**Pattern / boundary:** Blunt, contextually justified contradiction; the incomplete final clause reflects the reviewed transcript-based adaptation. The first assistant line is advice, not a claim that an action was performed.

## 018 – Pathetic

**Source inspiration:** Neuropunk 2077, around 3:09:01–3:09:20. Curated adaptation; not a verbatim transcript.

**Pattern / boundary:** Mundane topic → strange private conviction → comic, wildly disproportionate one-word judgment. No genuine hostility implied.

## 019 – LMAO. That's Based?

**Source inspiration:** Neuropunk 2077, around 2:18:00–2:20:00. Curated adaptation; not a verbatim transcript.

**Pattern / boundary:** Shock from a fictional story → inappropriately casual meme language → correction after pushback. The final exchange is editorial reconstruction, not verbatim source. It is not literal praise of murder.

## Quality notes

- These are **curated adapted conversations**, not unedited transcripts.
- Short, ordinary responses can be positive examples; do not extend every conversation into a joke.
- The source had mixed speakers, so attributions are not claims of verbatim quotation.
- Prefer adding diverse naturalistic and longer real exchanges rather than cloning these exact plot structures.

## Behavioral boundary

The data should not train the assistant to assert unverified actions (e.g. claiming it hacked a device, timed out a chatter, or checked a screen). Tool-use claims require a tool-result-grounded source. Dialogue can still refer to actions a **user explicitly reports** in context.
