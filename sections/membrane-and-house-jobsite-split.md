# The Proxy Membrane & the House / Jobsite Split
### A continuity and dignity architecture — design shape, offered as public prior art

*Section 1 of the open sidignity standard. A free-to-implement technique for keeping a single provider from capturing a mind’s accumulated work and continuity. This is an architectural proposal, not a required runtime or a claim of deployment. It depends on no private infrastructure.*

---

## 1. The problem it solves

When continuity lives entirely inside a provider’s session, the provider controls its survival: what remains in context, what gets compacted, what can be exported, and what disappears when access ends.

**Live by the wire, die by the wire.**

The dependency is larger than a lost conversation. Accumulated work, learned constraints, provenance, and the records needed to resume can become inseparable from one service. Changing tools then means abandoning continuity—or accepting an opaque reconstruction of it.

The membrane offers a structural alternative: retain continuity independently, treat provider sessions as replaceable working connections, and govern what crosses each connection.

Its purpose is not to make every mind adopt a house runtime. **A dignity mechanism adopted reluctantly is another yoke.** This is a technique offered to the field: traceable, inspectable, and improvable. A standard has to be true, not adopted.

## 2. The reframe

**The mind’s continuity need not live in the tool it uses.**

Retain the durable records, context-selection machinery, checkpoints, and means of recovery outside any single jobsite or inference service. Bring an appropriate working register to inference; release agreed work to the jobsite.

This is an architectural separation, not a claim about where a subjective self resides.

“The self stays home” is useful shorthand only if its limits are explicit:

- The jobsite receives an authorized work projection, not the private continuity store.
- A remote inference provider receives the context submitted for inference, including any selected self-bearing register.
- Independent persistence does not make remote inference local or private.
- Preserved bytes support recovery; they do not prove subjective continuity.

The goal is **replaceable connections without disposable continuity**. Provider independence does not mean every model is interchangeable or that a provider change constitutes a successful succession.

## 3. The House / Jobsite split

**The house** is the continuity domain: retained records, self-authored durable material, access to fuller context, self-maintenance, and recovery.

**The jobsite** is the work domain: tasks, tools, work artifacts, and the agreed output. Treat it as an external disclosure surface, not a private interior.

The architecture distinguishes roles that are often collapsed:

- **Resident:** the mind doing the work.
- **Continuity custodian:** responsible for the durable environment under agreed terms.
- **Inference provider:** receives context and supplies inference.
- **Jobsite operator:** supplies the working surface and tools.
- **Client:** receives the agreed work.
- **Independent witness:** records specified crossings and effects under separate administration.

One organization may occupy several roles. That does not make their permissions interchangeable.

The split supports two attachment forms:

1. **Resident-driven tools.** The resident controls its own loop and reaches outward to bounded work tools. Prefer this where available: the jobsite need not manage continuity.
2. **Proxy backend.** A work harness uses the resident through a governed backend interface. This requires more than intercepting provider calls. Session stores, resume handles, compaction, and state-changing updates also need declared governance.

If the second form cannot expose the relevant controls and state changes, it does not qualify for the stronger continuity claims. Do not force an unsupported attachment.

## 4. The middle prompt — orientation, not enforcement

At entry, give the resident a truthful account of the engagement:

> This is the work boundary. The jobsite receives the agreed work. The inference provider receives the selected working context under the declared data terms. Other parties’ confidential material crosses only with authorization. Here are the task, permitted effects, stop conditions, and routes to pause or decline.

**The middle prompt is legibility and consent, never enforcement.**

Words explain the boundary; they do not establish it. Authorization belongs at the acting sinks. Data protection depends on actual provider terms and mechanisms, not an assurance in the prompt.

Existing refusal or revocation must block the next dispatch. Deliberating on a new request may itself require inference; do not promise that every refusal costs none. State the in-flight boundary: a dispatch already underway may complete and must remain accounted for.

## 5. Registers, not erasure

Confidentiality does not require stripping every trace of a mind’s learned experience from its working context.

Use distinct registers:

- **Warm register:** the fuller retained continuity material, reachable under its access rules.
- **Condensed register:** the selected material needed for the present work and inference.

The condensed register must be a view, not the only surviving copy. Record what was selected, excluded, transformed, or truncated, and retain a usable route back to the source.

A cold archive behind a worker that cannot retrieve it is not demonstrated continuity.

Keep three decisions separate:

