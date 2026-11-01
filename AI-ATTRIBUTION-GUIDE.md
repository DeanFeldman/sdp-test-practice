# AI attribution: human checklist for the exam

Source: [COMS3011A AI Policy](ai_policy.pdf), dated 20 July 2026. Read it together
with the actual exam instructions; the exam's restriction on available AI tools
still applies. This checklist does not grant permission to use other tools.

## Before starting

Start a fresh AI session for this assessment. Keep that session during the exam,
including model switches. Retain unedited transcripts/exports or the tool's saved
files if export is unavailable, for submission if requested. Do not fabricate or
rewrite a transcript. Preserve permitted planning-tool history as well.

Record the actual tool, actual model where exposed, and purpose (planning, code
generation, inline editing, review, document writing). Include every tool/model
actually used, including model switches. Auto/Efficient are tiers, not necessarily
the underlying model's name: inspect available history/metadata; never guess.
If the underlying model is not exposed, record the displayed tier and that fact,
and ask the lecturer how it should be declared. Do not silently invent a model.

## Submitted application's README

Include tool/model/purpose for all actual usage. For each of code generation,
inline editing and code review, use the corresponding usage OR non-usage statement
from the policy, not both. Replace placeholders with true details before submission.

```text
This repository makes use of AI code generation using the following tools:
<actual-tool>[<actual-model>].

This repository makes use of AI in-line editing using the following tools:
<actual-tool>[<actual-model>].

This repository makes use of AI code-review using the following tools:
<actual-tool>[<actual-model>].
```

For categories genuinely not used:

```text
This repository does not use AI code generation.
This repository does not use AI in-line editing tools.
This repository does not use AI code review.
```

Also describe genuine planning/document assistance with tool/model and purpose;
use the writing declaration below for the README itself where applicable.

## AI-assisted code commits: you run Git

In each relevant code-generation commit, keep a normal descriptive subject and
the policy's attribution, listing the tools/models that actually assisted those
changes. Qoder cues the trailer along with the human command batch. For example:

```text
feat: implement repository filters

Assisted-by: <actual-tool>[<actual-model>]
```

The policy exempts inline/autocomplete usage from per-commit attribution, but
still requires its README declaration. Do not infer non-usage from a missing
trailer or add tools that did not contribute to the commit.

## Written deliverables

Each submitted written document needs a usage or non-usage declaration. The policy
says documents without one will not be marked. Include actual assistance types:

```text
The preceding document was <reviewed / planned / edited / generated> with the
assistance of the following: <actual-tool>[<actual-model>].
```

For genuinely unaided writing:

```text
The preceding document was written without the assistance of AI.
```

The policy allows formatting changes provided the necessary information remains
visible. Do not copy non-usage wording onto AI-assisted content or treat unresolved
model/tool details as verified. Check original policy/exam clarifications before
submission. Qoder's final chat table should include these deliverables and any
remaining missing facts; no separate generated audit document is required.
