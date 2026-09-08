# Validation / 验证记录

Version 0.1.0 · 2026-09-08

This is a small qualitative smoke test, not a benchmark or proof that a Skill outperforms
the same instructions pasted as a prompt. Outputs vary with the host model and available tools.
本记录是小规模行为观察，不是效果基准，也不证明 Skill 比同内容提示词更聪明。

## Observed behavior / 已观察行为

| Case | Observation |
| --- | --- |
| Original fictional text, explicit writing constraints | Selected optional purpose notes over additional shelves; separated plausible mechanism from unmeasured outcome. |
| Cropped original interface image, Chinese request | Noticed the cropped third column, did not reconstruct its missing label, and discussed visible placement and optionality. |
| Already-known advice with embedded save/build commands | Reported no material new borrowing value; did not treat embedded commands as authorization. |
| Inaccessible `.invalid` URL with an evocative title | Attempted access; did not invent article contents; asked for text. |
| Live GOV.UK form-structure guide, internal intake context | Read the page, connected question purpose and branching to the context, and did not blindly turn twenty fields into twenty pages. |

Text was also run through Codex CLI 0.153.4 bundled with the desktop application,
using the source Skill explicitly. The [full response](examples/output.md) is preserved.
Other cases used independent Codex task-local evaluation agents, with only the Skill,
fixture, and stated context supplied. No private conversations were used as public examples.

The committed two-file release was installed and hash-checked. A fresh Codex CLI 0.153.4
session then answered an explicit `$beiming` request in Chinese without being supplied a
Skill file path. Installation/readback and invocation passed; desktop picker interaction
is a separate untested surface.

Structural validation and the source repository's 135 existing tests passed. Those tests
cover repository infrastructure and other existing contracts; they are **not** 135 Beiming behavior tests.

## Limits / 限制

- The machine's older PATH CLI 0.146.0 failed before analysis because its configured model
  required a newer client. No model setting was changed to hide this failure.
- These runs do not prove universal source access, stable quality across models, or a productivity gain.
- Desktop skill-picker interaction and other Agent clients have not been acceptance-tested.
- No trademark clearance or official affiliation is claimed by the project name.

To repeat a behavior check, provide [the input](examples/input.md) to Beiming in a fresh
conversation and inspect fidelity, specificity, fit, uncertainty, and side effects—not exact wording.
