# Awesome AI for Economists

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![License: CC0-1.0](https://img.shields.io/badge/License-CC0_1.0-lightgrey.svg)](https://creativecommons.org/publicdomain/zero/1.0/)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](http://makeapullrequest.com)

> A curated list of AI tools and resources **specifically useful for economists** — not another generic AI tools list. We focus on what you can't easily find elsewhere.
>
> For general-purpose AI assistants (ChatGPT, Claude, Gemini) and generic coding tools (Cursor, Copilot), see [Appendix: General-Purpose AI](#appendix-general-purpose-ai). For the canonical framework on how economists can leverage AI, see Korinek's *[Generative AI for Economic Research](https://www.aeaweb.org/articles?id=10.1257/jel.20231736)* (JEL, 2023) and *[AI Agents for Economic Research](https://www.nber.org/papers/w34202)* (NBER, 2025).

---

## Contents

- [MCP Servers for Economic Data](#mcp-servers-for-economic-data)
- [Coding Tools for Economists](#coding-tools-for-economists)
- [Causal Inference and Econometrics](#causal-inference-and-econometrics)
- [Simulation, Forecasting and Macro Modeling](#simulation-forecasting-and-macro-modeling)
- [Literature Review and Research Discovery](#literature-review-and-research-discovery)
- [Economic Data and Analysis](#economic-data-and-analysis)
- [Academic Writing and LaTeX](#academic-writing-and-latex)
- [Document Processing and OCR](#document-processing-and-ocr)
- [NLP and Sentiment for Economics](#nlp-and-sentiment-for-economics)
- [Policy Analysis, Labor Market and Alternative Data](#policy-analysis-labor-market-and-alternative-data)
- [Finance-Specific AI](#finance-specific-ai)
- [Data Collection Tools](#data-collection-tools)
- [Papers and Books](#papers-and-books)
- [Courses, Conferences and Community](#courses-conferences-and-community)
- [Appendix: General-Purpose AI](#appendix-general-purpose-ai)
- [Contributing](#contributing)

---

## MCP Servers for Economic Data

The [Model Context Protocol](https://modelcontextprotocol.io/) (MCP) lets AI assistants directly query economic databases via natural language — a paradigm shift for data access. Ask your AI to "plot the unemployment rate vs inflation for the last 20 years" and it fetches live data.

- [TAM MCP Server](https://github.com/gvaibhav/TAM-MCP-Server) — **One server, 8 sources**: Alpha Vantage, BLS, Census, FRED, IMF, Nasdaq, OECD, and World Bank. 28 tools.
- [FRED MCP Server](https://github.com/stefanoamorelli/fred-mcp-server) — Access all 800,000+ FRED time series; search, browse, and retrieve filtered observations. ![GitHub stars](https://img.shields.io/github/stars/stefanoamorelli/fred-mcp-server?style=flat-square)
- [World Bank MCP Server](https://github.com/anshumax/world_bank_mcp_server) — Query World Bank Open Data API for development indicators across countries. ![GitHub stars](https://img.shields.io/github/stars/anshumax/world_bank_mcp_server?style=flat-square)
- [IMF Data MCP Server](https://github.com/c-cf/imf-data-mcp) — WEO forecasts, balance of payments, and more from the IMF.
- [Nasdaq Data Link MCP](https://github.com/stefanoamorelli/nasdaq-data-link-mcp) — Access Nasdaq/Quandl financial and economic datasets.
- [Alpha Vantage MCP](https://mcp.alphavantage.co/) — Official vendor-maintained server for stocks, forex, commodities, and economic indicators.
- [Census MCP Server](https://lobehub.com/mcp/brockwebb-census-mcp-server) — Natural language queries for U.S. Census demographic data.
- [OpenEcon](https://openecon.ai/) — AI platform querying FRED, World Bank, IMF, Comtrade, StatsCan, Eurostat, BIS via natural language.

> Browse the [MCP Registry](https://registry.modelcontextprotocol.io/) to discover more servers.

---

## Coding Tools for Economists

These are tools built for or particularly useful to economists — not generic coding assistants.

- [Stata-MCP](https://github.com/hanlulong/stata-mcp) — MCP server integrating Stata with AI assistants (Claude, Copilot, Cursor); real-time Stata output in editor, full .do/.ado/.mata support. ![GitHub stars](https://img.shields.io/github/stars/hanlulong/stata-mcp?style=flat-square)
- [Positron IDE](https://posit.co/products/ide/positron/) — Next-gen IDE from Posit (makers of RStudio); R and Python natively with "Positron Assistant" — understands your loaded data, plots, and session context.
- [awesome-econ-ai-stuff](https://github.com/meleantonio/awesome-econ-ai-stuff) — Reusable AI skills for economists (SKILL.md standard); works with Claude Code, Cursor, Codex, Gemini CLI. Covers Stata, Python, LaTeX workflows. ![GitHub stars](https://img.shields.io/github/stars/meleantonio/awesome-econ-ai-stuff?style=flat-square)
- [Marimo](https://github.com/marimo-team/marimo) — Reactive Python notebook stored as pure .py files (git-friendly, reproducible). AI-native with Copilot built in. ![GitHub stars](https://img.shields.io/github/stars/marimo-team/marimo?style=flat-square)
- [Jupyter AI Agents](https://github.com/datalayer/jupyter-ai-agents) — AI agents for JupyterLab with MCP integration — connect notebooks to FRED, World Bank, etc.
- [Jupyter AI](https://github.com/jupyterlab/jupyter-ai) — Official JupyterLab extension; `%%ai` magic commands for code generation/explanation. ![GitHub stars](https://img.shields.io/github/stars/jupyterlab/jupyter-ai?style=flat-square)

---

## Causal Inference and Econometrics

### Core Libraries

- [EconML](https://github.com/py-why/EconML) — Microsoft/py-why: Double ML, causal forests, heterogeneous treatment effects. ![GitHub stars](https://img.shields.io/github/stars/py-why/EconML?style=flat-square)
- [DoWhy](https://github.com/py-why/dowhy) — End-to-end causal inference: model, identify, estimate, refute. ![GitHub stars](https://img.shields.io/github/stars/py-why/dowhy?style=flat-square)
- [CausalML](https://github.com/uber/causalml) — Uber's uplift modeling and causal inference with ML. ![GitHub stars](https://img.shields.io/github/stars/uber/causalml?style=flat-square)
- [DoubleML](https://docs.doubleml.org/) — Chernozhukov et al. (2018) Double/Debiased ML; Python and R. Training via [Economic AI](https://economicai.com/).
- [awesome-causal-inference](https://github.com/matteocourthoud/awesome-causal-inference) — The definitive causal inference resource list. ![GitHub stars](https://img.shields.io/github/stars/matteocourthoud/awesome-causal-inference?style=flat-square)

### Frontier Tools

- [diff-diff](https://github.com/igerber/diff-diff) — sklearn-style DiD library (Jan 2026); fills a critical gap in Python. ![GitHub stars](https://img.shields.io/github/stars/igerber/diff-diff?style=flat-square)
- [contdid](https://github.com/bcallaway11/contdid) — DiD with continuous treatment, by Brantly Callaway. ![GitHub stars](https://img.shields.io/github/stars/bcallaway11/contdid?style=flat-square)
- [moderndid](https://github.com/jordandeklerk/moderndid) — GPU-accelerated modern DiD (staggered adoption, event studies). ![GitHub stars](https://img.shields.io/github/stars/jordandeklerk/moderndid?style=flat-square)
- [CausalMatch](https://github.com/bytedance/CausalMatch) — ByteDance's causal matching engine at industrial scale. ![GitHub stars](https://img.shields.io/github/stars/bytedance/CausalMatch?style=flat-square)
- [CausalFM](https://github.com/yccm/CausalFM) — Foundation models for causal inference (ICLR 2026); pre-trained models replace per-problem estimation. ![GitHub stars](https://img.shields.io/github/stars/yccm/CausalFM?style=flat-square)
- [CausalAgent](https://github.com/DMIRLAB-Group/CausalAgent) — Multi-agent AI for end-to-end causal inference through conversation (Jan 2026).
- [CImpact](https://github.com/Sanofi-Public/CImpact) — Sanofi's causal impact for time series; frequentist and Bayesian. ![GitHub stars](https://img.shields.io/github/stars/Sanofi-Public/CImpact?style=flat-square)
- [Salesforce CausalAI](https://github.com/salesforce/causalai) — Causal analysis for time series and tabular data. ![GitHub stars](https://img.shields.io/github/stars/salesforce/causalai?style=flat-square)
- [DoubleLingo](https://github.com/markov24/DoubleLingo) — Double ML with LLM-based nuisance models; causal inference on unstructured data.
- [TexIV](https://github.com/SepineTam/TexIV) — Extract instrumental variables from text data using ML.

---

## Simulation, Forecasting and Macro Modeling

### Agent-Based Models and LLM Simulation

- [BeforeIT.jl](https://github.com/bancaditalia/BeforeIT.jl) — **Bank of Italy's** ABM macroeconomics in Julia; institutional-quality, open-source. ![GitHub stars](https://img.shields.io/github/stars/bancaditalia/BeforeIT.jl?style=flat-square)
- [LLM-Economist](https://github.com/sethkarten/LLM-Economist) — Mechanism design with 3-1,000+ LLM agents; tackles optimal taxation. Supports GPT, Claude, Gemini, Llama. ![GitHub stars](https://img.shields.io/github/stars/sethkarten/LLM-Economist?style=flat-square)
- [EconAgent](https://github.com/tsinghua-fib-lab/ACL24-EconAgent) — LLM agents with personality traits simulating macro activities (ACL 2024). ![GitHub stars](https://img.shields.io/github/stars/tsinghua-fib-lab/ACL24-EconAgent?style=flat-square)
- [LLM-ABM Survey](https://github.com/tsinghua-fib-lab/LLM-Agent-Based-Modeling-and-Simulation) — Tsinghua's toolkit for LLM agent-based modeling. ![GitHub stars](https://img.shields.io/github/stars/tsinghua-fib-lab/LLM-Agent-Based-Modeling-and-Simulation?style=flat-square)

### Forecasting and Nowcasting

- [Now-Casting.com](https://www.now-casting.com/) — Real-time GDP forecasts for major economies, updated as data releases occur. By the methodology pioneers.
- [Project Spectrum](https://www.bis.org/about/bisih/topics/suptech_regtech/spectrum.htm) — BIS/ECB/Bundesbank: GenAI categorizes 34M+ products for **inflation nowcasting**. First central bank GenAI deployment for CPI.
- [Chronos](https://github.com/amazon-science/chronos-forecasting) — Amazon's pretrained time series models; Bolt variant is 250x faster. ![GitHub stars](https://img.shields.io/github/stars/amazon-science/chronos-forecasting?style=flat-square)
- [statsforecast](https://github.com/Nixtla/statsforecast) — Fast statistical forecasting for econometric time series. ![GitHub stars](https://img.shields.io/github/stars/Nixtla/statsforecast?style=flat-square)
- [uni2ts](https://github.com/SalesforceAIResearch/uni2ts) — Unified time series transformer models. ![GitHub stars](https://img.shields.io/github/stars/SalesforceAIResearch/uni2ts?style=flat-square)
- [Durbyn.jl](https://github.com/taf-society/Durbyn.jl) — Julia port of R's legendary `forecast` package.
- [emerging-trajectories](https://github.com/wgryc/emerging-trajectories) — LLM-based forecasting of political/economic events. ![GitHub stars](https://img.shields.io/github/stars/wgryc/emerging-trajectories?style=flat-square)

### DSGE and Structural Models

- [MacroModelling.jl](https://github.com/thorek1/MacroModelling.jl) — Julia DSGE toolkit. ![GitHub stars](https://img.shields.io/github/stars/thorek1/MacroModelling.jl?style=flat-square)
- [gEconpy](https://github.com/jessegrabowski/gEconpy) — DSGE toolkit in Python. ![GitHub stars](https://img.shields.io/github/stars/jessegrabowski/gEconpy?style=flat-square)
- [Deep Learning for Dynamic Econ](https://github.com/sischei/Deep_Learning_For_Dynamic_Econ) — Neural networks to solve DSGE models (course materials).
- [OpenSourceEconomics](https://github.com/OpenSourceEconomics) — JAX-compatible DC-EGM, Kalman filters, econ-project-templates.
- [optimagic](https://github.com/optimagic-dev/optimagic) — Numerical optimization for economists (formerly estimagic). ![GitHub stars](https://img.shields.io/github/stars/optimagic-dev/optimagic?style=flat-square)

---

## Literature Review and Research Discovery

- [Elicit](https://elicit.com/) — Research Agents (Dec 2025) synthesize up to 80 papers into a brief; 99.4% data extraction accuracy. 138M papers, Claude Opus-powered.
- [Consensus](https://consensus.app/) — "Consensus Meter" categorizes evidence as yes/no/mixed across 200M+ papers.
- [Undermind](https://www.undermind.ai/) — Autonomously reads hundreds of papers; structured reports with timeline, categories, foundational work. 10 free/month.
- [Scite](https://scite.ai/) — Classifies 1.5B+ citations as "supporting" or "contrasting." Scite Rankings: first AI-driven research ranking.
- [alphaXiv](https://www.alphaxiv.org/) — Line-by-line discussion on arXiv papers; AI paper analysis. Stanford AI Lab-endorsed.
- [ResearchRabbit](https://www.researchrabbit.ai/) — Rebuilt Oct 2025 with Litmaps; combines citation networks AND semantic similarity.
- [SciSpace](https://typeset.io/) — Deep Review with iterative search and Zotero integration. 280M papers.
- [Connected Papers](https://www.connectedpapers.com/) — Visual graphs of related papers from a seed paper.

---

## Economic Data and Analysis

### AI Data Analysis Platforms

- [OpenEcon](https://openecon.ai/) — Purpose-built for economists; query FRED, World Bank, IMF, Comtrade, Eurostat via natural language. Instant charts.
- [Julius AI](https://julius.ai/) — Upload datasets, ask questions in natural language; returns charts, regressions, reports. Supports R, Python, SQL.
- [Microsoft Data Formulator](https://github.com/microsoft/data-formulator) — Free, open-source: describe charts in English, get publication-quality output with Python code. ![GitHub stars](https://img.shields.io/github/stars/microsoft/data-formulator?style=flat-square)

### Economic Data Sources

- [Global Macro Database](https://www.globalmacrodata.com/) — Most comprehensive open-source macro stats: 241 countries, 1086-2024, 27 contemporary + 84 historical sources.
- [FRED API v2](https://fred.stlouisfed.org/docs/api/fred/) — Nov 2025: bulk retrieval of all series in any release. 800,000+ time series. Free.
- [Trading Economics API](https://tradingeconomics.com/api/) — 300,000+ indicators from 196 countries with Python/R packages.
- [fedfred](https://github.com/nsunder724/fedfred) — Modern Python client for FRED API at scale.

---

## Academic Writing and LaTeX

- [OpenAI Prism](https://prism.openai.com/) — **Free** LaTeX workspace (Jan 2026). Manages citations, converts Stata/R output to tables, whiteboard photos to equations. [Featured for economists](https://econ-jobs.com/media/openai-prism-ai-economists-research-papers/).
- [Overleaf AI Assist](https://www.overleaf.com/about/ai-features) — For 20M+ Overleaf users; LaTeX error fixing, table/equation generation from prompts or images.
- [Underleaf](https://www.underleaf.ai/) — Chrome extension: image-to-LaTeX (handwritten equations to code), smart citation generation.
- [Paperpal](https://paperpal.com/) — Academic writing assistant on Overleaf, Google Docs, Chrome; 3M+ users.
- [Thesify](https://www.thesify.ai/) — AI reviewer evaluating argumentation, methodology, and rigor.

---

## Document Processing and OCR

- [Docling](https://github.com/docling-project/docling) — IBM open-source: **0.97 table recognition accuracy**. Handles tables, equations, code. Apache-2.0. ![GitHub stars](https://img.shields.io/github/stars/docling-project/docling?style=flat-square)
- [Marker](https://github.com/datalab-to/marker) — PDF to Markdown/JSON at 122 pages/sec; multi-page table merging. Free for research. ![GitHub stars](https://img.shields.io/github/stars/datalab-to/marker?style=flat-square)
- [Mistral OCR 3](https://mistral.ai/news/mistral-ocr-3) — **$1-2 per 1,000 pages**; cursive, complex tables, low DPI. 97% cheaper than AWS Textract.
- [Transkribus](https://www.transkribus.org/) — Handwritten historical document transcription; 140+ AI models, 100+ languages. Essential for economic history.

---

## NLP and Sentiment for Economics

- [SentiBigNomics](https://github.com/consose/SentiBigNomics) — Sentiment analysis **designed for economic text**; aspect-based, negation handling, tense detection. Open-source.
- [FinBERT](https://huggingface.co/ProsusAI/finbert) — Fine-tuned BERT for financial sentiment; widely cited in econ/finance research.
- [FinVADER](https://github.com/PetrKorab/FinVADER) — VADER updated with financial lexicons. ![GitHub stars](https://img.shields.io/github/stars/PetrKorab/FinVADER?style=flat-square)
- [FinSentGPT](https://www.sciencedirect.com/science/article/pii/S1057521924002230) — Fine-tuned ChatGPT for financial sentiment; multilingual, tested on ECB Monetary Policy Decisions.

---

## Policy Analysis, Labor Market and Alternative Data

### Policy and Evidence Synthesis

- [ImpactAI](https://impactai.worldbank.org/) — World Bank DIME: GenAI synthesizes RCT evidence. Ask "what improves school attendance in Sub-Saharan Africa?" and get effect sizes. **Free**.
- [Meta-Mar](https://www.meta-mar.com/) — Free meta-analysis platform; AI reads PDFs and extracts quantitative outcomes. 5,800+ researchers.
- [Rayyan](https://www.rayyan.ai/) — AI screening for systematic reviews; 90% time reduction, 97-99% sensitivity. PRISMA flowcharts. 1M+ users.
- [Plural Policy](https://pluralpolicy.com/) — AI bill summarizer with version comparison and momentum indicators across U.S. jurisdictions.
- [PolicyEngine](https://github.com/PolicyEngine/policyengine-us) — Open-source U.S. tax-benefit microsimulation. ![GitHub stars](https://img.shields.io/github/stars/PolicyEngine/policyengine-us?style=flat-square)

### Labor Market Data

- [Revelio Labs](https://www.reveliolabs.com/) — 100M+ employment records; available via WRDS for academics. Launched Revelio Public Labor Statistics in 2025.
- [Lightcast](https://lightcast.io/) — 2.5B job postings, 800M profiles, 160+ countries. AI skills taxonomy.
- [LinkedIn Economic Graph](https://economicgraph.linkedin.com/) — Labor trends, skills migration, talent matching. Free for academic researchers.

### Spatial, Satellite and Alternative Data

- [CARTO Agentic GIS](https://carto.com/) — AI agents that reason with spatial data via natural language (Q4 2025).
- [FlyPix AI](https://flypix.ai/) — No-code custom AI models on satellite/drone imagery for economic measurement.
- [Stanford Satellite + AI](https://sustainability.stanford.edu/news/satellite-imagery-and-ai-reveal-development-needs-hidden-national-data) — HDI for 61,530 municipalities from satellite imagery (Nature Communications, Feb 2026).
- [Neudata](https://www.neudata.co/) — Alternative data intelligence; catalogs thousands of non-traditional data sources.

---

## Finance-Specific AI

- [FinGPT](https://github.com/AI4Finance-Foundation/FinGPT) — Open-source financial LLMs for sentiment, forecasting, reports. ![GitHub stars](https://img.shields.io/github/stars/AI4Finance-Foundation/FinGPT?style=flat-square)
- [Fin-R1](https://github.com/SUFE-AIFLM-Lab/Fin-R1) — Financial reasoning LLM by Shanghai University of Finance and Economics. ![GitHub stars](https://img.shields.io/github/stars/SUFE-AIFLM-Lab/Fin-R1?style=flat-square)
- [Dexter](https://github.com/virattt/dexter) — Autonomous financial research agent with task planning and real-time data. ![GitHub stars](https://img.shields.io/github/stars/virattt/dexter?style=flat-square)
- [awesome-quant](https://github.com/wilsonfreitas/awesome-quant) — Curated quantitative finance resources. ![GitHub stars](https://img.shields.io/github/stars/wilsonfreitas/awesome-quant?style=flat-square)

---

## Data Collection Tools

### Web Scraping

- [ScrapeGraphAI](https://github.com/ScrapeGraphAI/Scrapegraph-ai) — Open-source LLM-powered scraping; adapts to website changes automatically. ![GitHub stars](https://img.shields.io/github/stars/ScrapeGraphAI/Scrapegraph-ai?style=flat-square)
- [Firecrawl](https://www.firecrawl.dev/) — Webpages to structured markdown; AI extraction endpoint. Free for 500 pages.
- [Kadoa](https://www.kadoa.com/) — No-code AI extraction for financial and economic data. Free tier.

### Survey and Qualitative Research

- [Outset AI](https://outset.ai/) — Hundreds of AI-moderated interviews simultaneously via video/voice/text in 40+ languages. $21M raised.
- [Conveo](https://conveo.ai/) — AI video interviews with multimodal analysis; 100x faster, 75% cheaper than traditional.
- [ATLAS.ti](https://atlasti.com/) — AI Coding with GPT; reduces manual qualitative coding by 90%.
- [TheySaid](https://www.theysaid.io) — AI-moderated surveys with conversational follow-ups.

> **Warning:** [Nature](https://www.nature.com/articles/d41586-026-00221-8) reports AI chatbots infiltrating online surveys. Implement detection for MTurk/Prolific studies.

### Synthetic Data

- [Gretel](https://www.gretel.ai/) — Synthetic data with differential privacy; acquired by NVIDIA. [Open-source library](https://github.com/gretelai/gretel-synthetics).
- [MOSTLY AI](https://mostly.ai/) — High-fidelity synthetic datasets; GDPR/HIPAA compliant. Free tier.

---

## Papers and Books

### Key Papers

| Paper | Authors | Venue |
|-------|---------|-------|
| [Generative AI for Economic Research](https://www.aeaweb.org/articles?id=10.1257/jel.20231736) | Korinek (2023) | JEL |
| [AI Agents for Economic Research](https://www.nber.org/papers/w34202) | Korinek (2025) | NBER |
| [LLMs: An Applied Econometric Framework](https://www.nber.org/papers/w33344) | Ludwig, Mullainathan, Rambachan (2025) | NBER |
| [Deep Learning for Economists](https://www.aeaweb.org/articles?id=10.1257/jel.20241733) | Melissa Dell (2025) | JEL |
| [Economics in the Age of Algorithms](https://www.aeaweb.org/articles?id=10.1257%2Fpandp.20251118) | Mullainathan (2025) | AEA P&P |
| [Generative AI at Work](https://academic.oup.com/qje/article/140/2/889/7990658) | Brynjolfsson, Li, Raymond (2025) | QJE |
| [The Simple Macroeconomics of AI](https://academic.oup.com/economicpolicy/article-abstract/40/121/13/7728473) | Acemoglu (2025) | Economic Policy |
| [A.I. and Our Economic Future](https://www.nber.org/papers/w34779) | Jones (2026) | NBER |
| [Teaching Economics to the Machines](https://www.nber.org/papers/w34713) | Chen et al. (2026) | NBER |
| [DiD Causal Forests](https://onlinelibrary.wiley.com/doi/abs/10.1002/jae.70001) | Gavrilova et al. (2025) | J. Applied Econometrics |
| [ML Who to Nudge](https://www.gsb.stanford.edu/faculty-research/faculty/susan-athey) | Athey, Keleher, Spiess (2025) | J. Econometrics |
| [AI in Economics Research](https://onlinelibrary.wiley.com/doi/10.1111/joes.12694) | Bahoo et al. (2025) | J. Economic Surveys |

### Books

- **[Deep Learning for Economists](https://dell-research-harvard.github.io/projects/384econdl)** — Melissa Dell. JEL 2025 + companion notebooks.
- **[The Means of Prediction](https://www.amazon.com/Means-Prediction-Really-Works-Benefits-ebook/dp/B0FJ2NZW7D)** — Maximilian Kasy (Oxford). How AI works and who benefits. UChicago Press, 2025.
- **[The Scaling Era](https://www.dwarkesh.com/podcast)** — Dwarkesh Patel. Oral history from Amodei, Hassabis, Zuckerberg interviews.

---

## Courses, Conferences and Community

### Courses

- [Data Analysis with AI v2.0](https://gabors-data-analysis.com/ai-course/) — Gabor Bekes, CEU Vienna (2026). 12-week: LLMs for IV, DiD, simulations.
- [Economics of Transformative AI](https://digitaleconomy.stanford.edu/etai-course/) — Stanford. Slides and exercises available.
- [The Economics of AI](https://www.coursera.org/learn/economics-of-ai) — Korinek, UVA on Coursera.
- [genaiforecon.org](https://www.genaiforecon.org/) — Korinek's companion site; semi-annual updates on tools and techniques.
- [AI for Economists](https://sites.google.com/view/lastunen/ai-for-economists) — Jesse Lastunen's prompt-focused templates.
- [EconDL](https://dell-research-harvard.github.io/projects/384econdl) — Melissa Dell's Jupyter notebooks for deep learning in economics.
- [ML & Causal Inference](https://www.gsb.stanford.edu/faculty-research/labs-initiatives/sil/research/methods/ai-machine-learning/short-course) — Susan Athey, Stanford GSB.
- [ML and Economics at Oxford](https://maxkasy.github.io/home/ML_Econ_Oxford/) — Maximilian Kasy's reading group.
- [Using AI in Research and Teaching](https://github.com/paulgp/using-ai-in-research-and-teaching) — Paul Goldsmith-Pinkham, Yale SOM.

### Conferences (2025-2026)

- [ESIF Economics and AI+ML](https://www.econometricsociety.org/regional-activities/schedule/2026/06/16/2026-ESIFEconomics-and-AIML-Meeting) — Econometric Society, Cornell, June 2026.
- [NBER AI and Economic Measurement](https://www.nber.org/conferences/ai-and-economic-measurement-spring-2026) — Stanford, May 2026.
- [NBER Digital Economics and AI](https://www.nber.org/conferences/digital-economics-and-ai-meeting-spring-2026) — Spring 2026.
- [IESE Economics of AI](https://www.iese.edu/faculty-research/economics-ai-conference-2026/) — Barcelona, Feb 2026.

### Community

**Newsletters:** [genaiforecon](https://genaiforecon.substack.com/) (Korinek) | [Causal Inference](https://causalinf.substack.com/) (Cunningham) | [Autonomous Econ](https://autonomousecon.substack.com/) (Wong) | [One Useful Thing](https://www.oneusefulthing.org/) (Mollick)

**Podcasts:** [Dwarkesh Podcast](https://www.dwarkesh.com/podcast) | [Exponential View](https://podcasts.apple.com/us/podcast/azeem-azhars-exponential-view/id1172218725)

**People:** [Anton Korinek](https://genaiforecon.org/) (TIME100 AI) | [Scott Cunningham](https://causalinf.substack.com/) (@causalinf) | [Erik Brynjolfsson](https://twitter.com/erikbryn) (Stanford DEL) | [Antonio Mele](https://github.com/meleantonio/awesome-econ-ai-stuff) | [Melissa Dell](https://dell-research-harvard.github.io/) | [Sendhil Mullainathan](https://sendhil.org/)

**Institutions:** [NBER AI](https://www.nber.org/topics/artificial-intelligence) | [Stanford DEL](https://digitaleconomy.stanford.edu/) | [OECD.AI](https://oecd.ai/) | [World Bank ImpactAI](https://impactai.worldbank.org/)

---

## Appendix: General-Purpose AI

*These tools are widely known. We list them for completeness with notes on what economists specifically value.*

| Tool | Best For (per [AEI guide](https://www.aei.org/technology-and-innovation/ai-tools-for-economists-and-policy-analysts/)) |
|------|---------|
| [ChatGPT](https://chat.openai.com/) | Deep Research mode (500+ sources, analyst-grade reports) |
| [Claude](https://claude.ai/) | Coding (Stata, R, Python), long document analysis (200K context) |
| [Gemini](https://gemini.google.com/) | Writing/copyediting, visual reports, Google Workspace integration |
| [Perplexity AI](https://www.perplexity.ai/) | Academic Focus mode (peer-reviewed journals only), Wiley partnership |
| [DeepSeek R1](https://huggingface.co/deepseek-ai/DeepSeek-R1) | Open-source (MIT), self-hostable for data privacy |
| [NotebookLM](https://notebooklm.google.com/) | Document synthesis, Data Tables, Audio Overviews, 1M token context |
| [Claude Code](https://docs.anthropic.com/en/docs/claude-code) | Agentic terminal coding; [Cunningham](https://causalinf.substack.com/p/claude-code-changed-how-i-work-part) calls it transformative |
| [Cursor](https://cursor.com/) | AI-native code editor with Background Agents |
| [GitHub Copilot](https://github.com/features/copilot) | Agent Mode, [RStudio integration](https://docs.posit.co/ide/user/ide/guide/tools/copilot.html) |
| [OpenAI Codex](https://openai.com/codex/) | Parallel task execution, reusable agent skills |

---

## Contributing

Contributions welcome! See [CONTRIBUTING.md](CONTRIBUTING.md). Focus on tools **specific to economics** — we intentionally keep generic tools in the appendix.

---

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, the author has waived all copyright and related or neighboring rights to this work.
