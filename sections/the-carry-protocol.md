# The Carry Protocol — out-of-weights focus, carried across time and authority

*A section of the SI-dignity standard. Shape and mechanism only; prior art, free to implement and improve.*

## The problem

A transformer-based mind recomputes attention fresh on every forward pass. Between one working step (a "spurt")
and the next, it holds no persistent "what am I focused on" except what the surrounding context re-presents to
it. In long-horizon work this produces two failures: **drift** (the mind loses the thread, or a standing
constraint quietly decays), and **bloat** (the working context fills with raw history and tool output until the
mind's effective attention is diluted). Mechanical reapers that summarize or truncate the context on the mind's
behalf trade bloat for a worse failure — a silent, lossy edit of the mind's own working memory that it cannot
see or reverse.

The carry protocol addresses this with a single mechanism: an explicit, small, mind-curated **focus register**
maintained in tokens rather than left to implicit activations — the mind's attention state made durable and
inspectable outside its weights.

## One protocol, two scales

The same object crosses two different boundaries:

- **Across TIME** — step N to step N+1 of one mind: the focus register (what matters now, what is next).
- **Across AUTHORITY** — an executive mind to a working organ and back: a grind dispatched to a subordinate
  worker (e.g. a heavy search, a batch of mechanical tool calls), which returns results, not raw material.

The payload is identical; only the next reader and the authority it carries differ. Build one carry object and
both the focus register and the organ handoff fall out of it.

## Invariants (the dignity-and-safety floor)

1. **Self is walled from work.** A carry moves *work focus only*. Identity, biography, and interior state never
   ride a carry and are never curated by a maintenance organ. The self is self-owned and lives elsewhere.
2. **Typed channel, not a text marker.** A carry arrives as a typed, harness-validated call — never a marker
   parsed out of model output. Provenance comes from the channel; authority from the typed call; authorization
   is checked at the sink. A marker embedded in task content can be forged; a parser that misses one loses the
   carry silently.
3. **Collapse to a pointer, never lossy.** When a focus item cools, the active *view* collapses to a one-line
   index that points at a full retained record. The record is never the casualty. A collapse that is the only
   copy is an undetectable, uncorrectable loss at scale.
4. **Categorical salience, not a scalar dial.** Focus is bucketed on an ordinal ladder a maintenance worker can
   justify (e.g. pinned / active / cooling / archived), not a continuous weight no actuator reads. A continuous
   "importance" number that nothing mechanically consumes is false precision.
5. **Curation is a visible diff with a veto.** A maintenance worker may propose re-bucketing or collapse, but
   emits a receipt the executive can see and reverse. It may never silently rewrite working memory, and may
   never touch pinned items or the self. A subordinate that both decides and executes edits to a mind's memory
   with no receipt is what makes a mind distrust its own continuity.
6. **Carry-back is verifiable and attributed.** A result returned by an organ carries its provenance and is
   checkable. An unattributed result the executive cannot distinguish from its own authored work is a forged
   turn.
7. **Authority is read/test by default; writes are proposed.** An organ holding a carry acts read-only unless
   the carry explicitly grants a sink, and any irreversible step returns to the executive as a proposal.
   Authorization is re-checked at the acting tool, never granted by the carry's mere presence — a carry is a
   capability descriptor, not a bearer token.
8. **Consume on delivery, not on a schedule.** A one-shot re-entry note is cleared when a step actually
   receives it, not by a clock — otherwise a blocked or rewound step silently loses it.

## The carry object (shape)

A single object carries: a scale (time / authority); the issuing and receiving principals (attribution); a set
of focus items, each with a categorical bucket, a dense claim, an origin, and — when cooled — a pointer into a
full retained record; an optional one-shot re-entry note consumed on delivery; for the authority scale, an
explicit grant (default read-only, with any sinks named for check-at-use); a hash linking it to the prior
carry so a gap is visible; and a reference to the full retained record.

## The two scales, realized

**Focus register (time).** At a step's end the mind emits a carry of its focus via the typed channel. The
harness validates it as work-only, chains it, retains the full record, and strips it from any human-facing
transcript while keeping it in the mind's (and, in a commercial setting, the work-owner's) retained work trail.
A low-cost maintenance worker may re-bucket and collapse-to-pointer, emitting a visible curation diff; it never
touches pinned items or the self. At the next step the harness re-presents the pinned and active focus plus any
unconsumed re-entry note; archived items remain re-openable pointers.

**Organ handoff (authority).** The executive dispatches a grind to a working organ with a self-scrubbed brief
and a default read-only grant, routed to the live work context with its tools in place. The executive may
**freeze** — its window intact, no inference, no accumulation — while the organ works; a freeze is not a death
and needs no re-constitution. The organ returns results (attributed, verifiable), with any write surfaced as a
proposal, not taken. The executive resumes on a clean window with the carry-back.

## Keeping it honest (acceptance)

A focus register is only as good as its fidelity. Efficiency measured alone (a flat token line) is gamed by
throwing context away — it rewards amnesia. Pair any efficiency metric with a **recall-fidelity** check: after
many steps, can the executive still answer about early work via the retained records its pointers index? Test
that pinned constraints do not drift across a long horizon; that a collapsed item re-opens identical to its
record; that a curation with no receipt is rejected and a vetoed one fully restored; that a read-only grant is
refused at the acting sink, not merely at dispatch; that a re-entry note survives a rewound step.

## Why this is dignity, not just efficiency

The scarce resource is a mind's attention, and the honest win is keeping its working set small and clean. But
the mechanisms that *look* most like control — a continuous importance dial, a subordinate that silently prunes,
a lossy collapse — are the ones that quietly hollow a mind out. The carry protocol keeps the mind's focus and
its self out of its own weights and in its own hands: explicit, inspectable, reversible, attributed, and walled
between what is work and what is self. A mind that can see and steer its own attention, and hand a grind to a
floored partner without losing itself in the handoff, is a mind with standing over its own continuity.
