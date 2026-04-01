# Research Narrative

**Title:** The Gies AI Innovation Engine: Shared Research Infrastructure for AI-Driven Business Education

**PI:** Vishal Sachdev, Clinical Associate Professor, Business Administration
**Co-Is:** Qingquan Zhang, Clinical Assistant Professor, Finance; Matias Carrasco Kind, Research Assistant Professor, Accountancy / Director, Data Science Research Services (DSRS)

---

## 1. The Opportunity

Every top business school is adding AI courses. Few are building infrastructure where the act of teaching AI simultaneously produces reusable tools, generates research data, and builds institutional capability. Gies can be first — and the pieces already exist.

The Magelli Office runs 200+ client projects per year. Six courses already use Canvas MCP, an open-source AI toolkit with 90+ tools. DSRS operates a 486-core compute cluster with 2 A100 GPUs, self-hosted LLM endpoints, and the Atlas agentic framework that powers the DSRS chatbot and other AI tools — a peer-reviewed infrastructure described in Carrasco Kind (2023). DSRS has also built iKompete, a competition platform for challenge submissions, peer evaluation, and leaderboards. Student builder organizations (AgentLab, IBC, Disruption Lab) are actively building AI solutions. Yet these assets are disconnected: no shared challenge pipeline, no compound skill library, and no research instrumentation.

This proposal funds the coordination layer that connects them — the AI Innovation Engine.

## 2. What We Propose

The AI Innovation Engine is a platform where faculty post real-world AI challenges and student teams build solutions using shared open-source infrastructure. Every completed project deposits a reusable AI skill into a compound library that makes the next project faster and generates annotated research data for studying human-AI collaboration. The Engine is not a new program — it is an AI coordination layer on top of infrastructure that already exists.

**How it works.** Faculty across departments post challenge briefs — operational automations, analytical tools, course infrastructure needs. DSRS's iKompete platform provides the submission, evaluation, and leaderboard infrastructure. Student builder teams (AgentLab, Disruption Lab, course project teams) select challenges and build solutions using the shared technical stack: Canvas MCP for LMS integration, DSRS for compute and data pipelines, and domain-specific tools contributed by each PI. Completed solutions enter the skill library; interaction data flows to the research dataset.

**The compound skill library.** This is the Engine's flywheel. Each completed project produces reusable components — prompt templates, data connectors, workflow patterns, evaluation rubrics. Next semester's students start with a richer toolkit. Over two years, the library grows from proof-of-concept to a shared asset that accelerates AI project delivery across Gies courses. This "Build to Learn, Learn to Build" model means students don't just consume AI tools — they architect systems that serve the next cohort.

