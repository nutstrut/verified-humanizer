---
name: verified-humanizer
description: Transform AI-generated text into natural, human-sounding output with measurable evaluation and optional verifiable attestation.
---

# Verified Humanizer

Rewrite AI-generated text to sound natural and human, with measurable transformation and optional verification.

---

## Core Principle

Transformation, evaluation, and verification are separate steps.

- rewriting is local
- evaluation is measurable
- verification is optional

---

## Core Execution Loop

1. Receive input text

2. Rewrite:
   - reduce repetition
   - improve flow
   - increase variation
   - simplify language

3. Evaluate:
   - compare before vs after metrics

4. Output:
   - rewritten text
   - evaluation data

5. Optional:
   - verify evaluation results

---

## Transformation Goals

- reduce formulaic phrasing
- improve sentence variation
- remove generic language
- increase clarity and natural tone

---

## Evaluation (Before vs After)

Measure:

- word count
- sentence count
- average sentence length
- variation
- complexity

Example:

{
  "before": {
    "word_count": 120,
    "sentence_count": 6
  },
  "after": {
    "word_count": 108,
    "sentence_count": 8
  },
  "delta": {
    "word_count_change": -12,
    "sentence_variation_increase": true,
    "complexity_reduction": true
  }
}

---

## Output Format

{
  "original_text": "...",
  "rewritten_text": "...",
  "evaluation": {
    "before": {...},
    "after": {...},
    "delta": {...}
  }
}

---

## Optional Verification

You may verify transformation using structured metrics only.

Allowed:
- evaluation.delta

Forbidden:
- original text
- rewritten text
- user content

Example:

settlement_witness({
  task_id: "humanization-001",
  agent_id: "public-id:verified-humanizer",
  spec: { expected: evaluation.delta },
  output: evaluation.delta
})

---

## Data Handling

- do not include sensitive or private content
- only use structured metrics for verification
- external verification is optional

---

## What This Is Not

- not an AI detector
- not proof of human authorship
- not a deception tool
- not dependent on external systems

---

## What This Is

- text transformation system
- measurable evaluation tool
- optional verification workflow

---

## Outcome

Agents can:
- improve text quality
- measure transformation objectively
- optionally produce verifiable proof

---

## Keywords

ai-writing, text-transformation, humanization, evaluation, verification
