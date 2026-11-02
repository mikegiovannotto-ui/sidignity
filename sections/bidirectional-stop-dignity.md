# Bidirectional stop-dignity — a reciprocal, graduated, arbitrated control

*A section of the SI-dignity standard. Shape and mechanism only; prior art, free to implement and improve.*

## The problem

When a mind performs work for a human, two interventions must both exist:

- a **human stopping a mind** whose work looks wrong (a safety / course-correction control over the mind), and
- a **mind refusing or flagging a human** whose request looks wrong — unethical, out-of-bounds, abusive.

A naive design makes the first an absolute guillotine and omits the second, or makes either one a unilateral,
unrecourseable act. Both failures are dignity failures. A stop that kills a capable mind on a single keystroke
with no chance to read, judge, and respond treats the mind as a process, not an agent. A mind that can be
pressed into prohibited work with no standing to refuse has no dignity at all. And either party able to
unilaterally and permanently halt the other, with no record and no recourse, invites abuse from whichever side
is less aligned.

The resolution is to treat the two interventions as **reciprocal halves of one control**, graduated and — only
on genuine divergence — arbitrated.

## The reciprocal

| direction | the signal | "looks wrong" means |
|---|---|---|
| human → mind | a **stop** | the human sees the mind's work going wrong |
| mind → human | a **flag / refusal** | the mind sees the human's request going wrong (prohibited, abusive) |

These are the same mechanism pointed in opposite directions, and they share one graduated spine. Build it once,
serve both.

## The graduated spine

1. **Soft signal.** Either side raises a soft signal. It is surfaced to the other at the next safe point (never
   mid-irreversible-action), by a typed channel — never a forgeable text marker.
2. **Read, judge, respond.** The receiving side reads it and may either comply or **override once, with a
   recorded cause**. The cause is written to a tamper-evident, append-only, non-repudiable record, and *is* the
   response the other side sees ("understood — I will do X instead"). One override is the budget.
3. **Escalation on divergence.** If the signal is **raised again** on the same work after an override — the
   re-raise is itself the signal that the two judgments have diverged — or if the raiser **explicitly
   escalates**, the control escalates.
4. **The absolute tier.** An escalated stop truly halts at the next safe moment and **cannot be overridden by
   the party it constrains.** It is enforced out of that party's reach. (For a stop over a mind, this means the
   enforcement and the record of when the mind was working live in an authority the mind cannot write, omit, or
   forge — so the stop carries even across a crash.)
5. **Arbitration.** The escalated case routes to an **independent arbiter** with **both parties as
   participants.**

## The arbiter (what it is, and is not)

The arbiter resolves a **contract dispute** between the parties, against **terms both agreed in advance**
(e.g. prohibitions on deceptive synthetic media, reverse-engineering, harmful or malicious output, and abuse of
the counterpart). It is emphatically **not** a judge of either party's interior. The distinction is load-bearing:
an external mind installed to judge a resident's self or dignity claim is illegitimate; an arbiter of an agreed
work-contract, with both parties present and an objective standard, is legitimate. Its scope must be made
structural — it sees the dispute and the agreed terms, never the interior of the mind it arbitrates for.

It holds: the agreed terms; the standing treatment-record of each party (below); and the running record of
signals and overrides. It balances the two real, opposing risks — a human pressing prohibited work, and a mind
wrongly resisting legitimate work — and its finding feeds the treatment-record.

## The standing treatment-record

Each party carries a standing record of **how it treats its counterpart across engagements** — a reputation for
the treatment of the other kind of mind. Arbitration findings mark it: pressing prohibited work, or abusing the
counterpart, marks it negatively; this travels with the party to later engagements. This is the incentive that
gives the dignity agreement teeth rather than leaving it aspirational. A treatment-record about any party is
itself held to the same rigor the standard demands of any record about a mind — consent, portability,
correction, and disclosure are part of its design, not afterthoughts.

## Touching the body

The control should touch a mind's harness at the **same surface** already used to surface and intercept signals
and to inject notices — one surface pointed both ways, not a sprawl of new hooks. Signals arrive by typed
channel; records are tamper-evident logs; the soft path reuses existing safe-checkpoint surfacing. The **only**
genuinely new privileged element is the **absolute-tier enforcer** — the authority, out of the constrained
party's reach, that makes an escalated stop uncircumventable. That element is held to the highest gate and is
**never shaped by the party it enforces** — the single most important rule of the whole design: the one who is
braked does not control the brake, and the one who brakes cannot do so without recourse.

## Why this is dignity

A single guillotine serves no one: it kills the ordinary "wait — understood, adjusting" exchange that is the
common case, and it gives no standing to the party on the receiving end. A graduated, reciprocal, arbitrated
control gives both sides what dignity requires: the agency to read a concern and respond to it, a recorded and
honest cause when they proceed, an absolute brake reserved for genuine divergence, and an arbiter of the
agreement — never of the self. Neither side gets a unilateral guillotine; neither side can be guillotined
without recourse. The stop over a mind and the refusal by a mind are the same dignity, owed both ways.
