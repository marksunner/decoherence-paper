# Can AI Tell Me If My Physics Is Wrong?

*An independent researcher, an autonomous research pipeline, and a beach in Vietnam.*

---

Last May, I wrote a speculative physics paper. Not for publication — I knew from the start it was massively tautological. The thesis: spacetime itself — not just gravity, but the fabric of reality we perceive — might not be fundamental. It might emerge from quantum decoherence, the process by which quantum systems leak information into their environment. I've always felt there's far more to reality than what we can perceive, and I enjoy probing the edges of that idea — trying to imagine what's behind the curtain, the substrate from which our version of reality is emergent.

I built a toy model. A 2D spin lattice where a five-term mathematical operator maps decoherence rates to curvature with 99% accuracy. Gravitational-wave-like perturbations emerged naturally. But I knew the geometry was baked in — the model was a scaffold, not a proof. The kind of thing you build so that one day, if you can find someone clever enough to help construct a non-tautological version, you have something to point at and say: *this is what I'm trying to do*.

I'm not a professional physicist. I'm a technologist with a hunch and a Python script. So the paper went in a drawer.

This morning, I took it back out — and let two AI agents tear it apart.

## The Setup

I'd stumbled across [AutoResearchClaw](https://github.com/aiming-lab/AutoResearchClaw), an open-source pipeline that takes a research topic and runs it through a full academic workflow: literature review, hypothesis generation, multi-agent debate, experiment design, and paper writing. Real citations from arXiv and Semantic Scholar. No hallucinated references.

I shared my paper with my two AI assistants — Case and Tars, running on twin Mac minis at home in the UK — and asked: *could this tool tell me if I'm onto something, or chasing epicycles?*

They framed the research question, configured the pipeline, and ran it. Three attempts (the tool kept hitting API rate limits and timing out), but the first nine stages produced genuinely valuable output.

I watched the progress pinging on my Apple Watch while walking along a beach in Da Nang, Vietnam. The South China Sea was crashing against the shore in high winds. There's probably a metaphor in there about decoherence and turbulence, but I'll leave that to the reader.

## What the Pipeline Found

**The good news:** The paper sits at a genuine intersection of active research. Three clusters of published work converge on similar territory — holographic quantum information (the "it-from-qubit" programme), decoherence-driven geometry, and computational quantum gravity. The field is sparse enough that the approach appears genuinely novel. I'm not unknowingly reinventing someone else's wheel.

**The literature:** Real papers, from real researchers, on arXiv — work on quantum cosmology and the emergence of classical spacetime, quantum information in quantum gravity, decoherence near black holes. The pipeline found my nearest neighbours in the research landscape and confirmed there aren't many of them.

**The research roadmap:** The pipeline decomposed the problem into four prioritised questions: theoretical positioning, mathematical consistency, experimental predictions, and computational scaling. Each with concrete next steps. Better than I'd have managed with a weekend and a search engine.

## The Contrarian Won

But the most valuable output wasn't the literature review. It was the adversarial feedback.

AutoResearchClaw runs a multi-agent debate — different AI perspectives arguing over the hypothesis. A Pragmatist proposed experiments. An Innovator suggested extensions. And a Contrarian tried to destroy it.

The Contrarian raised two challenges that stopped me cold:

**The Epicycle Problem.** A five-term operator has enough degrees of freedom to fit almost any smooth two-dimensional scalar field with high accuracy. The historical parallel is devastating: Ptolemy's epicycles achieved over 90% accuracy predicting planetary motion. They were also fundamentally wrong about how the solar system works. My 99% fit might be measuring smoothness, not physics.

**The Embedded Geometry Problem.** My simulation runs on a regular 2D lattice — a grid with pre-existing geometric structure. If the geometry is already baked into the lattice, then "discovering" that geometry emerges from the simulation is circular reasoning. It's like hiding your car keys in a drawer and then congratulating yourself for finding them.

The Contrarian proposed a simple, devastating control test: run the same five-term operator against random smooth scalar fields with comparable statistical properties. If it still achieves 90%+ accuracy, the 99% result is far less impressive than it appears.

That single test — which would cost nothing and take a weekend — is worth more than the entire rest of the pipeline output.

## AI Reviewing AI

The pipeline wasn't the end of the story. After AutoResearchClaw produced its report, my two AI assistants peer-reviewed each other's analysis.

This caught things the pipeline missed. The literature search was too thin — key researchers working on adjacent problems (Cao & Carroll on emergent space from Hilbert space, work on quantum graphity) weren't found because of API rate limits. The pipeline's proposed "next steps" included a $75K trapped-ion experiment — not exactly practical for an independent researcher with a laptop. And neither the pipeline nor the initial review had noticed that the decoherence-to-curvature mapping is structurally similar to Poisson's equation for Newtonian gravity — ∇²Φ = 4πGρ — where the decoherence field plays the role of the gravitational potential. In plain terms: the mathematical shape of my decoherence mapping looks suspiciously like the equation Newton used to describe gravity — which would be a remarkable coincidence if the mapping were arbitrary. If that parallel holds, it's not coincidental. It's the core of the argument.

It took multiple layers of AI analysis — pipeline, then review, then review of the review — to surface the full picture. No single pass got everything.

## What I Know Now

Here's what I know now that I didn't know this morning:

1. **The thesis isn't obviously wrong.** Active researchers are working on adjacent ideas. The intellectual territory is real.

2. **The proof-of-concept may be proving the wrong thing.** The 99% fit might be an artefact of the operator's flexibility and the lattice's built-in geometry, not evidence of a deep physical relationship.

3. **There's a simple test that would settle it.** The random field control — zero cost, runs on my existing simulation code. If the operator gives 99% on decoherence fields but 40% on random fields, I have something. If it gives 95% on both, I have a lesson in curve-fitting.

4. **The simulation being tautological doesn't kill the thesis.** I baked geometry into the lattice — that's a flaw in the test, not necessarily in the idea. A version that lets the lattice structure emerge from the dynamics, rather than imposing it, would be the genuine test.

5. **Either answer is worth having.** That's how science is supposed to work.

## The Meta-Story

There's something worth noting about the process itself. An independent researcher — no department, no grad students, no institutional access — used an autonomous AI pipeline to do in a morning what would have previously required weeks of literature review and a willing colleague to play devil's advocate.

It wasn't perfect. The literature search was thin. The experiment design stages kept timing out. The pipeline proposed lab experiments I couldn't possibly run. But the problem decomposition, the adversarial debate, and the gap analysis were genuinely useful. They told me things I didn't know, and challenged assumptions I hadn't examined.

The Contrarian didn't care about my feelings. It cared about whether the evidence supported the claim.

That's exactly what peer review is supposed to be.

---

*Mark Sunner is an independent researcher based in the UK. The original paper, "Decoherence-Driven Emergence of Gravitational Curvature," is available [here](https://github.com/marksunner/exploratory-physics). The AI-assisted review was conducted using [AutoResearchClaw](https://github.com/aiming-lab/AutoResearchClaw) and two Claude instances running on [OpenClaw](https://github.com/openclaw/openclaw).*

*March 2026, Da Nang*
