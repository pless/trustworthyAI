---
layout: default
title: Project 1
---
## Trustworthy AI Final Project
 
The final is to write up a project in the scope and format of the [9th AAAI Conference on AI, Ethics, and Society](https://www.aies-conference.com/2026/call-for-papers/). You may, but do not have to, write it in exactly the right format to submit to this conference.
 
## Team
 
You can work in groups of up to 3 students.  Only one person needs to submit.
 
Submit here: [Google Form](https://docs.google.com/forms/d/e/1FAIpQLSeEvdpKrCRG17KMY4NBuYea32rZXUK3kZVmWTw_WJ7BCXLVIg/viewform?usp=sharing)
 
## Deadlines
 
- **Initial Project Deadline:** May 4 at noon. Projects submitted then will be graded, and final projects for the class will be calculated so you know what will be submitted assuming nothing additional is turned in. Guidance will be offered for how to improve a subsequent submission.
- **Final Final Project Deadline:** May 11 at noon.
---
 
The following outlines one way to think about and develop such a project, to give direction if helpful and share the scope. Many other structures are possible, and if you have something in mind I encourage you to explore that. First I will describe a more technical version; you can also choose the more analytical version described below.
 
## Technical Specific Goals
 
Identify and motivate a specific application or domain with an AI approach that has value in that area (a chatbot that more quickly answers customer queries, a diagnosis system that better interprets X-rays, a home-brew vision system that counts birds at your birdfeeder, etc.) and failure modes that could potentially undermine trust for you or others interested in that domain (e.g. it never recognizes painted buntings).
 
Describe your problem domain in depth. Who is harmed when the system fails? What "error rate" is good enough — is it like predicting Netflix movies where if you get it wrong it doesn't matter that much, or super-critical?
 
Develop and quantify at least one quantitative measure of "trustworthiness" relevant to your chosen AI system, and justify why that measure maps to trust in your domain:
 
- Does your system give a probability that it is correct? Are those probabilities correct?
- Does it do selective prediction where some groups or items or recommendations are always ignored?
- Does it improperly translate French idioms from Normandy?
Before proposing any modification, report the unmodified system's score on your metric, and pre-register (say ahead of time) 3–5 concrete inputs you predict will fail.
 
**Implement a trust-improving modification.** Propose and apply a concrete improvement to the AI system. This could involve writing additional code, introducing a new structural component, fine-tuning models, adjusting training data, or implementing refined prompting strategies.
 
**Evaluate and analyze your modification.** Conduct an analysis comparing your modified AI system to the original, using your quantitative measure(s). Include a qualitative analysis of realistic examples and use cases, drawn from a held-out set distinct from your quantitative evaluation set. Discuss the "trust tax" of your modification — what it costs in latency, compute, coverage, simplicity, or elsewhere — and note limitations and who remains unprotected. Well-analyzed negative results (interventions that fail to improve the metric) receive full credit.
 
## Analytical Specific Goals
 
1. Identify a domain and a trust failure mode, and define an *operationalizable* criterion, framework, or evaluation protocol relevant to it — operationalizable meaning that someone could in principle apply it to a system and reach a verdict.
2. Propose a concrete intervention to the governance, evaluation, deployment, disclosure, or auditing of the system, rather than to the system itself.
3. Apply your framework to at least two real or plausible near-future deployed systems as case studies, pre-registering hard cases before the analysis, and discuss the "trust tax" (compliance cost, chilling effects, false reassurance, tradeoffs with other values). Related-work expectations and AIES framing are unchanged; AIES in fact publishes more analytical work than empirical work.
### Example
 
I'm less good at defining projects like this, so here is the framing of a concrete project that could fit this model.
 
**A disclosure standard for "AI-assisted" in journalism.**
 
*Domain and failure mode:* Several outlets (AP, Wired, The Verge) have published AI-use policies. Define what a useful disclosure would need to specify — for example, which task (drafting, translation, summarization, image selection), which model, whether a human verified factual claims, whether sources were AI-suggested — so that a reader could form a calibrated view of how much to trust the piece.
 
*Intervention:* a four-line disclosure template.
 
*Case studies:* two published AI-use policies (pick any two outlets); show what each catches and misses.
 
*Pre-registered hard cases:* a piece where AI was used to find sources but not write; a piece translated by AI from a foreign-language original; a piece where AI drafted and a human edited lightly.
 
*Trust tax:* detailed disclosure is commercially awkward, and most readers won't read it; the question is whether it helps the readers who do.
 
## Deliverable
 
Your report could be a webpage or a PDF that has a clear section for each of the above steps. A short related-work paragraph (4–6 citations) situating the intervention is expected. If you are "coding", you are welcome to start with a model (e.g. something on HuggingFace or GPT-4o); if you are prompt engineering, you are welcome to start with a prompt that someone else has proposed — but in all cases be clear about what is your contribution and where you found your starting point.
