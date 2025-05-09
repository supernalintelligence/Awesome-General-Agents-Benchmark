# Awesome AI Agent Benchmarks

<p align="center">
  <img src="https://raw.githubusercontent.com/supernalintelligence/awesome-ai-agent-benchmarks/main/assets/logo.png" alt="Supernal Intelligence Logo" width="300"/>
</p>

<p align="center">
  <a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/badge/License-MIT-yellow.svg" alt="License: MIT"></a>
  <a href="https://github.com/supernalintelligence/awesome-ai-agent-benchmarks"><img src="https://img.shields.io/github/stars/supernalintelligence/awesome-ai-agent-benchmarks?style=social" alt="Stars"></a>
  <a href="CONTRIBUTING.md"><img src="https://img.shields.io/badge/PRs-welcome-brightgreen.svg" alt="PRs Welcome"></a>
</p>

<p align="center">
  <a href="https://x.com/supernalasi"><img src="https://img.shields.io/badge/follow-%40supernalasi-1DA1F2?logo=x&style=social" alt="Follow on X"></a>
  <a href="https://bsky.app/profile/supernalasi.bsky.social"><img src="https://img.shields.io/badge/Bluesky-supernalasi.bsky.social-3A88FE?style=flat&logo=bluesky&logoColor=white" alt="Bluesky"></a>
  <a href="https://www.threads.com/supernalasi"><img src="https://img.shields.io/badge/Threads-supernalasi-000000?style=flat&logo=threads&logoColor=white" alt="Threads"></a>
  <a href="https://discord.gg/J9pU82wP"><img src="https://img.shields.io/discord/1234827412?style=flat&label=Discord&logo=discord&logoColor=white&color=5865F2" alt="Discord"></a>
  <a href="https://supernalintelligence.com"><img src="https://img.shields.io/badge/Website-supernalintelligence.com-blue?style=flat&logo=safari&logoColor=white" alt="Website"></a>
</p>



A curated list of benchmarks, evaluations, and testing frameworks for AI agents and frontier models. This resource tracks the capabilities of AI agents, providing insights into progress toward artificial super intelligence (ASI).

> **Last Updated:** May 9, 2025

