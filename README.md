# Awesome AI for Economists

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![License: CC0-1.0](https://img.shields.io/badge/License-CC0_1.0-lightgrey.svg)](https://creativecommons.org/publicdomain/zero/1.0/)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](http://makeapullrequest.com)

> A curated list of AI tools, platforms, papers, courses, and resources at the intersection of artificial intelligence and economics — for economists, social scientists, and policy analysts.

---

## Contents

- [Korinek's Six Domains Framework](#korineks-six-domains-framework)
- [General-Purpose AI Assistants](#general-purpose-ai-assistants)
- [Coding and Development Tools](#coding-and-development-tools)
- [Literature Review and Research Discovery](#literature-review-and-research-discovery)
- [Data Analysis and Visualization](#data-analysis-and-visualization)
- [Causal Inference and Econometrics Libraries](#causal-inference-and-econometrics-libraries)
- [Economic Simulation and Agent-Based Models](#economic-simulation-and-agent-based-models)
- [Finance-Specific AI](#finance-specific-ai)
- [Foundational Papers and Reading](#foundational-papers-and-reading)
- [Courses and Learning Resources](#courses-and-learning-resources)
- [Blogs and Newsletters](#blogs-and-newsletters)
- [Institutional Resources](#institutional-resources)
- [Contributing](#contributing)
- [License](#license)

---

## Korinek's Six Domains Framework

Anton Korinek's 2023 paper *"Generative AI for Economic Research"* (Journal of Economic Literature) established the canonical framework for how economists can leverage AI. The framework identifies **six domains** where generative AI transforms the research workflow:

| Domain | Description | Example Tools |
|--------|-------------|---------------|
| **Ideation** | Brainstorming research questions, identifying gaps, generating hypotheses | ChatGPT, Claude, Gemini |
| **Writing** | Drafting, editing, summarizing, and translating academic text | ChatGPT, Claude, Gemini |
| **Literature Review** | Searching, synthesizing, and mapping the academic literature | Elicit, Consensus, Semantic Scholar |
| **Data Analysis** | Cleaning, exploring, and analyzing economic datasets | Code Interpreter, NotebookLM |
| **Coding** | Writing, debugging, and optimizing code (Stata, R, Python, Julia) | GitHub Copilot, Cursor, Claude Code |
| **Math** | Deriving equations, checking proofs, solving models symbolically | ChatGPT, Claude, Wolfram Alpha |

This framework is widely adopted in the profession and serves as a useful mental model for integrating AI into economic research.

---

## General-Purpose AI Assistants

- [ChatGPT](https://chat.openai.com/) — OpenAI's flagship model; best-in-class Deep Research mode for multi-step literature synthesis and long-form analysis.
- [Claude](https://claude.ai/) — Anthropic's assistant; excels at coding assistance, long document analysis (up to 200K context), and careful reasoning.
- [Gemini](https://gemini.google.com/) — Google's model with strong writing, copyediting, and integration with Google Workspace.
- [Perplexity AI](https://www.perplexity.ai/) — AI-powered search engine with inline citations; useful for quick fact-checking and sourced answers.

> **Note:** The American Enterprise Institute published a practical comparison of AI tools for economists and policy analysts. See [AEI — AI Tools for Economists and Policy Analysts](https://www.aei.org/technology-and-innovation/ai-tools-for-economists-and-policy-analysts/) for a side-by-side evaluation.

---

## Coding and Development Tools

- [GitHub Copilot](https://github.com/features/copilot) — AI pair programmer integrated into VS Code, JetBrains, and Neovim; supports Python, R, Stata, Julia, and more.
- [Cursor](https://cursor.sh/) — AI-native code editor built on VS Code with deep codebase awareness and multi-file editing.
- [Claude Code](https://docs.anthropic.com/en/docs/claude-code) — Anthropic's agentic CLI tool for terminal-based coding, debugging, and git workflows.
- [Stata-MCP](https://github.com/hanlulong/stata-mcp) — Model Context Protocol server for integrating Stata with AI assistants like Claude; enables AI-driven econometric workflows.
- [awesome-econ-ai-stuff](https://github.com/meleantonio/awesome-econ-ai-stuff) — Curated collection of AI skills, prompts, and workflows tailored to economic research.

---

## Literature Review and Research Discovery

- [Elicit](https://elicit.com/) — AI research assistant that searches 200M+ papers (via Semantic Scholar and OpenAlex) and extracts structured findings.
- [Consensus](https://consensus.app/) — AI-powered academic search engine across 200M+ papers with claim-level evidence synthesis.
- [ResearchRabbit](https://www.researchrabbit.ai/) — Visual literature mapping tool that discovers related papers and tracks citation networks over time.
- [Connected Papers](https://www.connectedpapers.com/) — Generates visual graphs of papers related to a seed paper, revealing clusters and influential works.
- [Semantic Scholar](https://www.semanticscholar.org/) — AI-powered academic search engine by the Allen Institute for AI with TLDR summaries and citation context.
- [Perplexity AI](https://www.perplexity.ai/) — Conversational search with inline academic citations; useful for rapid literature scoping.

---

## Data Analysis and Visualization

- [ChatGPT Code Interpreter](https://chat.openai.com/) — Upload datasets (CSV, Excel) directly to ChatGPT for exploratory analysis, visualization, and statistical modeling in Python.
- [NotebookLM](https://notebooklm.google.com/) — Google's AI notebook grounded in your uploaded documents; useful for synthesizing reports, PDFs, and datasets.
- [FRED](https://fred.stlouisfed.org/) — Federal Reserve Economic Data; 800,000+ time series from 100+ sources, with API access for programmatic retrieval.
- [World Bank Open Data](https://data.worldbank.org/) — Free, open access to global development data covering GDP, poverty, trade, health, and education.
- [DeepEcon.ai](https://deepecon.org/) — Open-source platform for computational economics with AI; combines economic modeling with machine learning tools.

---

## Causal Inference and Econometrics Libraries

- [EconML](https://github.com/py-why/EconML) — Microsoft/py-why library for machine learning-based causal inference and heterogeneous treatment effects. ![GitHub stars](https://img.shields.io/github/stars/py-why/EconML?style=flat-square)
- [CausalML](https://github.com/uber/causalml) — Uber's Python package for uplift modeling and causal inference with machine learning. ![GitHub stars](https://img.shields.io/github/stars/uber/causalml?style=flat-square)
- [DoWhy](https://github.com/py-why/dowhy) — Microsoft/py-why end-to-end causal inference library: model, identify, estimate, and refute causal effects. ![GitHub stars](https://img.shields.io/github/stars/py-why/dowhy?style=flat-square)
- [awesome-causality-algorithms](https://github.com/rguo12/awesome-causality-algorithms) — Comprehensive index of causal discovery and causal inference algorithms with code. ![GitHub stars](https://img.shields.io/github/stars/rguo12/awesome-causality-algorithms?style=flat-square)

---

## Economic Simulation and Agent-Based Models

- [AI Economist](https://github.com/salesforce/ai-economist) — Salesforce Research framework using multi-agent reinforcement learning to design and evaluate economic policies (taxation, redistribution). ![GitHub stars](https://img.shields.io/github/stars/salesforce/ai-economist?style=flat-square)
- [LLM-Economist](https://arxiv.org/abs/2503.18368) — 2025 research on using LLM-powered agents for economic simulation, exploring how language models replicate human economic behavior.

---

## Finance-Specific AI

- [FinGPT](https://github.com/AI4Finance-Foundation/FinGPT) — Open-source financial large language models for sentiment analysis, forecasting, and robo-advising. ![GitHub stars](https://img.shields.io/github/stars/AI4Finance-Foundation/FinGPT?style=flat-square)
- [awesome-quant](https://github.com/wilsonfreitas/awesome-quant) — Extensive curated list of libraries, tools, and resources for quantitative finance. ![GitHub stars](https://img.shields.io/github/stars/wilsonfreitas/awesome-quant?style=flat-square)
- [awesome-ai-in-finance](https://github.com/georgezouq/awesome-ai-in-finance) — Curated collection of machine learning and AI applications in financial markets. ![GitHub stars](https://img.shields.io/github/stars/georgezouq/awesome-ai-in-finance?style=flat-square)

---

## Foundational Papers and Reading

| Paper | Authors | Venue | Description |
|-------|---------|-------|-------------|
| [Generative AI for Economic Research: Use Cases and Implications for Economists](https://www.aeaweb.org/articles?id=10.1257/jel.20231736) | Korinek (2023) | Journal of Economic Literature | The canonical paper defining six domains where AI transforms economic research. |
| [AI Agents for Economic Research](https://www.nber.org/papers/w33788) | Korinek (2025) | NBER Working Paper | Explores how agentic AI systems can autonomously perform research tasks. |
| [How to Learn and Teach Economics with Large Language Models](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=4391863) | Cowen & Tabarrok | SSRN | Practical guide for integrating LLMs into economics pedagogy. |
| [Large Language Models: A Primer for Economists](https://www.bis.org/publ/work1218.htm) | BIS (2024) | BIS Working Papers | Accessible technical overview of LLM architectures for an economics audience. |
| [Large Language Models for Economic Research: Four Key Questions](https://cepr.org/voxeu/columns/large-language-models-economic-research-four-key-questions) | CEPR / VoxEU | VoxEU Column | Frames the core questions economists should ask about LLM adoption. |
| [Artificial Intelligence in Economics Research](https://onlinelibrary.wiley.com/doi/10.1111/joes.12696) | Bahoo et al. (2025) | Journal of Economic Surveys | Systematic review of 2,231 articles on AI in economics research. |

---

## Courses and Learning Resources

- [Economics of Transformative AI (EconTAI)](https://sites.google.com/view/econtai) — Stanford course exploring the economic implications of advanced AI systems.
- [genaiforecon.org](https://www.genaiforecon.org/) — Anton Korinek's companion site for "Generative AI for Economic Research"; updated semi-annually with new tools and techniques.
- [AI for Economists](https://www.aiforecon.org/) — Jesse Lastunen's prompt-focused resource with practical templates for economic research tasks.
- [Using AI in Research and Teaching](https://github.com/paulgp/using-ai-in-research-and-teaching) — Paul Goldsmith-Pinkham (Yale SOM) course materials on integrating AI into academic economics workflows.
- [Econometrics With Python](https://github.com/weijie-chen/Econometrics-With-Python) — Comprehensive Python-based econometrics tutorials covering OLS, IV, panel data, and more. ![GitHub stars](https://img.shields.io/github/stars/weijie-chen/Econometrics-With-Python?style=flat-square)
- [Guide2EconRA](https://github.com/jmshapir/Guide2EconRA) — Practical guide for economics research assistants covering data, code, and workflow best practices. ![GitHub stars](https://img.shields.io/github/stars/jmshapir/Guide2EconRA?style=flat-square)
- [BYU Library — Economics AI Tools Guide](https://guides.lib.byu.edu/economics/ai-tools) — Curated library guide covering AI tools relevant to economics research and coursework.

---

## Blogs and Newsletters

- [Marginal Revolution](https://marginalrevolution.com/) — Tyler Cowen and Alex Tabarrok's long-running economics blog; frequent and early coverage of AI and economics.
- [Economist Writing Every Day](https://economistwritingeveryday.com/) — Practical writing advice for economists with increasing focus on AI-assisted writing workflows.
- [One Useful Thing](https://www.oneusefulthing.org/) — Ethan Mollick's (Wharton) Substack on practical AI adoption in knowledge work and education.
- [The Rundown AI](https://www.therundown.ai/) — Daily newsletter covering the latest AI developments, tools, and applications.
- [genaiforecon Substack](https://genaiforecon.substack.com/) — Anton Korinek's update newsletter tracking new AI tools and techniques for economists.

---

## Institutional Resources

- [NBER — Artificial Intelligence](https://www.nber.org/topics/artificial-intelligence) — National Bureau of Economic Research working papers and conferences on AI and the economy.
- [AEI — AI Tools for Economists and Policy Analysts](https://www.aei.org/technology-and-innovation/ai-tools-for-economists-and-policy-analysts/) — American Enterprise Institute practical guide comparing AI tools for policy work.
- [OECD.AI Policy Observatory](https://oecd.ai/) — OECD toolkit for AI policy, governance frameworks, and cross-country comparisons.
- [Brookings — Generative AI and the Economy](https://www.brookings.edu/topics/artificial-intelligence/) — Research and commentary on AI's impact on labor markets, productivity, and regulation.
- [VoxDev — Generative AI for LMIC Research](https://voxdev.org/topic/technology-innovation) — Resources on how generative AI can support development economics research in low- and middle-income countries.

---

## Contributing

Contributions are welcome! Please read the following guidelines before submitting a pull request:

1. **Search existing entries** to avoid duplicates.
2. **Use the standard format:** `[Name](URL) — Brief description.`
3. **Keep descriptions concise** — one sentence, starting with a capital letter and ending with a period.
4. **Add new entries at the bottom** of the relevant section.
5. **Verify all links** are working and point to the correct resource.
6. **One pull request per addition/change** for easier review.

For major structural changes, please open an issue first to discuss.

---

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, the author has waived all copyright and related or neighboring rights to this work. See [LICENSE](LICENSE) for details.
