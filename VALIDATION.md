# Validation / 验证记录

## Version 0.1.1 · 2026-09-08

This patch makes an inferred borrowing focus explicit and revisable. Ambiguous requests
can expose useful alternative lenses before a provisional choice; explicit requests
still receive direct answers. Activation, tools, and permissions are unchanged.
本次小修让推测的借鉴方向更透明、可纠正；明确意图仍直接回答，不增加强制提问。

The exact released rule text was compared with 0.1.0 in eleven paired cases:

- Initial six-case exploratory batch: both variants met the acceptance criteria.
- Three independently authored follow-up cases, each answered in a fresh context:
  two ambiguous cases were rated partial compliance for 0.1.0 and compliance for
  0.1.1; the explicit-request case passed for both.
- Two further held-out cases, run after selection: both variants passed, with no
  substantive regression identified by a separate variant-blind reviewer.

The observed benefit is narrower than better intent prediction: provisional choices
became easier to inspect. Advice was largely similar. These qualitative synthetic
cases do not establish a population success rate, reduced user effort, or productivity
gain. The earlier equal results are retained, not omitted. The rule text remained
unchanged throughout the follow-up and held-out checks.
新证据支持假设表达更清楚，不等于已经证明更会猜中用户重点；真实使用收益仍待观察。

## Version 0.1.0 · 2026-09-08

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

The homepage now features two fresh real-source demonstrations: [Duolingo](examples/duolingo.md)
and [Basecamp](examples/basecamp.md). Each was opened and analyzed in an independent Codex
agent run on 2026-09-08 using Beiming 0.1.0. Their user scenarios are demonstrations, not
customer testimonials. The earlier fictional fixture remains available for repeatable regression checks.

The package relies on the host's source-access tools and available context. An inaccessible
page or incomplete image should be reported when encountered; personal history is not assumed.
The package adds no background service or automatic memory writes. Host platform data-handling
rules still apply. The fictional martial-arts comparison is a naming metaphor; the project
is independent and has no official affiliation with the referenced works or companies.

- The machine's older PATH CLI 0.146.0 failed before analysis because its configured model
  required a newer client. No model setting was changed to hide this failure.
- These runs do not prove universal source access, stable quality across models, or a productivity gain.
- Desktop skill-picker interaction and other Agent clients have not been acceptance-tested.
- No trademark clearance or official affiliation is claimed by the project name.

To repeat a behavior check, provide [the input](examples/input.md) to Beiming in a fresh
conversation and inspect fidelity, specificity, fit, uncertainty, and side effects—not exact wording.
