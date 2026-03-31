# Research Narrative

**Title:** Building Research Infrastructure for Studying Human-AI Collaboration in Business Education at Scale

**PI:** Vishal Sachdev, Clinical Associate Professor, Department of Business Administration

---

## 1. Research Problem and Motivation

The rapid integration of AI into business practice has created an urgent empirical gap: we do not understand how business professionals develop the skills to collaborate effectively with AI systems. Existing research on human-AI interaction relies predominantly on controlled laboratory experiments with simplified tasks (Brynjolfsson & McElheran, 2016; Dell'Acqua et al., 2023). While valuable, these studies cannot capture the longitudinal skill development, contextual adaptation, and organizational dynamics that characterize real-world AI adoption.

Business schools are uniquely positioned to close this gap. Every semester, thousands of students engage with AI tools across diverse business problems — from financial analysis to marketing strategy to operations optimization. Yet this naturalistic learning activity produces almost no usable research data because the interactions are fragmented across disconnected tools with no shared instrumentation.

This proposal addresses this infrastructure deficit by building a research platform that captures rich, IRB-consented interaction data as Gies students build AI solutions for authentic business challenges. The platform transforms an activity that already occurs at scale — student AI projects — into a systematic research program.

## 2. Research Questions and Scholarly Contributions

The platform enables three streams of inquiry, each targeting distinct scholarly audiences:

**Stream 1: Human-AI Collaborative Skill Development (Field Study)**

*RQ1: How do novice business professionals develop AI collaboration skills over time, and what task characteristics predict effective versus ineffective human-AI partnerships?*

This stream conducts a longitudinal field study tracking 500+ students across 60+ AI projects in Year 1. The platform captures task-level interaction data: prompting strategies, tool selections, iteration patterns, error recovery, and outcome quality. Analysis combines process mining of interaction sequences with qualitative coding of collaboration patterns. Prior work has shown that AI collaboration skill varies dramatically across individuals (Noy & Zhang, 2023), but no study has tracked how these skills develop over an academic term in realistic task environments.

Target outlets: *MIS Quarterly*, *Information Systems Research*, *Management Science*

**Stream 2: Organizational Attention and AI Infrastructure (Qualitative/Archival)**

*RQ2: How does shared AI infrastructure reshape organizational attention patterns toward technology capability building?*

This stream applies Ocasio's (1997, 2011) attention-based view to study how the platform itself — as a structural mechanism — channels institutional attention toward AI. Using archival data from the platform (challenge postings, resource allocation decisions, participation patterns) combined with interviews of faculty and administrators, this research examines how formal AI infrastructure differs from ad hoc AI initiatives in sustaining organizational commitment. This directly extends Ocasio's (2025) recent work on attentional control in organizations by providing empirical evidence from a designed intervention.

Target outlets: *Organization Science*, *Administrative Science Quarterly*, *Academy of Management Journal*

**Stream 3: Open Research Dataset for Gies Faculty**

*RQ3 (enabling): What patterns of AI-mediated decision-making, learning, and collaboration emerge from large-scale instrumented business education?*

The platform produces a curated, de-identified research dataset — targeting 15,000+ annotated interactions in Year 1 and 60,000+ by Year 3 — available to any Gies faculty with IRB approval. This dataset enables investigations that individual researchers could not resource alone: learning analytics studies of AI in pedagogy, behavioral studies of AI-assisted decision-making, and computational analyses of collaborative problem-solving. The infrastructure model follows successful precedents such as the Wharton Research Data Services (WRDS) approach of building shared data assets that serve an entire research community.

## 3. Research Design and Methods

**Data Collection Platform.** The AI Innovation Engine provides a shared technical environment where students complete AI projects. The platform instruments interactions at three levels: (a) task-level logs capturing tool usage, prompting, and iteration; (b) project-level metadata including challenge type, team composition, and outcomes; and (c) assessment data from rubric-based evaluations. All data collection follows IRB protocols with informed consent.

**Participant Recruitment.** Participants are students enrolled in Gies courses that use the platform. Year 1 targets 3 courses (approximately 500 students). By Year 3, the platform targets 30 courses across departments. The naturalistic field study design avoids selection bias — students encounter the platform as standard course infrastructure, not a research intervention.

**Analysis Methods.** Stream 1 employs mixed methods: process mining of interaction sequences using ProM/PM4Py, qualitative coding of collaboration patterns (Strauss & Corbin grounded theory), and regression analysis of skill development trajectories. Stream 2 uses qualitative case study methodology (Eisenhardt, 1989) with archival platform data triangulated against semi-structured interviews (target: 20-30 faculty, staff, and administrators). Stream 3 involves dataset curation, documentation, and validation following FAIR data principles.

**Timeline.**

| Period | Activity |
|---|---|
| Summer 2026 | Platform development, IRB submission, pilot instrumentation |
| Fall 2026 | Data collection begins: 3 courses, ~500 students, ~60 projects |
| Spring 2027 | Scale to 12 courses. Stream 1 analysis begins. Stream 2 interviews. |
| AY 2027-28 | Publications from Streams 1 & 2. Dataset release (Stream 3). NSF proposal. |
| AY 2028-29 | Follow-up studies. External grant-funded expansion. |

## 4. Broader Impact and Multi-Investigator Potential

This infrastructure is deliberately designed to serve multiple researchers. The open dataset (Stream 3) enables any Gies faculty member to study AI-related phenomena without building their own data collection apparatus. Specific cross-departmental opportunities include:

- **Accountancy:** AI-assisted audit judgment and decision-making
- **Finance:** AI in financial analysis workflows and risk assessment
- **Marketing:** AI-mediated consumer insight generation
- **Strategy/OB:** Organizational responses to AI capability building

The platform also builds directly on existing Gies investments: the Magelli Office's 200+ annual client projects (which provide the authentic challenge pipeline), the PI's open-source Canvas MCP tools (90+ tools, adopted across 6 courses, published on PyPI), and active student builder organizations (IBC, Disruption Lab, AgentLab).

**External Funding Trajectory.** The Year 1 data and initial publications position a competitive NSF proposal to the Cyberlearning and Future Learning Technologies program (estimated submission: Fall 2027, typical award: $500K-$750K). Corporate research partnerships with current Gies DBC/CSP partners provide additional funding pathways.

## 5. PI Qualifications

The PI brings a distinctive combination of technical building and pedagogical research:

- Developer of Canvas MCP, an open-source AI toolkit for education (90+ tools, PyPI-published, adopted across 6 Gies courses)
- Clinical Associate Professor teaching AI-intensive courses (BADM 554, BADM 590) with 1,000+ students using AI tools annually
- Presenter at ICIS 2025 on AI capability architecture in organizations
- Founded and advises AgentLab, a student research organization focused on AI agent development
- 11 years of industry experience in technology product management prior to academia

---

## References

Brynjolfsson, E., & McElheran, K. (2016). The rapid adoption of data-driven decision-making. *American Economic Review*, 106(5), 133-139.

Dell'Acqua, F., et al. (2023). Navigating the jagged technological frontier. *Harvard Business School Working Paper* 24-013.

Eisenhardt, K. M. (1989). Building theories from case study research. *Academy of Management Review*, 14(4), 532-550.

Noy, S., & Zhang, W. (2023). Experimental evidence on the productivity effects of generative AI. *Science*, 381(6654), 187-192.

Ocasio, W. (1997). Towards an attention-based view of the firm. *Strategic Management Journal*, 18(S1), 187-206.

Ocasio, W. (2011). Attention to attention. *Organization Science*, 22(5), 1286-1296.
