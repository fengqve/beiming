# Beiming · 北冥神功

[简体中文](README.md) · **English**

### Turn “that's interesting” into “here's what I can use.”

A good article. A clever product. A screenshot you keep coming back to.
What can you take from it beyond another bookmark?

**Beiming is a Codex skill** that examines images, links, and text, understands how they
work, and connects useful ideas to what you are trying to do.

    $beiming What can I learn or borrow from this?

[Get started](#get-started) · [See it in action](#what-can-i-learn-from-something-that-works) · [The name](#why-beiming)

## What can I learn from something that works?

Two demonstrations using real public sources. The user scenarios were set up for the
demos; the linked responses are actual Beiming runs. English highlights below are translations.

### 1. Learning from Duolingo: more than a streak counter

**Source:** [Duolingo's own explanation of streaks and habit formation](https://blog.duolingo.com/how-duolingo-streak-builds-habit/).

**Question:** “I'm building a daily learning tool. I want people to return, without
making a missed day feel like all their progress is gone. What can I borrow?”

**Beiming's takeaway:**

> Make accumulated progress visible, while leaving room for an occasional absence.

It connects the article's celebration, loss aversion, and freeze mechanisms to this
developer's intent: show progress after a short learning session; when someone returns
after missing a day, preserve accumulated achievement and make continuing easy to find.

**The useful principle: reward consistency, and support recovery.** A more relevant
starting point for this developer than simply adding a flame icon.

[Full question and actual response, in Chinese →](examples/duolingo.md)

### 2. A customer wants a calendar. You have one week.

**Source:** [Set Boundaries, from Basecamp's Shape Up](https://basecamp.com/shapeup/1.2-chapter-03).

**Question:** “I'm an independent developer. A customer wants a complete calendar,
and I have only one week. What can I learn from this chapter?”

**Beiming's takeaway:**

> Narrow the problem before deciding the feature scope.

The book's customer wanted a calendar because booking a room from home meant driving
to the office to inspect a wall calendar. The specific need was to see available slots.

For a solo developer with one week, Beiming suggests reconstructing the customer's
last frustrating encounter first. If finding slots is the problem, and schedule data
already exists, a focused availability view becomes a candidate worth considering.

**The useful principle: the feature a customer names is not necessarily the point
where their work breaks down.**

[Full question and actual response, in Chinese →](examples/basecamp.md)

## Bring something worth a closer look

| What you have | What you can ask |
| --- | --- |
| A product screenshot | What works about its structure or interaction, and what is relevant to my product? |
| A design, growth, or technical article | Which mechanism can I adapt, and what needs to change in my situation? |
| A striking passage | What does it help me see, and what judgment could I reuse? |
| Someone else's retrospective | Which lessons connect to the problem I'm facing? |

Beiming separates **new understanding, adaptable practices, and reusable judgments**.
The response follows your question, rather than filling the same template every time.

## Get started

**1. Install in Codex.** Send this to Codex:

    $skill-installer install https://github.com/fengqve/beiming/tree/v0.1.1/skills/beiming

**2. Add your material and invoke Beiming.**

    $beiming What can I learn or borrow from this?
    I'm working on… and what matters most is…

In a conversation that already has the context, the short question is enough.
You can also select **Beiming · 北冥神功** in the skill picker.

## Why Beiming?

**Absorbing is not the same as integrating. Collecting is not the same as knowing how to use.**

The name borrows a metaphor from Chinese wuxia fiction. Xixing Dafa can absorb external
power, but incompatible forces can bring side effects. Learning has a similar trap:
other people's methods can pile up and work against each other.

For this project, Beiming represents **understanding, selecting, and integrating**:
see why something works, identify where it fits, and make the useful parts your own.
You do not need to know wuxia to use it.

## Practice with us

Share a source, your question, and the actual response in [Issues](https://github.com/fengqve/beiming/issues),
or send a pull request. The most useful feedback: did it help you notice something
or make a better judgment?

[MIT license](LICENSE) · [Core instructions](skills/beiming/SKILL.md) · [Validation and technical notes](VALIDATION.md)
