# Research Narrative

**Title:** Studying Human-AI Collaboration in Business Education: A Cross-Departmental Research Platform Built on Existing Gies Infrastructure

**PI:** Vishal Sachdev, Clinical Associate Professor, Business Administration
**Co-Is:** Qingquan Zhang, Clinical Assistant Professor, Finance; Matias Carrasco Kind, Research Assistant Professor, Accountancy / Director, Data Science Research Services (DSRS)

---

## 1. Research Problem

The rapid integration of AI into business practice has created an urgent empirical gap: we do not understand how business professionals develop the skills to collaborate effectively with AI systems. Existing research relies predominantly on controlled laboratory experiments with simplified tasks (Dell'Acqua et al., 2023). While valuable, these studies cannot capture the longitudinal skill development and contextual adaptation that characterize real-world AI use. Meanwhile, every semester thousands of Gies students engage with AI tools across business courses — yet this naturalistic activity produces almost no usable research data because interactions are fragmented across disconnected tools with no shared instrumentation.

This proposal addresses this infrastructure deficit by combining existing Gies assets — Canvas MCP (Sachdev), DSRS computational infrastructure (Carrasco Kind), and AI-finance research expertise (Zhang) — into a shared research platform that captures rich, IRB-consented interaction data as students build AI solutions across multiple business domains.

## 2. Research Questions

**RQ1:** How do novice business professionals develop AI collaboration skills over time, and what task characteristics predict effective versus ineffective human-AI partnerships?

**RQ2:** How does AI assistance affect the quality, speed, and confidence calibration of business decisions across functional domains (finance, analytics, general management)?

**RQ3:** What patterns of appropriate versus inappropriate AI reliance emerge from large-scale instrumented business education, and do they vary by domain expertise and AI experience?

## 3. Research Design

**Data Collection Platform.** The platform instruments student-AI interactions at three levels: (a) task-level logs capturing tool usage, prompting strategies, and iteration patterns; (b) project-level metadata including task type, team composition, and outcomes; and (c) assessment data from rubric-based evaluations. All data collection follows IRB protocols with informed consent. Students encounter the platform as standard course infrastructure, not a research intervention, avoiding selection bias.

**Infrastructure.** Rather than building from scratch, this project integrates two mature Gies systems. Sachdev's Canvas MCP — an open-source AI toolkit with 90+ tools, published on PyPI and adopted across 6 courses — provides the student-facing instrumentation layer. DSRS's on-premises compute cluster (486 CPU cores, 2.2 TB RAM, NVIDIA A100 GPUs, Kubernetes) and Atlas agentic framework provide the backend for data processing, LLM inference, and analysis pipelines. This integration eliminates the need for new infrastructure investment and leverages over $160K in existing Microsoft Azure credits awarded to DSRS.

**Domain-Specific Tasks.** Zhang contributes finance-domain AI decision tasks drawn from his research on AI-driven competitive intelligence (Zhang, 2025, *Expert Systems with Applications*), alternative data in investment management (Zhang, 2022, Palgrave Macmillan), and AI-assisted financial analysis. These validated tasks enable controlled comparisons of AI-assisted versus unassisted decision-making in finance — complementing the naturalistic field study data from Canvas MCP-instrumented courses.

**Analysis Methods.** RQ1 employs mixed methods: process mining of interaction sequences (PM4Py) and regression analysis of skill development trajectories across a semester. RQ2 uses within-subject experimental designs embedded in finance courses, measuring decision quality, confidence calibration, and process efficiency. RQ3 combines quantitative analysis of the instrumented dataset with qualitative coding of collaboration patterns (grounded theory). The cross-departmental design enables comparisons that single-department studies cannot achieve.

**Participants.** Year 1 targets 3 courses (~300 students) across Business Administration and Finance. Year 2 scales to 8 courses across all three departments. The naturalistic design means students participate through normal coursework, not as recruited subjects — dramatically reducing participant acquisition costs while increasing ecological validity.

## 4. Team and Complementary Expertise

This proposal brings together three investigators whose existing work directly enables the project without new infrastructure development:

**Vishal Sachdev (PI, Business Administration)** — Developer of Canvas MCP (90+ tools, PyPI-published, 6 course adoptions), founder of AgentLab student research organization, presenter at ICIS 2025. Provides the student-facing instrumentation layer and student builder ecosystem.

**Qingquan Zhang (Co-I, Finance)** — Author of *Alternative Data and AI Techniques* (Palgrave Macmillan, 2022), published on AI-driven competitive intelligence and generative AI's impact on corporate valuation. CITL Faculty Fellow and Gies Innovation Scholar (2024-25). Provides finance-domain AI decision tasks and experimental methodology expertise. Zhang's EdTech startup experience contributes practical insight on AI tool design and adoption measurement.

**Matias Carrasco Kind (Co-I, Accountancy/DSRS)** — Director of Data Science Research Services, which has completed 245+ tasks for 60+ faculty members across departments. DSRS operates a 486-core compute cluster with A100 GPUs, manages the Atlas agentic framework, and has self-hosted LLM inference endpoints. Provides computational infrastructure, data pipeline expertise, and the student intern team for platform integration.

## 5. Timeline

| Period | Activity |
|---|---|
| Summer 2026 | IRB submission; instrument Canvas MCP courses for data capture; integrate with DSRS Atlas backend; develop finance-domain AI decision task battery |
| Fall 2026 | Pilot data collection: 3 courses, ~300 students; Zhang runs finance AI decision experiment |
| Spring 2027 | Scale to 5 courses; begin analysis of Fall data; draft RQ1 and RQ2 papers |
| Summer 2027 | Dataset curation and documentation (FAIR principles); prepare NSF Cyberlearning pre-proposal |
| Fall 2027 | Full deployment: 8 courses across 3 departments; release open dataset for Gies faculty |
| Spring 2028 | Submit 2-3 papers; submit NSF proposal; present at ICIS and AOM |

## 6. Broader Impact and External Funding

The open research dataset (targeting 10,000+ annotated interactions in Year 1, 40,000+ by Year 2) is available to any Gies faculty member with IRB approval, enabling investigations that individual researchers could not resource alone: learning analytics, AI-mediated decision-making, and technology adoption studies across Accountancy, Finance, Marketing, and Strategy.

The Year 1 data and initial publications position a competitive NSF proposal to the Cyberlearning and Future Learning Technologies program (typical award $500K-$750K). Zhang's existing connections to fintech industry sponsors and an alumni investor with interest in AI agent research provide additional external funding pathways. The cross-departmental design — spanning three departments and two methodological traditions (field study and experimental) — strengthens the external grant narrative substantially.

## 7. Alignment with CFP Criteria

- **"Educational or pedagogical data acquisition, extraction, and analyses costs"** — directly listed as eligible use
- **"Improvements to the capabilities of any current research initiatives or laboratories"** — extends DSRS capabilities to education research
- **Multi-investigator:** Three departments, shared dataset serving 10+ researchers
- **External funding trajectory:** NSF Cyberlearning + fintech industry partnerships
- **College strategic priority:** AI is the top strategic priority; this provides research evidence to guide the strategy

---

## References

Dell'Acqua, F., et al. (2023). Navigating the jagged technological frontier. *Harvard Business School Working Paper* 24-013.

Noy, S., & Zhang, W. (2023). Experimental evidence on the productivity effects of generative AI. *Science*, 381(6654), 187-192.

Zhang, Q. (2022). *Alternative Data and Artificial Intelligence Techniques: Applications in Investment and Risk Management*. Palgrave Macmillan.

Zhang, Q., et al. (2025). From Data to Strategy: A Public Market Framework for Competitive Intelligence. *Expert Systems with Applications*.

Zhang, Q. (2025). Information Transparency and the Effectiveness of Tax Policies: Evidence from Cryptocurrency Price Disparity. *Best Paper Award, 25th NBES Annual Conference*.
