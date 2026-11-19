# datasets

Curated, compact conversational SFT examples for an experimental AI VTuber personality (Gemma 4 12B via Axolotl).

## Data

- `data/behavior_multiturn.jsonl` – **6 multi-turn conversations**, OpenAI `messages` JSONL format, one JSON object per line.
- `notes/annotations.md` – behavioral rationale and provenance; **not included in training data**.
- `axolotl/dataset-snippet.yml` – minimal Axolotl dataset configuration fragment, to merge into a model-specific training config.

The desired behavior is context-grounded, playful reinterpretation, mild audacity and natural short responses – **not** forced jokes or cyberpunk vocabulary.

## Axolotl

```yaml
chat_template: tokenizer_default
datasets:
  - path: data/behavior_multiturn.jsonl
    type: chat_template
    roles_to_train: ["assistant"]
train_on_inputs: false
```

The tokenizer's **actual** Gemma 4 chat template should be confirmed against the model and inference setup. This is a dataset configuration fragment, **not a complete Gemma 4 12B training configuration**. Verify EOS/EOT labels and loss masks in an Axolotl preprocessing dry run before training.

Six examples alone are insufficient for a generalizable fine-tune. Keep validation dialogs separate from training data, and compare base model vs adapter on unseen conversations.

## Curation

Conversation 006 is a speech-only adaptation of a moderation incident: it does not contain claimed executed timeouts. See `notes/annotations.md` for source-level provenance.

Inspired by situations in a Neuropunk 2077 stream; manually paraphrased/adapted to remove names and game-specific details, **not presented as verbatim Neuro-sama transcripts**. Public reuse rights for third-party source materials should be reviewed before expansion with direct quotations.

Annotations are deliberately separated from `messages` to prevent teaching the model the evaluation labels.

See [Axolotl's conversation dataset documentation](https://docs.axolotl.ai/docs/dataset-formats/conversation.html).
