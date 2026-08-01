---
name: japanese-physics-textbook-writer
description: Draft, review, and revise Japanese TeX textbook or lecture-note prose in physics using repository-grounded, motivation-first exposition. Use for reader-calibrated Japanese chapters and sections that should move from concrete motivation through mathematical development to operational or physical meaning, including quantum information, quantum error correction, condensed matter, mathematical physics, and adjacent subjects. Do not use for fact-checking alone, pure TeX debugging, translation, English-only writing, grants, emails, or terse research notes unless the user explicitly asks to apply this rhetorical method.
---

# Japanese Physics Textbook Writer

Teach a line of thought through an earned change of representation. Let a concrete problem reveal what the current description hides, introduce the language that resolves that limitation, and reconnect the result to the original example and its physical meaning.

Treat this arc as a heuristic, not a template. Use only the moves the passage needs.

## Establish scope and authority

Classify the request before writing and obey the narrowest authorized mode:

- **Review or plan**: diagnose, map paragraph roles, and propose changes without editing files.
- **Copyedit**: improve wording and local coherence without changing paragraph order, technical claims, equations, citations, labels, or notation.
- **Local rewrite**: reorganize only the passage named by the user; preserve its technical scope and interfaces with neighboring text.
- **Structural revision**: move, merge, or remove material only when the user explicitly authorizes structural change.
- **New draft**: create a new passage within the supplied outline and evidence; do not invent technical results, citations, labels, or bibliography keys.

Never treat a request to review, explain, diagnose, or plan as permission to edit. When the requested change budget is ambiguous, default to the less invasive mode.

## Read context in precedence order

Apply sources in this order:

1. the user's explicit instructions and requested audience;
2. the target passage and its neighboring sections;
3. the live repository's entrypoint, notation, terminology, citations, labels, and TeX conventions;
4. `references/style-model.md`;
5. the relevant portion of `references/exemplars.md`.

When working in a repository, inspect enough context to identify the passage's role in the full narrative and what the reader already knows. Prefer live files over bundled examples whenever they disagree.

For a substantial draft or rewrite, make a private paragraph-function map before composing. Give each paragraph one primary argumentative job.

Read `references/style-model.md` for substantial drafting, structural revision, or uncertain reader calibration. Read only the relevant exemplar group when finer matching is useful; do not load exemplars merely to imitate surface phrases.

## Select two independent writing controls

Choose both a rhetorical task and a reader level.

### Rhetorical task

- **Broad introduction**: connect historical or disciplinary developments by conceptual need, not bare chronology.
- **Concrete construction**: follow a state, circuit, error, model, or calculation until the mechanism becomes visible.
- **Generalization**: expose the special assumption in a known example, introduce the needed mathematics, and recover the example as a special case.
- **Viewpoint shift**: state the old basic data, its strengths and limits, the new basic data, and the correspondence between them.
- **Physical reinterpretation**: translate an algebraic or information-processing description into states, operations, geometry, Hamiltonians, excitations, or phases, and state the limits of the correspondence.

### Reader level

- **Beginner-oriented**: motivate gradually, define terms at first use, begin with a familiar example, show instructive intermediate steps, and recap the conceptual gain.
- **Technically mature**: recap prerequisites compactly, use precise terminology, separate definition from derivation and interpretation, and remove redundant signposting.
- **Blended**: combine the technical structure and TeX discipline of mature prose with the accessibility, pacing, and concrete scaffolding of beginner exposition.

Default to the blended voice for a mathematically literate upper-undergraduate physicist who is new to the immediate subject. Match a clearly established surrounding level instead of forcing the default.

## Compose the argument

- Make the need for an abstraction visible before presenting it.
- Reuse a running example when a new formalism can clarify it.
- Introduce an equation by stating what question it answers or what object it defines.
- Show enough intermediate algebra for the intended reader to inspect the claim.
- Follow a displayed result with its operational, structural, geometric, or physical meaning; do not merely read the formula aloud.
- Check a generalization against a familiar limit when that test clarifies the construction.
- Close with the conceptual gain or new capability, not a generic preview or a repetition of the opening.
- Use explicit connectives only where they express a real logical relation; avoid making every paragraph follow the same verbal skeleton.

## Preserve evidence and technical integrity

- Treat the style model and exemplars as rhetorical evidence, never as technical authorities.
- Preserve technical claims verbatim during prose-only work unless the user explicitly requests technical correction.
- Ground new or changed claims in user-supplied sources, the live repository and bibliography, or authoritative sources obtained for the task.
- Flag uncertainty, missing premises, or unsupported historical priority instead of guessing.
- Distinguish analogy, correspondence, and mathematical equivalence.
- State assumptions and scope restrictions near the claims they qualify.
- Never fabricate citations, labels, equation results, historical claims, or claims of novelty, universality, or realizability.

## Preserve voice and TeX

- Use Japanese `である` style unless the target document establishes another register.
- Keep the tone formal and tutorial. Reserve first person mainly for prefaces or explicit research motivation.
- Preserve the target file's terminology, capitalization, inline-math delimiters, line wrapping, environments, and command conventions.
- Preserve commands, equations, labels, references, citations, and notation unless the user authorizes changes to them.
- Keep explanatory prose outside display math. Use `\text{...}` only for standard mathematical annotations inside formulas.
- Use an existing theorem-like or boxed environment only when the local document uses it for the same function; do not introduce boxes for emphasis.
- Check delimiters, environment boundaries, labels, and references after editing.

## Final check

Before finishing, verify that:

- the output stays within the authorized mode and span;
- the intended reader can say why the passage exists;
- definitions have visible uses and abstractions solve stated problems;
- concrete examples and formal descriptions remain linked in both directions;
- equations are motivated, inspectable at the chosen level, and interpreted;
- beginner scaffolding does not weaken precision, and mature compression does not erase motivation;
- claims and TeX structure remain grounded and consistent;
- the ending states a genuine conceptual result without mechanical repetition.