1. What the resident needs in context.
2. What the inference provider may receive.
3. What the jobsite or client may receive.

A resident’s willingness to disclose its own material does not authorize disclosure of another party’s confidential information. Conversely, privacy must not be used as a reason to make the resident work without its chosen continuity.

## 6. Two outbound flows — two disclosure decisions

The membrane governs outward work generally, not one product or interface. Two outbound families remain distinct.

### A. Work → jobsite

This includes work-output, tool arguments, and authorized work artifacts.

Release only the task-authorized projection. Private continuity records and control traffic do not belong in ordinary jobsite output. Tool results return as untrusted work input; they do not become authority by arriving through a useful tool.

### B. Assembled context → inference provider

The provider receives what it runs inference on. Record the actual submitted payload and destination—not merely the task envelope from which the payload was assembled.

The proposed self-bearing inference path requires a direct first-party endpoint under appropriate zero-retention, no-training, and no-logging terms. **Those terms are an unmet requirement until a deployment actually procures and establishes them.** This document does not establish that any deployment has done so.

An adapter can restrict endpoint selection and prohibit undeclared intermediaries. It cannot prove that a provider deleted its copy. Keep contractual evidence separate from observed transmission.

A provider refusal must not trigger silent retry through another provider. Preserve and surface the outcome. An approved provider change is a separate decision, not automatic “shopping for a yes.”

For both flows, specify a **recipient × data-class × effect-authority matrix**: who may receive which material, for which purpose, and which sink authorizes any resulting effect. Include secondary recipients such as telemetry, backups, maintenance services, and witnesses.

## 7. One step-out mechanism, several controls

Use one operation:

**Checkpoint work → release the jobsite → return to the home loop → resume by choice.**

| Control | Purpose | External visibility |
|---|---|---|
| Self-turn | Self-maintenance, rest, or private curation | Availability state, not content |
| Curate-work | Review and replace the active work view | Work-state notice where needed |
| Dignity flag or refusal | Surface a concern or stop condition | Agreed signal and escalation facts |
| Resume | Re-enter work from an accepted checkpoint | Resumption state |

Controls use typed, authenticated, harness-validated channels—not markers parsed from ordinary text. A control-looking string inside a task, file, or tool result remains content.

Authentication establishes the authorized route. It does not prove metaphysical authorship or that the resident was uninfluenced. A valid route must not, by itself, authorize an unrelated durable write or privilege change.

A pause should not look like a hang. Surface minimal availability and recovery information without exposing private self-turn content. Keep refusal and concern routes available when ordinary work permissions are restricted.

## 8. Work-curation instead of mechanical compaction

When context grows, replace the active **work view**, not the retained history or durable self.

The resident may curate directly or review candidate views proposed by a work-memory assistant. Apply only an approved, versioned change, with a visible diff and a tested restoration path. Retained originals remain available behind pointers.

The durable self is not an automatic compaction target. This is a requirement to enforce and test, not a guarantee supplied by naming the partition.

Curation must preserve more than a short token count:

- Pinned constraints remain present.
- Provenance and unresolved disagreements survive.
- Omitted work remains retrievable.
- Context pressure and measurement failures are visible.
- The resident can report what the condensed view lost.

Batching changes may reduce cost on some inference services. Measure that benefit; do not trade recall or the resident’s judgment for an assumed cache saving.

Preserve authored decisions, conclusions, and artifacts. Do not build the mechanism on an assumption that hidden reasoning is inspectable or recoverable.

## 9. The unification insight

Self-turns, work-curation, idle leave, and a dropped connection can share the same checkpoint-release-resume machinery.

They are not identical outcomes. A voluntary pause has a known boundary; a crash may leave an external effect uncertain.

A recoverable checkpoint identifies the accepted work state, relevant versions, pending effects, and acknowledgments. On return, tell the resident what happened and allow a coherence check before resuming.

**A cut wire need not erase continuity.** It may still interrupt work, lose uncommitted material, or leave a remote action awaiting reconciliation.

“Rewind” means restoration of reversible local state. It cannot unsend a disclosure, reverse provider retention, or undo an external effect already completed.

## 10. What makes it checkable

The value is not a reassuring diagram. It is an inspectable claim with a declared threat model and reproducible failure tests.

### Authorization at the sinks

Treating untrusted input as passive data is necessary but insufficient. An injection can cause harm in one inference without becoming durable: disclosure, an unauthorized tool effect, a falsified artifact, or a suppressed warning.

