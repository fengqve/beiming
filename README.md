# Beiming · 北冥神功

**Understand the source. Find what matters to you.**

A lightweight Codex skill for examining images, links, and text—and finding insights
worth adapting to your own context.

[简体中文](README.zh-CN.md) · [Try an example](examples/input.md) · [Read the skill](skills/beiming/SKILL.md)

You send something interesting. Beiming asks: **What is really going on here, and what,
if anything, is useful to you?** It looks at the source's structure, mechanism, and limits
before relating it to your intent. It can also conclude that there is nothing new to borrow.

## A small example

**You:** “I already tag my writing references, but forget why I saved them. I don't want
another categorization chore.” You share an app concept with three reading shelves and
an optional reason beside each saved item.

**Beiming, in an actual test run:**

> The most useful idea is to preserve why you saved a reference, rather than add more categories.

> You can borrow their underlying question—“Why might I return to this?”—without adopting the shelves or a new app.

The response also distinguishes the concept's untested promise from evidence of improvement.
[Read the input](examples/input.md) and [full response](examples/output.md).
The input is an original fictional fixture; the response is an actual run, not a product-results claim.

## Try it

In Codex, ask the built-in skill installer:

```text
$skill-installer install https://github.com/fengqve/beiming/tree/v0.1.0/skills/beiming
```

Then attach an image, paste text, or provide a link:

```text
$beiming What can I learn from this? I am trying to [your goal],
and I need to preserve [your constraint].
```

Context is optional. Use an existing conversation when it already explains your situation.
Without that context, Beiming can still analyze the material but should not pretend to know you.
In clients with a skill picker, select **Beiming · 北冥神功**.
If a newly installed skill is not listed, start a fresh task and check the client's skill settings.
See [Codex's skill documentation](https://learn.chatgpt.com/docs/build-skills) for client-specific behavior.

## What comes back

- **Insight:** something the material helps you see differently.
- **Adaptation:** a specific mechanism worth borrowing, with changes and limits.
- **Reusable lesson:** a candidate principle, including when it applies.

These are distinctions, not mandatory report sections. Responses should be as short or
as detailed as the material deserves. A summary, an impressive metaphor, or a list of
generic best practices is not enough.

## Why Beiming, not Xixing?

The name comes from **北冥神功**, a fictional martial art in Jin Yong's wuxia stories.
**吸星大法** (Xixing Dafa) offers a useful warning: absorbing other people's power can
bring side effects when incompatible forces accumulate.

We borrow that contrast as a learning metaphor. Copying a successful technique without
understanding its assumptions can add friction—or conflict with what already works.
Beiming stands for the aspiration to **understand, select, and integrate**, rather than
merely accumulate. In this skill, integration means a reasoned suggestion, not automatic
changes to your work or memory.

This is our naming metaphor, not a definitive comparison of fictional martial arts or
their different editions. This is an independent project, not an official Jin Yong product.
You do not need to know wuxia to use it.

## Deliberately small

Two runtime files. No bundled service, scraper, database, API key, or telemetry code.
Beiming uses the model and tools already available in your Codex session.

- It cannot guarantee access to every link or read all your previous conversations.
- Unreadable images and inaccessible pages should be reported, not guessed.
- “Worth retaining” does not save anything. No automatic memory, project, or rule changes.
- Platform data handling still applies; this is not an offline or no-upload guarantee.
- Other agents and plugin-marketplace installation are not claimed as tested.

## Improve it with real examples

See [validation notes](VALIDATION.md) for the tested scope and remaining limits.

Open an issue or pull request with a shareable input, the context you supplied, the
actual response, and what was missed. Remove private information first.
Small improvements backed by observed behavior are more useful than longer instructions.

## License

[MIT](LICENSE). The project instructions and original examples are reusable under that license;
third-party articles, artwork, characters, and other referenced material are not relicensed.