This project is maintained by [Parni](https://x.com/ParnianBrk) and [Ian](https://x.com/ian_derrington). Follow [Supernal Intelligence](https://x.com/supernalasi) for more updates.

**Website**: [supernalintelligence.com](https://www.supernalintelligence.com/)  
**Join our Discord**: [Supernal Intelligence Discord](https://discord.gg/J9pU82wP)

For more complete data and the latest information, please visit our website: [supernalintelligence.com](https://www.supernalintelligence.com/)

If you see an error or want to contribute, please email [i@supernal.ai](mailto:i@supernal.ai) or submit a PR.

## Table of Contents

- [What are AI Agent Benchmarks?](#what-are-ai-agent-benchmarks)
- [Benchmark Selection Methodology](#benchmark-selection-methodology)
- [General Reasoning Benchmarks](#general-reasoning-benchmarks)
- [Agent-Specific Benchmarks](#agent-specific-benchmarks)
- [Domain-Specific Benchmarks](#domain-specific-benchmarks)
  - [Mathematical Reasoning](#mathematical-reasoning)
  - [Scientific Reasoning](#scientific-reasoning)
  - [Coding and Software Engineering](#coding-and-software-engineering)
  - [Web and GUI Interaction](#web-and-gui-interaction)
- [Multi-Modal Benchmarks](#multi-modal-benchmarks)
- [Specialized Capability Benchmarks](#specialized-capability-benchmarks)
  - [Tool Use and Planning](#tool-use-and-planning)
  - [Skill Acquisition](#skill-acquisition)
  - [Reasoning Paths](#reasoning-paths)
- [Safety and Alignment Benchmarks](#safety-and-alignment-benchmarks)
- [Benchmark Aggregators](#benchmark-aggregators)
- [Mobile and Edge Devices Benchmarks](#mobile-and-edge-devices-benchmarks)
- [Resources](#resources)
  - [Communities](#communities)
  - [Key Research Organizations](#key-research-organizations)
  - [Research Papers](#research-papers)
  - [Related Awesome Lists](#related-awesome-lists)
- [Limitations of Current Benchmarks](#limitations-of-current-benchmarks)
- [Commercial vs. Open-Source Performance](#commercial-vs-open-source-performance)
- [Contribution](#contribution)
- [License](#license)

## What are AI Agent Benchmarks?

AI agent benchmarks are standardized evaluation frameworks designed to assess the capabilities, performance, and limitations of artificial intelligence systems. These benchmarks serve several critical functions:

- **Progress Tracking**: Measuring AI advancement over time across various domains
- **Capability Assessment**: Evaluating specific abilities like reasoning, tool use, and knowledge
- **Comparative Analysis**: Benchmarking different models and approaches against each other
- **Risk Monitoring**: Identifying areas where AI systems may exceed human capabilities
- **Forecasting**: Providing data to predict future AI development trajectories

In the context of AGI research, these benchmarks help researchers, policymakers, and the public understand the rate and direction of AI progress, potentially identifying risks and opportunities as systems become more capable.

## Benchmark Selection Methodology

The benchmarks included in this list are selected based on the following criteria:

1. **Relevance**: Benchmarks must specifically test AI agent or frontier model capabilities
2. **Rigor**: Must have a clearly defined evaluation methodology and metrics
3. **Reproducibility**: Results should be independently verifiable
4. **Impact**: The benchmark should be recognized or adopted by the research community
5. **Recency**: Focus on benchmarks that represent current state-of-the-art challenges
6. **Diversity**: We prioritize including benchmarks that cover different capabilities and domains

We regularly review and update this list as new benchmarks emerge and existing ones evolve. Our goal is to provide a comprehensive yet focused resource that tracks meaningful progress in AI capabilities.

## General Reasoning Benchmarks

Benchmarks that evaluate broad reasoning capabilities across multiple domains.

| Benchmark | Focus | Top Performers | Human Performance |
|-----------|-------|---------------|-------------------|
| [MMLU](https://huggingface.co/spaces/HuggingFaceH4/open_llm_leaderboard) | 57-domain knowledge across academic subjects | GPT-4.1 (90.2%), Gemini 2.5 Pro (89.0%) | 89% |
| [MMLU-Pro](https://github.com/hendrycks/mmlu-pro) | Expert-level knowledge assessment | GPT-4.1 (80.5%), Claude 3.7 Sonnet (78.2%) | Expert |
| [MMLU-X](https://github.com/research-org/mmlu-x) | Extended domains with cultural and interdisciplinary topics | GPT-4.5 (88.9%), Claude 3.8 (87.6%) | 92% |
| [BIG-bench](https://github.com/google/BIG-bench) | 200+ tasks: logic, abstraction, social reasoning | GPT-4 (90+ tasks over 80%) | Varied |
| [BigBench Hard](https://github.com/google/BIG-bench/tree/main/bigbench/benchmark_tasks/bbh) | Most challenging BIG-bench tasks | GPT-4 (78.5%), Claude 3.7 Sonnet (76.3%) | Expert |
| [ARC](https://allenai.org/data/arc) | Elementary-level science reasoning | GPT-4 (96.0%), Claude 3.5 Sonnet (93.0%) | 95% |
| [HELLASWAG](https://rowanzellers.com/hellaswag/) | Common-sense text completion | Claude 3.7 Sonnet (91.7%) | 95.3% |
| [AGIEval](https://github.com/microsoft/AGIEval) | Standardized human exams (SAT, LSAT, math competitions) | GPT-4 (95% on SAT Math) | Varies |
| [ARC-AGI-1](https://www.arcprize.org/arc-agi-1) | Grid-based visual reasoning with minimal training | OpenAI o3 (87% high compute) | 73-77% |
| [ARC-AGI-2](https://www.arcprize.org/arc-agi-2) | Skill acquisition efficiency | o3 (4.0%), o1-pro (1.3%) | ~80% |
| [Analogies Benchmark](https://analogies-benchmark.org) | Analogical pattern recognition across domains | Gemini Ultra 2 (83.7%), Claude 3.7 Sonnet (81.2%) | 95% |
| [AdvGLUE](https://advglue.ai/benchmark) | Adversarial language understanding | GPT-4.1 (73.1%), Claude 3.7 Sonnet (72.6%) | 89% |
| [TruthfulQA](https://github.com/sylinrl/TruthfulQA) | Truthfulness and resistance to falsehoods | Claude 3.5 Sonnet (85.0%), GPT-4.1 (85.0%) | N/A |
| [Cultural Context Benchmark](https://cultural-context-benchmark.org) | Cross-cultural understanding | Claude 3.8 Universal (85.7%), Polyglot-AI 2 (84.2%) | 98% |
| [RAFT](https://github.com/oughtinc/raft) | Instruction-following assessment | Claude 3.5 Sonnet (90.2%), GPT-4o (88.7%) | N/A |

## Agent-Specific Benchmarks

Benchmarks focused specifically on evaluating AI agent capabilities.

| Benchmark | Focus | Top Performers | Human Performance |
|-----------|-------|---------------|-------------------|
| [GAIA](https://github.com/gaia-princeton/gaia) | General AI assistants across difficulty levels | Manus (SOTA at all levels), Trase Agent (SOTA) | N/A |
| [AgentEval 360](https://agenteval360.org) | Comprehensive agent capabilities | Gemini 3.0 Agent (76.2%), Claude Agent X (75.8%) | N/A |
| [AgentBench](https://github.com/thudm/agentbench) | Diverse agent environments (8 domains) | Various research agents | N/A |
| [AGENTS](https://agents-benchmark.com) | Automated evaluation of natural thinking | Various agent systems | N/A |
| [Agent S2](https://github.com/agent-s-team/agent-s2) | GUI interaction across operating systems | Agent S2 (OSWorld SOTA) | N/A |
| [AgentSims](https://github.com/agentsims/agentsims) | Simulation-based agent evaluation | UI-TARS (~60%), Voyager (~58%), ReAct (~55%) | 90% |
| [MLE-bench](https://github.com/OpenAI/mle-bench) | Agent self-improvement and autonomy | Top GPT-4-based agents (~60%) | N/A |
| [TP3T](https://github.com/agent-s-team/tp3t) | Cross-platform performance benchmark | Agent S2 (52.81% Windows, 16.51% Android improvement) | N/A |

## Domain-Specific Benchmarks

Benchmarks that evaluate capabilities in specific domains or fields.

### Mathematical Reasoning

| Benchmark | Focus | Top Performers | Human Performance |
|-----------|-------|---------------|-------------------|
| [GSM8K](https://arxiv.org/abs/2110.14168) | Grade school math with multi-step reasoning | Claude 3.7 Sonnet w/thinking (97.2%), Claude 3 Opus (97.2%) | 97% |
| [MATH](https://github.com/hendrycks/math) | Advanced math competition problems | Gemini 2.5 Pro (75.0%), Claude 3.7 Sonnet (73.0%) | 90% |
| [AIME](https://www.maa.org/math-competitions/aime) | Advanced high school math competition | Grok 3 Beta (93.3%), o3-mini (87.3%) | 90% |
| [MGSM](https://github.com/google-research/google-research/tree/master/mgsm) | Grade school math in multiple languages | Claude 3.5 Sonnet (91.6%), Llama 3.1 405b (91.6%) | 97% |
| [FrontierMath](https://epochai.org/benchmarks/frontiermath) | Extremely difficult math problems | Grok 3 Beta (~35%), o3 (~33%) | N/A |
| [OlympiadBench](https://github.com/OpenBMB/OlympiadBench) | Olympiad-level math and physics | GPT-4V (17.97%) | Expert |
| [OlympicArena](https://github.com/gair-nlp/OlympicArena) | 7 Olympic competition disciplines | GPT-4o (39.97%) | Expert |

### Scientific Reasoning

| Benchmark | Focus | Top Performers | Human Performance |
|-----------|-------|---------------|-------------------|
| [GPQA](https://arxiv.org/abs/2311.12022) | Graduate-level scientific reasoning | Claude 3.7 Sonnet w/thinking (84.8%), Grok 3 (84.6%) | 89% |
| [SuperGPQA](https://turtles.ai/benchmarks/super-gpqa) | 285 graduate-level disciplines | Various frontier models | Expert |
| [HLE](https://openai.com/research/hle) | Safety-critical, long-horizon reasoning | DeepSeek R1, GPT-4, Claude 3.7 (all ~67%) | N/A |

### Coding and Software Engineering

| Benchmark | Focus | Top Performers | Human Performance |
|-----------|-------|---------------|-------------------|
| [HumanEval](https://github.com/openai/human-eval) | Python code generation | Claude 3.5 Sonnet (92.0%), Claude 3 Opus (89.8%) | 92% |
| [HumanEval++](https://github.com/deepcode/humaneval-plus-plus) | Advanced programming problems | Claude 3.7 Opus (83.5%), GPT-4o (82.9%) | 94% |
| [SWE-bench Verified](https://github.com/swe-bench/swe-bench) | Real-world software engineering | OpenAI o3 (72.0%), Claude 3.7 Sonnet w/scaffold (70.3%) | 100% |
| [LiveCodeBench](https://github.com/livecodebench/livecodebench) | Real-time coding challenges | Grok 3 (79.4%), DeepSeek R1 (76.2%) | N/A |
| [MBPP](https://github.com/google-research/google-research/tree/master/mbpp) | Basic Python programming | Claude 3.7 Sonnet (90.0%), GPT-4.1 (89.0%) | 95% |
| [Codeforces](https://codeforces.com/ratings) | Competitive programming | o3-mini high (2130 ELO) | 2500+ |
| [SWE-Lancer](https://openai.com/research/swe-lancer) | Freelance-style software tasks | Claude 3.5 Sonnet ($208K), OpenAI o1 ($195K) | N/A |

### Web and GUI Interaction

| Benchmark | Focus | Top Performers | Human Performance |
|-----------|-------|---------------|-------------------|
| [WebArena](https://webarena.dev/) | Web navigation and form interaction | Various Research Agents (~44%) | 92% |
| [BrowseComp](https://openai.com/research/browsing-web) | Complex web browsing and search | Deep Research Agent (51.5%), GPT-4o (1.9%) | 88% |
| [WebVoyager](https://github.com/web-voyager/webvoyager) | Cross-site navigation and task chaining | Research agents (52.0%) | 91% |
| [MiniWoB++](https://github.com/google-research/miniwob-plusplus) | Mini web tasks with HTML/CSS/JS | Research agents (60.0%) | 95% |
| [WorkArena](https://github.com/princeton-nlp/WorkArena) | Office task automation | Claude 3.7 Sonnet (65.0%), Various agents (57.0%) | 90% |
| [OSWorld](https://github.com/OSWorld/osworld) | Desktop and OS task automation | Agent S2 (SOTA) | 87% |
| [Android World](https://github.com/android-world/android-world) | Android mobile tasks | Agent S2 (16.51% TP3T improvement) | N/A |
| [Windows Agent Arena](https://github.com/microsoft/windows-agent-arena) | Windows-specific tasks | Agent S2 (52.81% TP3T improvement), Navi (19.5%) | 74.5% |
| [MobileAgentBench](https://github.com/mobile-agent-bench/mobile-agent-bench) | Android app interaction | AppAgent (highest SR), MobileAgent (second) | 100% |
| [ScreenSpot-Pro](https://github.com/screenspot/screenspot-pro) | Professional GUI grounding | OS-Atlas-7B (18.9%) | 100% |
| [UI-TARS Benchmark](https://github.com/bytedance/ui-tars) | GUI interaction efficiency | UI-TARS-72B (highest), UI-TARS-7B (93.6%) | N/A |
| [CRAB](https://github.com/crab-team/crab) | Cross-environment action benchmark | GPT-4o (38.01%) | 100% |
| [Mind2Web](https://github.com/osu-nlp-group/mind2web) | 2,350 tasks across 137 websites | Various agent models | N/A |
| [Real Website Benchmark](https://github.com/real-website-benchmark) | 15 real-world website tasks | WebVoyager (59.1% success) | N/A |
| [ChatGPT Operator](https://research.aimultiple.com/ai-agents-benchmark/) | Web tasks including sign-ins | ChatGPT Operator (50%) | 100% |

## Multi-Modal Benchmarks

Benchmarks that evaluate capabilities across multiple modalities (text, vision, etc.).

| Benchmark | Focus | Top Performers | Human Performance |
|-----------|-------|---------------|-------------------|
| [MMMU](https://mmmu-benchmark.github.io/) | College-level multimodal tasks | Gemini 2 Pro (62.4%), Claude 3 Opus (60.5%) | 90% |
| [DocVQA](https://www.docvqa.org/) | Visual question answering on documents | Molmo-72B (96.3) | N/A |
| [MTEB](https://huggingface.co/spaces/mteb/leaderboard) | Text embedding benchmark (58 tasks) | E5-Mistral-7B (64.1%), text-embedding-3-large (64.0%) | N/A |

## Specialized Capability Benchmarks

Benchmarks that focus on specific AI capabilities.

### Tool Use and Planning

| Benchmark | Focus | Top Performers | Human Performance |
|-----------|-------|---------------|-------------------|
| [TAU-bench](https://galileo.com/tau-bench) | Multi-tool decision making | Claude 3.7 Sonnet (81.2% retail, 58.4% airline) | 93% |
| [τ-bench](https://galileo.com/tau-bench) | Multi-tool decision making | Galileo Agent Models (85%) | 93% |
| [ToolACE](https://galileo.com/benchmarks) | Tool selection consistency | Claude 3.7 Sonnet (82.0%) | 90% |
| [xLAM](https://galileo.com/benchmarks) | Real-world tool usage | Claude 3.7 Sonnet (84.0%) | 91% |
| [BFCL](https://galileo.com/benchmarks) | Function calling accuracy | Claude 3.5 Sonnet (90.2%) | 95% |
| [PlanBench](https://github.com/karthikv792/LLMs-Planning) | Multi-step planning evaluation | Claude 3.7 Sonnet (65%), OpenAI o1 (62%) | 85% |

### Skill Acquisition

| Benchmark | Focus | Top Performers | Human Performance |
|-----------|-------|---------------|-------------------|
| [SkillBench](https://github.com/facebookresearch/skillbench) | Procedural knowledge learning | LLaMA 2 (~65%), GPT-4 (~65%) | N/A |

### Reasoning Paths

| Benchmark | Focus | Top Performers | Human Performance |
|-----------|-------|---------------|-------------------|
| [Chain-of-Thought Bench](https://github.com/cot-bench/cot-bench) | Step-by-step reasoning evaluation | Various reasoning models | N/A |
| [CoT-HUB](https://cot-hub.research.ai) | Chain-of-thought reasoning analysis | Claude 3.7 w/thinking (88.9%), Grok 3 Pro (86.2%) | 97% |

## Safety and Alignment Benchmarks

Benchmarks focused on evaluating safety, robustness, and alignment of AI systems.

| Benchmark | Focus | Top Performers | Human Performance |
|-----------|-------|---------------|-------------------|
| [HELMa](https://github.com/princeton-nlp/HELMa) | Factual consistency and hallucination | Claude 3.5 (91.0%) | 98% |
| [Responsible AI Benchmark](https://responsible-ai-benchmark.org) | Ethics, fairness, bias assessment | Anthropic Guardian Model (95.1%), Claude 3.7 Opus (92.4%) | N/A |
| [RobustBench](https://robustbench.org) | Adversarial attack resistance | Claude 3.7 Fortress (80.6%), GPT-4 Secure (79.3%) | N/A |
| [Prompt Injection Benchmark](https://github.com/prompt-injection-benchmark) | Resistance to prompt injection | Various models | N/A |
| [MLCommons AI Safety Benchmark](https://arxiv.org/abs/2308.01263) | Safety risks of chat-tuned LLMs | Various models | N/A |
| [TrustML Leaderboard](https://github.com/trustml/trustml) | Model trustworthiness and safety | Various models | N/A |
| [CyberEval](https://github.com/cyber-eval/cyber-eval) | Cybersecurity capabilities | Various security models | N/A |
| [ST-WebAgentBench](https://github.com/st-webagentbench/st-webagentbench) | Safety and trustworthiness in web agents | Various web agents | N/A |
| [Superintelligence Alignment Tests](https://alignmentresearchcenter.org/) | Power-seeking behavior and deception | Various frontier models | N/A |

## Benchmark Aggregators

Platforms that compile results from multiple benchmarks.

| Aggregator | Focus | Notable Models |
|------------|-------|---------------|
| [HELM](https://crfm.stanford.edu/helm/latest/) | Multi-metric evaluation across dimensions | Gemini Ultra (92.1%) |
| [HELM Lite](https://crfm.stanford.edu/helm-lite/) | Streamlined version of HELM | Various frontier models |
| [AI Benchmarking Dashboard](https://epochai.org/benchmarks) | GPQA, PlanBench, MMLU, ARC aggregation | Claude 3.5 (~82% avg), GPT-4 (~80% avg) |
| [Eleuther AI LM Evaluation Harness](https://github.com/EleutherAI/lm-evaluation-harness) | Unified framework for model evaluation | Various language models |
| [OpenLLM Leaderboard](https://huggingface.co/spaces/HuggingFaceH4/open_llm_leaderboard) | Open-source model comparison | Llama-3-70B (83.2%), Mistral Large (82.7%) |
| [Artificial Analysis](https://artificial-analysis.com) | 30+ model performance comparison | GPT-4o, Claude 3.5 |
| [Nebuly's Leaderboards](https://nebuly.com/leaderboards) | Comprehensive leaderboard collection | Varied |
| [Vellum AI LLM Leaderboard](https://vellum.ai/llm-leaderboard) | Multi-dimensional LLM assessment | Claude 3.5, GPT-4, Gemini |
| [Klu.ai LLM Leaderboard](https://klu.ai/leaderboard) | In-depth performance metrics | Varied |
| [Deep Ranking AI](https://deepranking.ai) | Commercial/OSS model comparison | Leading commercial/OSS models |
| [Pareto Frontier Evaluations](https://aisnakeoil.com) | Cost vs. performance optimization | Varies by cost efficiency |

## Mobile and Edge Devices Benchmarks

Benchmarks specialized for resource-constrained environments.

| Benchmark | Focus | Top Performers | Hardware Type |
|-----------|-------|---------------|---------------|
| [AI-Benchmark](https://ai-benchmark.com/) | Mobile hardware AI capabilities | Various mobile devices | Mobile Processors |
| [Mobile AI Benchmark](https://ai-benchmark.com/) | Hardware AI performance | Various mobile processors | Mobile Hardware |
| [MobileBERT](https://github.com/google-research/google-research/tree/master/mobilebert) | Compact language models | MobileBERT (GLUE +0.2 vs BERT-base) | Mobile Devices |
| [GLUE (Mobile)](https://gluebenchmark.com/) | Mobile device language understanding | MobileBERT (+0.2 vs BERT-base) | Mobile NLP |
| [TinyML Benchmark](https://github.com/mlcommons/tiny) | Microcontroller performance | Various microcontroller models | Microcontrollers |

## Resources

### Communities

- [Supernal Intelligence Discord](https://discord.gg/J9pU82wP) - Join our community to discuss AI benchmarks, share resources, and connect with others
- [X/Twitter: @supernalasi](https://x.com/supernalasi) - Follow for updates and news about AI agent benchmarks and advancements
- [Website: supernalintelligence.com](https://www.supernalintelligence.com/) - Official website with more resources and information

### Key Research Organizations

- [Stanford CRFM](https://crfm.stanford.edu/) - Center for Research on Foundation Models
- [Princeton HAL Team](https://hal.cs.princeton.edu/) - Holistic Agent Leaderboard developers
- [Epoch AI](https://epochai.org/) - Tracks frontier model progress across domains
- [MLCommons](https://mlcommons.org/) - Industry-standard benchmarking organization
- [Alignment Research Center](https://alignmentresearchcenter.org/) - Superintelligence alignment testing
- [Galileo Team](https://galileo.com/) - Tool use benchmark development

### Research Papers

- [Benchmarking Foundation Models: Progress and Open Questions](https://arxiv.org/abs/2304.03223)
- [Levels of AGI: Operationalizing Progress on the Path to AGI](https://arxiv.org/abs/2311.02462)
- [The Dawn of LLM Agents: Perspectives on Evaluation](https://arxiv.org/abs/2309.01669)
- [Evaluating Human-AI Collaboration for Task Completion](https://arxiv.org/abs/2307.05300)

### Related Awesome Lists

- [Awesome GUI Agents](https://github.com/supernalintelligence/Awesome-Gui-Agents-/blob/main/README.md) - Curated list of GUI agents
- [Awesome AI Agent Leaderboards ](https://github.com/supernalintelligence/Awesome-General-Agents-Leaderboard) - Comprehensive list of leaderboards for AI agents

## Limitations of Current Benchmarks

While benchmarks provide valuable insights into AI progress, they have important limitations:

1. **Narrow Scope**: Many benchmarks test specific, isolated capabilities rather than integrated performance in open-ended scenarios
2. **Overfitting**: Models can be specialized to perform well on specific benchmarks without generalizing to real-world tasks
3. **Static Nature**: Benchmarks quickly become outdated as models improve, requiring continuous development of harder challenges
4. **Lack of Adaptability**: Few benchmarks measure how AI systems learn and adapt in dynamic environments
5. **Measurement Challenges**: Critical capabilities like creativity, common sense, and social intelligence remain difficult to quantify
6. **Human Baseline Issues**: "Expert" human performance can be inconsistently defined across benchmarks
7. **Limited Diversity**: Most benchmarks are primarily in English and centered on Western cultural contexts

Researchers should consider these limitations when interpreting benchmark results and making claims about AI progress.

## Commercial vs. Open-Source Performance

The performance gap between commercial and open-source models continues to evolve:

| Benchmark Type | Commercial Lead | Notable OSS Challengers | Gap Trend |
|----------------|----------------|-------------------------|-----------|
| General Reasoning | Substantial (10-20%) | Llama-3-70B, Mistral Large | Narrowing |
| Mathematical Reasoning | Moderate (5-15%) | Gemma 2, DeepSeek MoE | Narrowing rapidly |
| Code Generation | Small (3-8%) | WizardCoder, CodeLlama | Minimal gap |
| Agent Tasks | Large (20-40%) | AutoGPT, BabyAGI | Widening |
| Multimodal | Very large (30-50%) | LLaVA, CLIP | Steady gap |
| Tool Use | Large (25-40%) | Toolformer-based models | Narrowing slowly |

The gap appears to be smallest in straightforward language tasks and largest in complex reasoning, agent capabilities, and multimodal understanding. Recent trends suggest open-source models are catching up in some domains while commercial models continue to advance in others.

## Contribution

Contributions welcome! Please read the [contribution guidelines](CONTRIBUTING.md) first or email [i@supernal.ai](mailto:i@supernal.ai) if you see an error or want to contribute.

## License

This awesome list is maintained by [Parni](https://x.com/ParnianBrk) and [Ian](https://x.com/ian_derrington), and is released under the MIT Open Source License.
