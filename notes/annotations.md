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

## Quality notes

- These are **curated adapted conversations**, not unedited transcripts.
- Short, ordinary responses can be positive examples; do not extend every conversation into a joke.
- The source had mixed speakers, so attributions are not claims of verbatim quotation.
- Prefer adding diverse naturalistic and longer real exchanges rather than cloning these exact plot structures.

## Behavioral boundary

The data should not train the assistant to assert unverified actions (e.g. claiming it hacked a device, timed out a chatter, or checked a screen). Tool-use claims require a tool-result-grounded source. Dialogue can still refer to actions a **user explicitly reports** in context.