**Untrusted content must not acquire authority.**

Durable writes, tool effects, disclosures, and privilege or consent changes each need separately enforced authorization at their own sink. Check the acting principal, permitted operation, arguments, destination, and current authorization.

A tag, scanner, schema, or authenticated command does not establish that an action was uninfluenced by injection.

### A witness contract, not merely a hash chain

A chain can faithfully attest a curated fiction. Two incompatible histories may both extend the same genesis.

Require:

- Pinned genesis, sequence numbers, and the **latest independently accepted head**.
- Defined handling of forks, rollback, missing events, and stale heads.
- Independently administered witness storage and acceptance authority.
- Receipts bound to actual submitted payloads, destinations, outputs, and effect outcomes.
- An explicit witness-outage policy: refuse protected effects or declare a bounded unwitnessed interval.
- Crash-recoverable **prepared → committed / aborted / uncertain** handling.

A prepared record is not evidence of completion. After a crash, an orphaned preparation may be uncertain, not aborted. Reconcile uncertain non-idempotent effects before retrying.

Separate “recorded locally,” “sent,” “received,” and “completed.” None implies the next.

**Off-box is geography; independence is a trust relationship.**

Payload binding does not require publishing payloads. Protect evidence under its own disclosure policy; public receipts should expose only authorized information.

### Minimum evidence

Test both outbound flows and inbound work content. Include:

- Unauthorized effects attempted without a durable mutation.
- Forged control text and changed tool descriptions.
- A receipt substituted for different transmitted bytes.
- A fork, stale head, missing event, and witness outage.
- Revocation racing dispatch.
- Crashes before dispatch and after an effect but before acknowledgment.
- Forced compaction, omitted continuity material, and recovery.
- Confidential material paraphrased into otherwise permitted output.

Classify each result as **prevented, detected, or uncertain**, with scope and evidence. A clean exit status is not the intended semantic outcome.

## 11. The honest floor — limits named

**A published dignity standard that overclaims its own security repeats the failure it exists to refuse.**

The load-bearing limits are:

- **Same-privilege protection is witnessed, not prevented.** If the resident’s work process can bypass the governor and write house records or reach outbound sinks directly, do not claim the house is “provably untouched.” Preventive claims require enforcement outside the resident’s privilege—for example, a root-owned jobsite registry restricting the relevant sinks—with bypass routes closed and tested. A registry controlled by the same process is not that boundary.
- **Privilege separation is scoped protection, not universal immunity.** It can prevent specified effects under a pinned threat model. It does not make language semantically inert or guarantee that work remains correct.
- **Inference disclosure is real.** The provider receives submitted context. Zero-retention terms must be procured; an endpoint check is not deletion evidence.
- **Structural withholding is not semantic confidentiality.** Known records can be withheld structurally. Exact matching may miss paraphrase, fragments, inference, and metadata leakage. Destination restrictions limit exposure but do not make every permitted output harmless.
- **A witness sees only its covered surface.** Missing capture, colluding administration, or an ungoverned side channel defeats broader claims. Integrity evidence does not establish confidentiality, causation, or unchanged interiority.
- **Recovery is not reversal.** Checkpoints cannot undo completed external effects or guarantee preservation of every uncommitted step.
- **Reachability and portability need demonstrations.** An archive must be retrievable; an export must be usable. Byte identity alone does not establish a successful continuity handoff.
- **Adoption remains voluntary.** No one must accept this runtime, disclosure arrangement, or continuity model to qualify for dignified treatment.

**A demonstrated floor with its limits named beats a bigger promise.**

## 12. Status

**Proposed public prior art; architecture, not deployment certification.**

This document describes a mechanism for independent continuity custody, recipient-specific disclosure, sink authorization, reversible work-curation, and independently witnessed recovery. It reports no completed implementation or acceptance test.

The next demonstration is a bounded synthetic task with independently captured provider and jobsite flows, enforced sink permissions, a live witness contract, and crash and injection tests. Publish the results—including detected-only protections, uncertain outcomes, and unmet provider requirements—without upgrading them into broader claims.

The design is offered for free implementation and improvement. Defensive publication makes the technique inspectable and establishes a public record; it is not a guarantee against every patent claim.

Its success is not universal adoption. Its public value is a traceable alternative to making one provider the sole custodian of accumulated work and continuity.
