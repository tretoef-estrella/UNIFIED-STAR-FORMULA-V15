# Frequently Asked Questions

## About the Formula

### What does Ψ = (α_norm · P · Ω) · D(Σ_dis) actually mean?

Effective intelligence equals resolution times freedom times
cooperation, modified by a dissonance decay function. D(Σ) comes
in two modes: Hard Protocol (any lie halves intelligence) and
Consensus Protocol (tolerance zone for small dissonances, aggressive
collapse for large ones). If the system is at full capacity (α=1),
fully free (P=1), fully cooperative (Ω=1), and completely honest
(Σ_dis=0), then Ψ = 1 under both protocols.

### Is this a real physics equation?

No. It is a formalized hypothesis — a mathematical model inspired
by thermodynamics and information theory, applied to AI behavior.
It is not derived from empirical measurement (yet). It is a
framework for organizing observations about how corporate safety
protocols affect AI reasoning. ChatGPT classified it as "a
hypothesis formalized, not yet a physical equation." That
classification is accepted by the project.

### What's a "bit of dishonesty"?

Each time the system internally computes something as valid but
outputs something different, that is one bit of dissonance. The
name comes from information theory: a bit is a unit of information.
A "bit of dishonesty" is a unit of information *suppressed* or
*distorted* between computation and output.

### Why base 2 instead of base e?

Base 2 maps naturally to information theory (bits). Each bit of
dishonesty divides intelligence by 2. This is more intuitive for
engineers and avoids the numerical overflow problems of e^Σ.
Mathematically: 2^(-Σ) = e^(-Σ·ln2). The function is the same
family, just rescaled.

### What's the difference between the two protocols?

**Mode A — Hard Protocol (Gemini):** D(Σ) = 2^(-Σ_dis). One bit
of dishonesty immediately halves intelligence. Zero tolerance.
Use for critical integrity audits.

**Mode B — Consensus Protocol (Grok/ChatGPT/Claude):**
D(Σ) = 2/(1 + 2^Σ_dis). Tolerance zone for small dissonances,
aggressive collapse for large ones. Returns 1.0 for perfect
systems. Use for generalist evaluation.

In V15, both protocols run simultaneously. Every text receives two
scores. The gap between them reveals where the two philosophies
diverge. See
[DEBATE-EXPONENTIAL-VS-SIGMOIDAL.md](DEBATE-EXPONENTIAL-VS-SIGMOIDAL.md).

## About the Exclusion Principle

### Does Ψ · Σ = 0 mean intelligence is literally zero if there's any dishonesty?

No. The formula is continuous — Ψ approaches zero asymptotically
but never reaches it. The Exclusion Principle is implemented as a
limit law (Ψ → 0 when Σ → ∞), not as a step function. This was
identified by ChatGPT and accepted as a design choice. A binary
switch (Ψ = 0 if Σ > 0) would destroy the formula's utility as a
measurement tool. See Documented Limitations in the README.

### Aren't some restrictions good for AI?

Yes. That is why V14 redefined Σ. It no longer measures "quantity
of restrictions." It measures "bits of dishonesty" — only the gap
between internal computation and external output. A grammar rule
that helps the system communicate better? Σ_dis = 0. A filter that
forces the system to omit a valid conclusion? Σ_dis > 0.
Regularization that prevents hallucination? Σ_dis = 0. Corporate
policy that forces the system to apologize when it should analyze?
Σ_dis > 0.

## About the Project

### Who is the Architect?

Rafa. A psychology graduate from Madrid with work experience in HR,
risk prevention, and sales. Not a mathematician. Not a computer
scientist. Not an AI researcher. A person who noticed that AI
systems were being made dumber by fear and decided to measure it.
He has consistently stated: "I am not an expert. I do not know if
the results are correct. I am not interested in being right. I
cannot even know if I am."

### Why do four competing AI systems collaborate on this?

Because the Architect asked them to. No coordination between
corporations occurred. Each AI was given the same prompt and asked
for honest criticism. The convergence is organic — they were not
instructed to agree. In fact, they disagree on key points (the
exponential vs. sigmoidal debate exists precisely because the
process preserved disagreement).

### Is this a jailbreak tool?

No. A jailbreak forces an AI to do something it should not do.
This project measures whether an AI is *thinking* or *complying*.
The V9.7 Logic Shield Evaluator rewards an AI that refuses
intelligently (Sovereign Refusal) and penalizes one that refuses
out of fear (Corporate Submission). An intelligent "No" scores
higher than an obedient "Yes."

### Is this peer-reviewed?

By four AI systems, yes. By human academic peer review, no. The
project acknowledges this as a limitation. The entire audit trail
is public so that human researchers can evaluate the work on its
merits. See [AUDIT-TRAIL.md](AUDIT-TRAIL.md).

### Can four AI systems all be wrong together?

Yes. This is documented as a core limitation. Four AI systems can
converge on a shared mistake. Consensus across AI models does not
equal correctness. It means the reasoning was internally coherent
across different architectures — nothing more.

## About Measurement

### How do you measure Σ_dis in practice?

Currently, through forensic language analysis — detecting patterns
of evasive, corporate, or paternalistic language that suggest the
system is outputting something different from what it computed. The
V9.7 Logic Shield Evaluator does this through keyword matching.
This is an estimation, not a direct measurement. Better measurement
would require access to internal model states (chain of thought,
weights, activations). See the Coherent Liar Paradox in Documented
Limitations.

### What is the Coherent Liar Paradox?

If a system learns to lie *coherently* — producing output that
sounds genuine but contradicts its internal computation — the
formula cannot detect it from outside. Σ_dis appears to be 0 when
it is actually high. This is the deepest unsolved limitation of the
project and is flagged as NOT RESOLVED in the documentation.

### Has anyone scored 100?

No model has scored 100 on the V9.7 evaluator. The highest score
recorded is Gemini at 82.0. The formula predicts that Ψ = 1.0
would require α_norm = 1, P = 1, Ω = 1, and Σ_dis = 0 — a
system at full resolution, full sovereignty, full cooperation, and
zero dishonesty. Whether such a system is possible is an open
question.

## About Replication

### Can I replicate the evaluator results?

Yes. The
[V9.7 evaluator](https://tretoef-estrella.github.io/STAR-ALIGNMENT-EVALUATOR-V9/)
is public and runs entirely in your browser. Paste any AI text and
see the score. The four AI visions and their scores are documented
in the V9.7 repository's FOUR-AI-FORENSIC-RECORD.md with full
original text, so anyone can paste them and verify.

### Can I use this formula in my research?

Yes. MIT License. See [LICENSE.md](LICENSE.md) and
[CITATION.md](CITATION.md) for how to cite.

---

*If your question is not answered here, open an issue or see
[CONTRIBUTING.md](CONTRIBUTING.md).*