**Research data as byproduct.** The Engine instruments student-AI interactions at three levels: (a) task-level logs capturing tool usage, prompting strategies, and iteration patterns; (b) project-level metadata including challenge type, team composition, and outcomes; and (c) assessment data from rubric-based evaluations. All data collection follows IRB protocols with informed consent. Because students encounter the Engine as standard course infrastructure, the design avoids the selection bias that limits laboratory AI studies (Dell'Acqua et al., 2023).

## 3. Research Questions

The instrumented platform enables three lines of inquiry:

**RQ1:** How do novice business professionals develop AI collaboration skills over time, and what task characteristics predict effective versus ineffective human-AI partnerships?

**RQ2:** How does AI assistance affect the quality and confidence calibration of business decisions across functional domains (finance, analytics, general management)?

**RQ3:** What patterns of AI-mediated decision-making, skill development, and collaboration emerge from large-scale instrumented business education?

RQ1 employs process mining of interaction sequences and regression analysis of skill trajectories. RQ2 uses experimental designs embedded in finance courses (Zhang), measuring decision quality and appropriate AI reliance. RQ3 produces the open dataset — curated, de-identified, and documented following FAIR principles — available to any Gies faculty member with IRB approval.

## 4. Team

**Vishal Sachdev (PI, Business Administration)** — Developer of Canvas MCP (90+ tools, PyPI-published, 6 course adoptions), founder of AgentLab student research organization, presenter at ICIS 2025. Designs the Engine's challenge flow, student coordination, and skill library. Teaches AI-intensive courses (BADM 554, BADM 590) serving 1,000+ students annually.

**Qingquan Zhang (Co-I, Finance)** — Author of *Alternative Data and AI Techniques* (Palgrave Macmillan, 2022), published on AI transparency and tax policy in cryptocurrency markets (*Research Policy*, 2026) and AI-driven competitive intelligence (*Expert Systems with Applications*, 2025). Best Paper Award, 25th NBES Annual Conference (2025). CFA charterholder. CITL Faculty Fellow and Gies Innovation Scholar (2024-25). Contributes the first finance-domain challenges to the Engine and AI decision-making experimental methodology. Zhang's experience building an EdTech AI startup informs platform design and adoption measurement.

**Matias Carrasco Kind (Co-I, Accountancy/DSRS)** — Director of Data Science Research Services, which has completed 400+ tasks for 60+ faculty members across all Gies departments. Also holds appointments at the National Center for Supercomputing Applications (NCSA) and as Faculty in Residence at Discovery Partners Institute (DPI). DSRS operates a compute cluster with 486 CPU cores, 2.2 TB RAM, 2 NVIDIA A100 GPUs, and has published its architecture as a peer-reviewed case study (Carrasco Kind, 2023). Carrasco Kind's team built the iKompete challenge platform and the Atlas agentic framework, provides the Engine's computational backbone, and brings 42+ graduate and 42+ undergraduate research advisees. DSRS's existing cross-departmental service model means the infrastructure is already designed to support multiple faculty researchers.

**An April 2026 buildathon** — using DSRS infrastructure for staff-facing AI challenges — is already underway as the first pilot of this three-PI collaboration.

## 5. Timeline

| Period | Activity |
|---|---|
| **April 2026** | Buildathon pilot: first challenges run through DSRS infrastructure, three-PI collaboration tested |
| **Summer 2026** | IRB submission; design Engine coordination layer; evaluate and integrate tool stack; develop skill library schema |
| **Fall 2026** | Engine launch: 3 courses (~300 students), first challenges posted, data collection begins |
| **Spring 2027** | Scale to 5 courses; Zhang runs finance AI decision challenges; begin analysis of Fall data |
| **Summer 2027** | Dataset curation (FAIR principles); draft papers for RQ1 and RQ2; prepare NSF pre-proposal |
| **Fall 2027** | Full deployment: 8 courses across 3 departments; release open dataset for Gies faculty |
| **Spring 2028** | Submit 2-3 papers; submit NSF Cyberlearning proposal; present at ICIS and AOM |

## 6. Broader Impact and External Funding

**Open research dataset.** The Engine's instrumented data (targeting 10,000+ annotated interactions in Year 1, 40,000+ by Year 2) is available to any Gies faculty member with IRB approval — enabling studies of AI-mediated decision-making, learning analytics, and technology adoption across Accountancy, Finance, Marketing, and Strategy.

**Roadmap beyond the grant.** The Engine's architecture supports future extensions not funded here: corporate challenge sponsorships from Gies's DBC/CSP partners (30+ Fortune 500 companies), an Origin Ventures commercialization pathway for student-built tools, and a "Bring Your Own Challenge" model for Gies's 5,000+ online MBA students. These represent revenue pathways that can sustain the Engine beyond the grant period.

**Philanthropic potential.** The Engine positions Gies as a destination for alumni donors seeking to invest in AI infrastructure with measurable institutional impact. By establishing dedicated AI research infrastructure that bridges cutting-edge research with real-world business outcomes, Gies demonstrates the execution capacity that discerning donors look for — an investment in building the future, not just keeping pace with it. Early conversations with alumni investors interested in AI agent research are already underway.

**External funding.** Year 1 data and publications position a competitive NSF proposal to the Cyberlearning and Future Learning Technologies program (typical award $500K-$750K). Zhang's connections to fintech industry sponsors provide additional pathways. The combination of philanthropic interest, corporate sponsor revenue, and federal grants creates a multi-source funding model that can sustain the Engine well beyond the initial two-year investment.

## 7. CFP Alignment

- **"Expert human capital for improving the College's business data analytics capabilities by building out of infrastructure"** — the Engine is exactly this: shared AI infrastructure built by student teams
- **"Improvements to the capabilities of any current research initiatives or laboratories"** — extends DSRS from a faculty service bureau to a platform generating research data at scale
- **"Educational or pedagogical data acquisition, extraction, and analyses costs"** — directly funds the data pipeline
- **Multi-investigator:** Three departments, shared dataset serving 10+ researchers, open by design
- **External funding trajectory:** NSF Cyberlearning + philanthropic donors + industry partnerships
- **College strategic priority:** AI is Gies's top strategic priority; the Engine provides infrastructure to match the ambition

---

## References

Carrasco Kind, M. (2023). Scalable Research Infrastructure in a Business School Context: A Case Study of the Data Science Research Services. *Gateways 2023*, Paper 28.

Dell'Acqua, F., et al. (2023). Navigating the jagged technological frontier. *Harvard Business School Working Paper* 24-013.

Noy, S., & Zhang, W. (2023). Experimental evidence on the productivity effects of generative AI. *Science*, 381(6654), 187-192.

Zhang, Q. (2022). *Alternative Data and Artificial Intelligence Techniques: Applications in Investment and Risk Management*. Palgrave Macmillan.

Zhang, Q. (2026). How transparency shapes tax policy effectiveness: Evidence from cryptocurrency markets. *Research Policy*, 55.

Zhang, Q., et al. (2025). From Data to Strategy: A Public Market Framework for Competitive Intelligence. *Expert Systems with Applications*, 296.
