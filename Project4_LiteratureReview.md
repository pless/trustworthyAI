# Trustworthy AI Project 4: Literature Review

In the Trustworthy AI domain, we often say "trust is a construct," which means: let's start from the idea that trust is something we humans make up and agree on—it's not something that just appears on its own. Over the course of this semester, we've talked about different ways that people are trying to understand AI systems, understand what it would mean to trust AI systems, and perhaps understand how to build systems that can be trusted. These discussions remain incomplete, and what "trust" is as a construct related to AI is both unclear and changing as the technology (and our relationship to it) changes.

This assignment focuses on understanding what a construct is and why there is so much confusion about what things mean. For **Part I**, you will identify and digest 6 readings that center on trust (or trust by another name) and for each reading chart the move from fuzzy concept to operationalization. For **Part II**, you will catalogue the various names trust goes by. For **Part III**, you will construct a schema that represents the construct most relevant to your problem domain or area of interest. Finally, in **Part IV**, you will write a bridging reflection that connects the pieces.

---

## Acceptable Sources

Your 6 readings should be drawn from the following source types:

- **Peer-reviewed publications**: journal articles, conference papers (e.g., FAccT, AIES, NeurIPS, CHI, CSCW, IEEE S&P)
- **Policy and standards documents**: NIST AI RMF, EU AI Act supporting documents, ISO/IEC standards
- **White papers and technical reports**: from research labs, think tanks, or government agencies (e.g., RAND, AI Now, Partnership on AI, GAO)
- **Book chapters**: from edited volumes on AI ethics, STS, or related fields

Blog posts, news articles, and opinion pieces do not count toward the 6, though you may reference them in your discussion.

---

## 1. Pick your context

Choose a specific AI application domain you care about. Be specific. "AI for healthcare" is too broad. "AI-assisted medical diagnosis" or "LLMs for legal document review" is better.

As a concrete example, imaging you pick "AI for donation pricing" helping a relief organization that uses a VLM system to value donated goods (boxes of diapers, boots, dish soap). The system photographs each donation box, segments the objects, and assigns a price to each item. There are papers about this topics (my group is writing some of them).  When those papers talk about trust, it becomes clear that "Trust" in that system means very different things depending on where you stand. At the algorithm level, trust is about accuracy (did the VLM correctly identify 24 diapers vs. a box of 24 diapers? Is the price lookup current?). At the operator level, it's about appropriate reliance (does the volunteer just accept the number, or do they sanity-check?). At the organization level, it's about defensibility (can you stand behind these valuations in a tax audit?). At the societal level, it's about legitimacy (will the IRS accept this methodology?). Same word, completely different conceptualizations and operationalizations at each layer.

## 2. Find 6 journal papers

Find 6 journal papers that discuss trust/trustworthiness of AI in your context (or closely related ones). Prioritize peer-reviewed work.

## 3. Extract fuzzy concept, conceptualization, and operationalization (Part I)

For each paper, extract three things and put them in the table in the deliverable template:

- **Fuzzy concept:** what do they think trust is, in plain language? What problem does lack of trust cause?
- **Conceptualization:** how do they make it precise? What dimensions or components do they define?
- **Operationalization:** how do they propose to measure it? (Surveys? Behavioral proxies? System metrics like explanation fidelity?)

Using the donation example, one row might look like: Fuzzy concept = "the system gives us numbers we can defend to the IRS." Conceptualization = "consistency of valuations across sites, operators, and time." Operationalization = "coefficient of variation in per-item valuations across 5 sites over 30 days."

## 4. Look for "trust by other names" (Part II)

Include this as a section in your document. Other papers in your domain may not use the word "trust" but discuss closely related constructs: reliability, confidence, transparency, accountability, fairness, interpretability, etc. Identify these and note how they relate to trust. In the donation system, for instance, you might find papers on "valuation accuracy" or "appraisal consistency" that never mention trust but are clearly operationalizing a facet of it.

## 5. Build your trust schema (Part III)

Using the system boundary diagram from the slides (algorithm, system, user/operator, operating context, society), map where each construct and operationalization lives. Trust at the algorithm level (e.g., segmentation IoU) is very different from trust at the societal level (e.g., regulatory compliance).

## 6. Reflection

Write a short reflection (roughly half a page) connecting Parts I–III:

- Of the 6 operationalizations you charted in Part I, which one is most relevant to the trust relationship you identified in your schema (Part III)? Why?
- Which operationalization is the *least* appropriate fit? What does it miss about your domain?
- If none of the operationalizations from Part I fully capture the trust relationship in your schema, describe what an ideal operationalization would need to account for.

## 6. Turn in your deliverable

Turn in your deliverable as a **PDF or a blog post** here: [Submission Link](https://docs.google.com/forms/d/e/1FAIpQLSeEvdpKrCRG17KMY4NBuYea32rZXUK3kZVmWTw_WJ7BCXLVIg/viewform?usp=sharing)
