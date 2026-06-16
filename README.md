<div align="center">
    <h1>Awesome OPC: Agentic One-Person Company</h1>
</div>

<p align="center">
    <a href="https://github.com/sindresorhus/awesome"><img src="https://awesome.re/badge.svg" alt="Awesome list badge"></a>
    <a href="LICENSE"><img src="https://img.shields.io/badge/License-MIT-blue.svg" alt="MIT License"></a>
    <a href="CONTRIBUTING.md"><img src="https://img.shields.io/badge/PRs-welcome-brightgreen.svg" alt="PRs welcome"></a>
</p>

This repository curates papers, benchmarks, tools, reports, and legal context for **OPC**: AI-enabled **One-Person Company** and agentic company automation.

It is **not** a general LLM-agent survey list. The filter is: does this resource help one person use AI agents to perform company-level work such as research, product building, software delivery, marketing, sales, support, finance, operations, governance, or compliance?

## News

**[2026/05/30]** Refocused the repository around company-function automation. Broad agent surveys were removed unless they directly cover computer use, office/GUI/OS operation, or agent security for delegated business action.

## Overview

- [News](#news)
- [Overview](#overview)
- [Contributing](#contributing)
- [Scope](#scope)
- [Core OPC Evidence](#core-opc-evidence)
  - [Company-Level-Benchmarks-and-Business-Simulations](#company-level-benchmarks-and-business-simulations)
- [Company Functions](#company-functions)
  - [Research-and-Product](#research-and-product)
  - [Software-Engineering-and-Delivery](#software-engineering-and-delivery)
  - [Marketing-Sales-CRM-and-Support](#marketing-sales-crm-and-support)
  - [Finance-and-Operations](#finance-and-operations)
- [Execution Layer](#execution-layer)
  - [Computer-Use-Web-and-Office-Agents](#computer-use-web-and-office-agents)
  - [Tool-Use-API-and-MCP](#tool-use-api-and-mcp)
  - [Memory-and-Long-Term-Agent-State](#memory-and-long-term-agent-state)
  - [Virtual-Organization-and-Multi-Agent-Workflows](#virtual-organization-and-multi-agent-workflows)
- [Governance](#governance)
  - [Permissions-Secrets-and-Enterprise-Safety](#permissions-secrets-and-enterprise-safety)
- [OPC Context](#opc-context)
  - [Industry-Reports-and-Market-Signals](#industry-reports-and-market-signals)
  - [Legal-and-Corporate-Form](#legal-and-corporate-form)
- [OPC Reading Map](#opc-reading-map)

## Contributing

We welcome high-signal additions through pull requests. Please see [CONTRIBUTING.md](CONTRIBUTING.md).

## Scope

In this list, **OPC** means AI-enabled **One-Person Company**, not only the legal form called one person company in some jurisdictions.

### In Scope

- **Company-level work benchmarks**: agents evaluated on realistic professional tasks, economic deliverables, business simulations, office work, CRM, finance, software engineering, or long-horizon company operations.
- **Function-specific automation**: research/product, engineering, marketing, sales, customer support, finance, accounting, legal, operations, and reporting.
- **Execution interfaces**: web, browser, GUI, OS, Office, SaaS, command-line, code, data tools, and tool-use environments that let agents operate real work systems.
- **Virtual organizations**: multi-agent workflows that explicitly model roles, handoffs, SOPs, collaboration, or "AI company" structures.
- **Governance and safety**: permissions, secrets, auditability, contextual integrity, tool misuse, indirect prompt injection, and long-horizon reliability for delegated business actions.
- **Business/legal context**: solopreneur, nanocorp, zero-person company, single-shareholder company, one-person company, and small-business formation context.

### Out of Scope

- Generic LLM-agent surveys with no company-function mapping.
- Generic prompt-engineering, chatbot, or RAG resources unless they support a concrete company workflow.
- Broad reasoning, latent-space, or alignment papers unless they are used in an agentic work system.
- Toy multi-agent role-play without real tasks, tools, verification, or company-operation relevance.

## Core OPC Evidence

### Company-Level-Benchmarks-and-Business-Simulations

| Date     | Paper / Resource Title                                                                                                                                             | OPC Relevance                                                                                              | Code |
|----------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------|------|
| 2024/03  | [WorkArena: How Capable Are Web Agents at Solving Common Knowledge Work Tasks?](https://arxiv.org/abs/2403.07718)                                                  | Evaluates agents on enterprise ServiceNow tasks, a close proxy for back-office work a solo company must run. | [Github](https://github.com/ServiceNow/WorkArena) |
| 2024/05  | [WorkBench: A Benchmark Dataset for Agents in a Realistic Workplace Setting](https://arxiv.org/abs/2405.00823)                                                     | Provides realistic workplace tasks for testing whether agents can handle everyday professional work.          | [Github](https://github.com/olly-styles/WorkBench) |
| 2024/07  | [OfficeBench: Benchmarking Language Agents across Multiple Applications for Office Automation](https://arxiv.org/abs/2407.19056)                                   | Tests long-horizon office workflows that require switching across realistic applications and information sources. | [Github](https://github.com/zlwang-cs/OfficeBench) |
| 2024/07  | [WorkArena++: Towards Compositional Planning and Reasoning-based Common Knowledge Work Tasks](https://arxiv.org/abs/2407.05291)                                   | Extends workplace web tasks toward compositional planning, closer to real back-office task chains.            | [Github](https://github.com/ServiceNow/WorkArena) |
| 2024/12  | [TheAgentCompany: Benchmarking LLM Agents on Consequential Real World Tasks](https://arxiv.org/abs/2412.14161)                                                     | Simulates digital coworkers doing professional work through web browsing, coding, programs, and coworker communication. | [Github](https://github.com/TheAgentCompany/TheAgentCompany) |
| 2025/02  | [Vending-Bench: A Benchmark for Long-Term Coherence of Autonomous Agents](https://arxiv.org/abs/2502.15840)                                                        | A concrete tiny-business benchmark where an agent manages inventory, pricing, ordering, and fees over a long horizon. | - |
| 2025     | [Top of the CLASS: Benchmarking LLM Agents on Real-World Enterprise Tasks](https://openreview.net/pdf?id=RQjUpeINII)                                               | Evaluates agents on enterprise tasks, useful for checking whether digital workers can handle company operations. | [Github](https://github.com/Miking98/classic_benchmark) |
| 2025/08  | [OdysseyBench: Evaluating LLM Agents on Long-Horizon Complex Office Application Workflows](https://arxiv.org/abs/2508.09124)                                      | Tests long-horizon Word, Excel, PDF, email, and calendar workflows that match everyday solo-company office work. | - |
| 2025/09  | [APEX Benchmarks: The AI Productivity Index](https://www.mercor.com/apex/)                                                                                         | Measures whether agents can complete economically valuable knowledge-work cases in professional-service roles. | [Benchmark](https://www.mercor.com/apex/) |
| 2025/09  | [AI Playing Business Games: Benchmarking Large Language Models on Managerial Decision-Making in Dynamic Simulations](https://arxiv.org/abs/2509.26331)              | Uses business-game simulations to test repeated managerial decisions under changing market conditions.        | - |
| 2025/10  | [GDPval: Evaluating AI Model Performance on Real-World Economically Valuable Tasks](https://arxiv.org/abs/2510.04374)                                              | Measures real professional deliverables across occupations, useful for estimating which company tasks can be delegated. | [OpenAI](https://openai.com/index/gdpval/) |
| 2025/10  | [ManagerBench: Evaluating the Safety-Pragmatism Trade-off in Autonomous LLMs](https://arxiv.org/abs/2510.00857)                                                    | Focuses on managerial decision scenarios where agents must balance business goals against safe action.        | - |
| 2025/10  | [Can LLMs Help You at Work? A Sandbox for Evaluating LLM Agents in Enterprise Environments](https://arxiv.org/abs/2510.27287)                                      | Simulates enterprise software, HR, finance, and administration workflows with fragmented data and access control. | - |
| 2026/03  | [How Well Does Agent Development Reflect Real-World Work?](https://arxiv.org/abs/2603.01203)                                                                        | Maps agent benchmarks to occupations and skills, useful for checking whether OPC evaluations track real labor. | - |
| 2026/03  | [RetailBench: Evaluating Long-Horizon Autonomous Decision-Making and Strategy Stability of LLM Agents in Realistic Retail Environments](https://arxiv.org/abs/2603.16453) | Tests retail agents on long-horizon decisions, strategy stability, and business operations.                   | - |
| 2026/03  | [Can LLM Agents Be CFOs? A Benchmark for Resource Allocation in Dynamic Enterprise Environments](https://arxiv.org/abs/2603.23638)                                 | Tests budget and resource-allocation decisions in changing enterprise environments.                            | - |
| 2026/04  | [MarketBench: Evaluating AI Agents as Market Participants](https://arxiv.org/abs/2604.23897)                                                                        | Tests whether agents can estimate their own cost and success probability, a prerequisite for agent labor markets. | - |
| 2026/04  | [Market-Bench: Benchmarking Large Language Models on Economic and Trade Competition](https://arxiv.org/abs/2604.05523)                                             | Evaluates agents acting as retailers in a configurable multi-agent supply-chain economy.                      | - |
| 2026/04  | [YC-Bench: Benchmarking AI Agents for Long-Term Planning and Consistent Execution](https://arxiv.org/abs/2604.01212)                                               | Evaluates whether agents can maintain plans and execute consistently over longer business-like horizons.       | - |
| 2026/04  | [ClawsBench: Evaluating Capability and Safety of LLM Productivity Agents in Simulated Workspaces](https://arxiv.org/abs/2604.05172)                                | Evaluates agents across email, chat, calendar, docs, and drive services, combining productivity tasks with safety-critical cases. | - |
| 2026/04  | [Claw-Eval-Live: A Live Agent Benchmark for Evolving Real-World Workflows](https://arxiv.org/abs/2604.28139)                                                       | Adds a live benchmark for evolving workflow tasks, useful when agent work environments change over time.       | [Project](https://claw-eval-live.github.io) |
| 2026/05  | [JobBench: Aligning Agent Work With Human Will](https://arxiv.org/abs/2605.26329)                                                                                  | Shifts occupational-agent evaluation from replacement value to workflows experts actually want to delegate.    | - |

## Company Functions

### Research-and-Product

| Date     | Paper / Resource Title                                                                                                                        | OPC Relevance                                                                                                  | Code |
|----------|-----------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------|------|
| 2024/08  | [The AI Scientist: Towards Fully Automated Open-Ended Scientific Discovery](https://arxiv.org/abs/2408.06292)                                 | Demonstrates an end-to-end research loop: idea generation, coding, experiments, visualization, writing, and review. | [Github](https://github.com/SakanaAI/AI-Scientist) |
| 2024/10  | [ScienceAgentBench: Toward Rigorous Assessment of Language Agents for Data-Driven Scientific Discovery](https://arxiv.org/abs/2410.05080)     | Grounds research-agent claims in executable data-driven scientific tasks with expert validation.                  | [Leaderboard](https://hal.cs.princeton.edu/scienceagentbench) |
| 2025/01  | [Agent Laboratory: Using LLM Agents as Research Assistants](https://arxiv.org/abs/2501.04227)                                                  | Models a multi-agent research-assistant pipeline that can turn a human idea into report and code artifacts.       | - |
| 2025/02  | [Towards an AI co-scientist](https://arxiv.org/abs/2502.18864)                                                                                | Frames research automation as a supervised multi-agent collaborator rather than fully unsupervised autonomy.       | - |
| 2025/02  | [MLGym: A New Framework and Benchmark for Advancing AI Research Agents](https://arxiv.org/abs/2502.14499)                                     | Evaluates AI research agents on open-ended ML experimentation, iteration, and improvement tasks.                  | - |
| 2025/06  | [DeepResearch Bench: A Comprehensive Benchmark for Deep Research Agents](https://arxiv.org/abs/2506.11763)                                    | Measures deep research agents on PhD-level research tasks, directly relevant to solo-founder market and technical research. | [Github](https://github.com/Ayanami0730/deep_research_bench) |
| 2025/10  | [DRBench: A Realistic Benchmark for Enterprise Deep Research](https://arxiv.org/abs/2510.00172)                                               | Evaluates enterprise-style deep research agents on realistic evidence-gathering and synthesis requests.            | [Github](https://github.com/ServiceNow/drbench) |
| 2026/03  | [SciVisAgentBench: A Benchmark for Evaluating Scientific Data Analysis and Visualization Agents](https://arxiv.org/abs/2603.29139)            | Tests agents that turn scientific data into analysis and visualizations, a product-research and reporting primitive. | - |
| 2026/05  | [AutoResearch AI: Towards AI-Powered Research Automation for Scientific Discovery](https://arxiv.org/abs/2605.23204)                          | Surveys workflow-level research automation from grounding and hypothesis generation to validation and reporting.  | [Project](https://mr-tieguigui.github.io/AutoResearch-AI/) |
| 2026/05  | [EngiAI: A Multi-Agent Framework and Benchmark Suite for LLM-Driven Engineering Design](https://arxiv.org/abs/2605.19743)                    | Tests multi-agent engineering design workflows, expanding research/product automation beyond pure software tasks. | - |
| 2026/05  | [AI Research Agents Narrow Scientific Exploration](https://arxiv.org/abs/2605.27905)                                                          | Important cautionary evidence for OPC research agents: automation can amplify search while narrowing exploration. | - |

### Software-Engineering-and-Delivery

| Date     | Paper / Resource Title                                                                                                                        | OPC Relevance                                                                                                  | Code |
|----------|-----------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------|------|
| 2023/10  | [SWE-bench: Can Language Models Resolve Real-World GitHub Issues?](https://arxiv.org/abs/2310.06770)                                         | Core benchmark for delegating bug fixing and feature work to coding agents in real repositories.                  | [Github](https://github.com/SWE-bench/SWE-bench) |
| 2024/05  | [SWE-agent: Agent-Computer Interfaces Enable Automated Software Engineering](https://arxiv.org/abs/2405.15793)                                | Shows that agent-computer interfaces materially improve autonomous repository navigation, editing, and testing.   | [Github](https://github.com/SWE-agent/SWE-agent) |
| 2024/07  | [OpenHands: An Open Platform for AI Software Developers as Generalist Agents](https://arxiv.org/abs/2407.16741)                               | Provides an open runtime for agents that code, use the shell, browse, and run evaluations in sandboxed environments. | [Github](https://github.com/All-Hands-AI/OpenHands) |
| 2024/12  | [Training Software Engineering Agents and Verifiers with SWE-Gym](https://arxiv.org/abs/2412.21139)                                          | Introduces a trainable environment and verifier loop for improving real-world software engineering agents.        | [Github](https://github.com/SWE-Gym/SWE-Gym) |
| 2025/04  | [R2E-Gym: Procedural Environments and Hybrid Verifiers for Scaling Open-Weights SWE Agents](https://arxiv.org/abs/2504.07164)                | Builds scalable executable environments for training open-weight software-engineering agents.                    | - |
| 2025/09  | [SWE-Bench Pro: Can AI Agents Solve Long-Horizon Software Engineering Tasks?](https://arxiv.org/abs/2509.16941)                              | Raises the bar toward enterprise-grade, long-horizon software tasks that matter for real product delivery.        | [Scale](https://scale.com/blog/swe-bench-pro) |

### Marketing-Sales-CRM-and-Support

| Date     | Paper / Resource Title                                                                                                                        | OPC Relevance                                                                                                  | Code |
|----------|-----------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------|------|
| 2024/06  | [tau-bench: A Benchmark for Tool-Agent-User Interaction in Real-World Domains](https://arxiv.org/abs/2406.12045)                             | Tests agents handling retail and airline support conversations with policies, APIs, and simulated users.          | [Github](https://github.com/sierra-research/tau-bench) |
| 2024/11  | [CRMArena: Understanding the Capacity of LLM Agents to Perform Professional CRM Tasks in Realistic Environments](https://arxiv.org/abs/2411.02305) | Evaluates CRM service, analyst, and manager personas in a realistic customer-relationship workflow.               | [Github](https://github.com/SalesforceAIResearch/CRMArena) |
| 2025/05  | [CRMArena-Pro: Holistic Assessment of LLM Agents Across Diverse Business Scenarios and Interactions](https://arxiv.org/abs/2505.18878)       | Expands CRM-agent evaluation across more realistic business scenarios, interactions, and confidentiality constraints. | - |
| 2025/06  | [tau^2-bench: Evaluating Conversational Agents in a Dual-Control Environment](https://arxiv.org/abs/2506.07982)                              | Models service workflows where both customer and agent can act on the shared environment.                         | [Github](https://github.com/sierra-research/tau2-bench) |
| 2025/07  | [ECom-Bench: Can LLM Agent Resolve Real-World E-commerce Customer Support Issues?](https://arxiv.org/abs/2507.05639)                         | Focuses on multimodal e-commerce customer support, a natural OPC support and operations workload.                 | [Dataset](https://huggingface.co/datasets/Alibaba-NLP/EcomBench) |
| 2026/02  | [AD-Bench: A Real-World, Trajectory-Aware Advertising Analytics Benchmark for LLM Agents](https://arxiv.org/abs/2602.14257)                  | Tests advertising and marketing analytics agents over real business requests and tool-call trajectories.          | [Github](https://github.com/Emanual20/adbench-leaderboard) |

### Finance-and-Operations

| Date     | Paper / Resource Title                                                                                                                        | OPC Relevance                                                                                                  | Code |
|----------|-----------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------|------|
| 2023/11  | [FinanceBench: A New Benchmark for Financial Question Answering](https://arxiv.org/abs/2311.11944)                                           | Not an agent benchmark by itself, but a useful baseline for financial-document analysis and filing-grounded QA.   | [PDF](https://www.patronus.ai/financebench.pdf) |
| 2024/05  | [FinRobot: An Open-Source AI Agent Platform for Financial Applications using Large Language Models](https://arxiv.org/abs/2405.14767)         | Provides specialized financial agents for analysis, reporting, and decision support.                             | [Github](https://github.com/AI4Finance-Foundation/FinRobot) |
| 2026/03  | [FinToolBench: Evaluating LLM Agents for Real-World Financial Tool Use](https://arxiv.org/abs/2603.08262)                                    | Provides a runnable benchmark for auditable financial tool execution by agents.                                  | - |
| 2026/03  | [FinMCP-Bench: Benchmarking LLM Agents for Real-World Financial Tool Use under the Model Context Protocol](https://arxiv.org/abs/2603.24943) | Tests financial agents over real MCP tools, multi-tool chains, and multi-turn financial scenarios.               | - |
| 2026/06  | [BigFinanceBench: A Workflow-Grounded Benchmark for Financial-Research Agents](https://arxiv.org/abs/2606.03829)                            | Evaluates finance-research agents on workflow-grounded tasks, useful for solo-company financial analysis and reporting. | [Dataset](https://huggingface.co/datasets/RogoAI/big-finance-benchmark) |

## Execution Layer

### Computer-Use-Web-and-Office-Agents

| Date     | Paper / Resource Title                                                                                                                        | OPC Relevance                                                                                                  | Code |
|----------|-----------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------|------|
| 2023/06  | [Mind2Web: Towards a Generalist Agent for the Web](https://arxiv.org/abs/2306.06070)                                                          | Builds web-agent tasks from real websites, an early base for browser agents that operate SaaS and web tools.      | [Github](https://github.com/OSU-NLP-Group/Mind2Web) |
| 2023/07  | [WebArena: A Realistic Web Environment for Building Autonomous Agents](https://arxiv.org/abs/2307.13854)                                      | Establishes reproducible web tasks across realistic websites, a foundation for SaaS and browser automation.      | [Github](https://github.com/web-arena-x/webarena) |
| 2024/01  | [VisualWebArena: Evaluating Multimodal Agents on Realistic Visual Web Tasks](https://arxiv.org/abs/2401.13649)                               | Adds visual grounding for web tasks where screenshots and page appearance matter.                                | [Github](https://github.com/web-arena-x/visualwebarena) |
| 2024/01  | [WebVoyager: Building an End-to-End Web Agent with Large Multimodal Models](https://arxiv.org/abs/2401.13919)                                | Demonstrates an end-to-end multimodal web agent for real online tasks, relevant to browser-based company work.    | [Github](https://github.com/MinorJerry/WebVoyager) |
| 2024/04  | [OSWorld: Benchmarking Multimodal Agents for Open-Ended Tasks in Real Computer Environments](https://arxiv.org/abs/2404.07972)               | Evaluates agents on real desktop tasks across operating systems, close to how an OPC operator uses software.      | [Github](https://github.com/xlang-ai/OSWorld) |
| 2024/10  | [VideoWebArena: Evaluating Long Context Multimodal Agents with Video Understanding Web Tasks](https://arxiv.org/abs/2410.19100)              | Adds video and long-context understanding to web tasks, useful for agents that must inspect dynamic workflows.    | - |
| 2024/11  | [Large Language Model-Brained GUI Agents: A Survey](https://arxiv.org/abs/2411.18279)                                                        | Focused survey of GUI agents, action spaces, datasets, and evaluation for operating software interfaces.          | [Github](https://github.com/vyokky/LLM-Brained-GUI-Agents-Survey) |
| 2024/12  | [The BrowserGym Ecosystem for Web Agent Research](https://arxiv.org/abs/2412.05467)                                                          | Provides a unified environment for building and evaluating web agents.                                           | [Github](https://github.com/ServiceNow/BrowserGym) |
| 2025/01  | [AI Agents for Computer Use: A Review of Instruction-based Computer Control, GUI Automation, and Operator Assistants](https://arxiv.org/abs/2501.16150) | Reviews the instruction-to-action stack for agents controlling computers, GUIs, and browsers.                    | - |
| 2025/04  | [An Illusion of Progress? Assessing the Current State of Web Agents / Online-Mind2Web](https://arxiv.org/abs/2504.01382)                    | Reassesses web-agent progress on online tasks, a useful caution for OPC browser automation claims.                | - |
| 2025/05  | [OSUniverse: Benchmark for Multimodal GUI-navigation AI Agents](https://arxiv.org/abs/2505.03570)                                             | Evaluates multimodal GUI navigation agents across operating-system tasks and interfaces.                         | [Github](https://github.com/agentsea/osuniverse) |
| 2025/08  | [OS Agents: A Survey on MLLM-based Agents for General Computing Devices Use](https://arxiv.org/abs/2508.04482)                               | Reviews OS-level agents for computers and phones, including planning, grounding, personalization, safety, and privacy. | - |
| 2025/11  | [ProBench: Benchmarking GUI Agents with Accurate Process Information](https://arxiv.org/abs/2511.09157)                                      | Evaluates GUI agents with explicit process information, matching professional workflows that span multiple steps. | - |
| 2026/01  | [Terminal-Bench: Benchmarking Agents on Hard, Realistic Tasks in Command Line Interfaces](https://arxiv.org/abs/2601.11868)                 | Tests agents on realistic terminal tasks, covering the command-line execution layer used in technical operations. | [Github](https://github.com/harbor-framework/terminal-bench) |
| 2026/04  | [WindowsWorld: A Process-Centric Benchmark of Autonomous GUI Agents in Professional Cross-Application Environment](https://arxiv.org/abs/2604.27776) | Evaluates cross-application Windows workflows where agents must track process state across professional desktop tasks. | - |
| 2026/05  | [Workspace-Bench 1.0: Benchmarking AI Agents on Workspace Tasks with Large-Scale File Dependencies](https://arxiv.org/abs/2605.03596)         | Tests workspace tasks with large file dependencies, matching real solo-operator document and file workflows.      | - |
| 2026/05  | [Code as Agent Harness](https://arxiv.org/abs/2605.18747)                                                                                    | Surveys code as executable, verifiable, and stateful agent infrastructure for tool use, GUI/OS automation, DevOps, and enterprise workflows. | [Github](https://github.com/YennNing/Awesome-Code-as-Agent-Harness-Papers) |
| 2026/05  | [TerminalWorld: Benchmarking Agents on Real-World Terminal Tasks](https://arxiv.org/abs/2605.22535)                                         | Adds real-world terminal tasks, relevant to agents that run scripts, deployments, data jobs, and operational checks. | - |
| 2026/06  | [MedCUA-Bench: A Screenshot-Only Benchmark for Clinical Computer-Use Agents](https://arxiv.org/abs/2606.03203)                              | Tests screenshot-only computer-use agents in clinical software, a high-stakes example of regulated workflow automation. | - |

### Tool-Use-API-and-MCP

| Date     | Paper / Resource Title                                                                                                                        | OPC Relevance                                                                                                  | Code |
|----------|-----------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------|------|
| 2023/04  | [API-Bank: A Comprehensive Benchmark for Tool-Augmented LLMs](https://arxiv.org/abs/2304.08244)                                               | Early benchmark for tool-augmented agents that call APIs, a foundation for delegated business workflows.         | [Github](https://github.com/AlibabaResearch/DAMO-ConvAI/tree/main/api-bank) |
| 2023/05  | [Gorilla: Large Language Model Connected with Massive APIs](https://arxiv.org/abs/2305.15334)                                                | Connects models to large API ecosystems, relevant to agents operating company software through tools.            | [Github](https://github.com/ShishirPatil/gorilla) |
| 2024/08  | [ToolSandbox: A Stateful, Conversational, Interactive Evaluation Benchmark for LLM Tool Use Capabilities](https://arxiv.org/abs/2408.04682)   | Tests stateful conversational tool use, closer to real business workflows than one-shot API calls.               | [Github](https://github.com/apple/ToolSandbox) |
| 2025/08  | [MCPToolBench++: A Large Scale AI Agent MCP Tool Use Benchmark](https://arxiv.org/abs/2508.07575)                                           | Evaluates MCP-based tool discovery, selection, parameter control, and cross-tool planning across large tool ecosystems. | - |
| 2025/08  | [MCP-Bench: Benchmarking Tool-Using LLM Agents with Complex Real-World Tasks via MCP Servers](https://arxiv.org/abs/2508.20453)              | Evaluates agents across live MCP servers, including finance, travel, scientific computing, and academic search.   | - |
| 2025/12  | [MCPAgentBench: A Real-world Task Benchmark for Evaluating LLM Agent MCP Tool Use](https://arxiv.org/abs/2512.24565)                         | Focuses on real-world MCP tool-use tasks, useful for testing whether agents can safely operate tool integrations. | - |
| 2026/02  | [SkillsBench: Benchmarking How Well Agent Skills Work Across Diverse Tasks](https://arxiv.org/abs/2602.12670)                               | Evaluates reusable agent skills across diverse tasks, relevant to building auditable company-task playbooks.      | - |
| 2026/04  | [The Amazing Agent Race: Strong Tool Users, Weak Navigators](https://arxiv.org/abs/2604.10261)                                               | Distinguishes tool-use competence from navigation ability, a key gap for agents using real SaaS workflows.        | - |
| 2026/05  | [TOBench: A Task-Oriented Omni-Modal Benchmark for Real-World Tool-Using Agents](https://arxiv.org/abs/2605.16909)                           | Tests omni-modal tool-using agents on task-oriented real-world workflows.                                        | [Github](https://github.com/Pi3AI/TOBench) |

### Memory-and-Long-Term-Agent-State

| Date     | Paper / Resource Title                                                                                                                        | OPC Relevance                                                                                                  | Code |
|----------|-----------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------|------|
| 2024/10  | [LongMemEval: Benchmarking Chat Assistants on Long-Term Interactive Memory](https://arxiv.org/abs/2410.10813)                                | Tests long-term interactive memory, a prerequisite for agents remembering customers, projects, and decisions.    | [Github](https://github.com/xiaowu0162/LongMemEval) |
| 2025/02  | [A-MEM: Agentic Memory for LLM Agents](https://arxiv.org/abs/2502.12110)                                                                      | Proposes agentic memory mechanisms for persistent context across tasks and interactions.                         | - |
| 2025/07  | [MemoryAgentBench: Evaluating Memory in LLM Agents via Incremental Multi-Turn Interactions](https://arxiv.org/abs/2507.05257)                | Evaluates memory over incremental interactions, matching long-running solo-company workstreams.                  | - |
| 2026/04  | [Memory in the LLM Era: Modular Architectures and Strategies in a Unified Framework](https://arxiv.org/abs/2604.01707)                       | Surveys memory architectures that support long-horizon tasks, ongoing customer context, and agent self-improvement. | - |
| 2026/04  | [From Recall to Forgetting: Benchmarking Long-Term Memory for Personalized Agents](https://arxiv.org/abs/2604.20006)                         | Tests both remembering and forgetting, important for agents that handle personal, customer, or confidential data. | - |
| 2026/05  | [EvoMemBench: Benchmarking Agent Memory from a Self-Evolving Perspective](https://arxiv.org/abs/2605.18421)                                  | Evaluates whether agent memory can improve over time rather than merely store static context.                    | - |
| 2026/05  | [MemGym: a Long-Horizon Memory Environment for LLM Agents](https://arxiv.org/abs/2605.20833)                                                  | Provides a long-horizon environment for testing memory under repeated tasks and changing state.                  | - |

### Virtual-Organization-and-Multi-Agent-Workflows

| Date     | Paper / Resource Title                                                                                                                        | OPC Relevance                                                                                                  | Code |
|----------|-----------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------|------|
| 2023/07  | [ChatDev: Communicative Agents for Software Development](https://arxiv.org/abs/2307.07924)                                                    | Early "software company" pattern where specialized agents communicate through a development pipeline.            | [Github](https://github.com/OpenBMB/ChatDev) |
| 2023/08  | [MetaGPT: Meta Programming for A Multi-Agent Collaborative Framework](https://arxiv.org/abs/2308.00352)                                      | Encodes human SOPs into role-based multi-agent collaboration, directly relevant to virtual company design.        | [Github](https://github.com/FoundationAgents/MetaGPT) |
| 2023/08  | [AutoGen: Enabling Next-Gen LLM Applications via Multi-Agent Conversation](https://arxiv.org/abs/2308.08155)                                 | General framework for programmable multi-agent workflows with tools, human input, and conversational handoff.     | [Github](https://github.com/microsoft/autogen) |
| 2023/08  | [AgentVerse: Facilitating Multi-Agent Collaboration and Exploring Emergent Behaviors](https://arxiv.org/abs/2308.10848)                      | Studies dynamic agent groups and emergent collaboration, useful for thinking about team-like agent organizations. | [Github](https://github.com/OpenBMB/AgentVerse) |
| 2024/08  | [AutoGen Studio: A No-Code Developer Tool for Building and Debugging Multi-Agent Systems](https://arxiv.org/abs/2408.15247)                 | Gives solo operators a visual way to compose, debug, and evaluate reusable multi-agent workflows.                 | [Github](https://github.com/microsoft/autogen) |
| 2024/08  | [BattleAgentBench: A Benchmark for Evaluating Cooperation and Competition Capabilities of Language Models in Multi-Agent Systems](https://arxiv.org/abs/2408.15971) | Tests cooperation, competition, and task execution, useful for agent teams that must negotiate priorities and conflicts. | - |
| 2024/11  | [Magentic-One: A Generalist Multi-Agent System for Solving Complex Tasks](https://arxiv.org/abs/2411.04468)                                  | Uses an orchestrator to coordinate web, file, code, and terminal agents across open-ended digital work.            | [Github](https://github.com/microsoft/autogen) |
| 2025/01  | [Multi-Agent Collaboration Mechanisms: A Survey of LLMs](https://arxiv.org/abs/2501.06322)                                                   | Surveys actors, structures, strategies, and coordination protocols behind agent collaboration.                    | - |
| 2025/02  | [Beyond Self-Talk: A Communication-Centric Survey of LLM-Based Multi-Agent Systems](https://arxiv.org/abs/2502.14321)                       | Reviews communication goals and protocols for delegation, reporting, handoffs, and conflict resolution.           | - |
| 2025/03  | [MultiAgentBench: Evaluating the Collaboration and Competition of LLM Agents](https://arxiv.org/abs/2503.01935)                              | Benchmarks multi-agent coordination, collaboration, and competition patterns that virtual organizations must handle. | [Github](https://github.com/MultiagentBench/MARBLE) |
| 2026/03  | [Silo-Bench: Evaluating Distributed Coordination in Multi-Agent LLM Systems](https://arxiv.org/abs/2603.01045)                               | Tests whether agents can integrate distributed information, a core problem for role-based virtual companies.      | - |
| 2026/05  | [Beyond Individual Intelligence: Surveying Collaboration, Failure Attribution, and Self-Evolution in LLM-based Multi-Agent Systems](https://arxiv.org/abs/2605.14892) | Frames collaboration with failure attribution and self-evolution, important for debugging company-level agent teams. | - |

## Governance

### Permissions-Secrets-and-Enterprise-Safety

| Date     | Paper / Resource Title                                                                                                                        | OPC Relevance                                                                                                  | Code |
|----------|-----------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------|------|
| 2024/03  | [InjecAgent: Benchmarking Indirect Prompt Injections in Tool-Integrated Large Language Model Agents](https://arxiv.org/abs/2403.02691)        | Tests a core OPC risk: agents reading untrusted content and then misusing tools.                                 | [Github](https://github.com/uiuc-focal-lab/InjecAgent) |
| 2024/06  | [AgentDojo: A Dynamic Environment to Evaluate Prompt Injection Attacks and Defenses for LLM Agents](https://arxiv.org/abs/2406.13352)        | Evaluates tool-using agents under realistic prompt-injection attacks involving email, banking, travel, and web tasks. | [Github](https://github.com/ethz-spylab/agentdojo) |
| 2024/10  | [ST-WebAgentBench: A Benchmark for Evaluating Safety and Trustworthiness in Web Agents](https://arxiv.org/abs/2410.06703)                    | Tests safety and trustworthiness for web agents before they operate business websites and SaaS dashboards.        | - |
| 2024/10  | [AgentHarm: A Benchmark for Measuring Harmfulness of LLM Agents](https://arxiv.org/abs/2410.09024)                                           | Measures harmful agent behavior under tool-use settings, relevant before giving agents real business powers.      | [Github](https://github.com/centerforaisafety/AgentHarm) |
| 2025/04  | [WASP: Benchmarking Web Agent Security Against Prompt Injection Attacks](https://arxiv.org/abs/2504.18575)                                   | Focuses on prompt-injection risk in web agents, an unavoidable threat for browser-based company automation.       | - |
| 2025/04  | [MCP Safety Audit: LLMs with the Model Context Protocol Allow Major Security Exploits](https://arxiv.org/abs/2504.03767)                    | Shows how MCP tool integrations can enable malicious execution, remote access, or credential leakage.             | - |
| 2025/05  | [RedTeamCUA: Realistic Adversarial Testing of Computer-Use Agents in Hybrid Web-OS Environments](https://arxiv.org/abs/2505.21936)           | Red-teams computer-use agents across web and OS contexts where attacks can cross application boundaries.          | - |
| 2025/06  | [A Survey on Autonomy-Induced Security Risks in Large Model-Based Agents](https://arxiv.org/abs/2506.23844)                                  | Covers risks that appear because agents act autonomously: memory poisoning, tool misuse, reward hacking, and misalignment. | - |
| 2025/06  | [OS-Harm: A Benchmark for Measuring Safety of Computer Use Agents](https://arxiv.org/abs/2506.14866)                                        | Tests unsafe behavior in GUI and computer-use agents before they operate real desktops, files, and business apps. | - |
| 2025/06  | [Model Context Protocol at First Glance: Studying the Security and Maintainability of MCP Servers](https://arxiv.org/abs/2506.13538)         | Studies open-source MCP servers for vulnerabilities, tool poisoning, insecure descriptions, and maintainability risks. | - |
| 2025/08  | [MCPSecBench: A Systematic Security Benchmark and Playground for Testing Model Context Protocols](https://arxiv.org/abs/2508.13220)          | Evaluates MCP server and client attacks, tool poisoning, and protocol risks in agent tool ecosystems.             | [Github](https://github.com/ChristianCella/mcp-security-bench) |
| 2025/09  | [A Multi-Agent LLM Defense Pipeline Against Prompt Injection Attacks](https://arxiv.org/abs/2509.14285)                                      | Uses specialized defense agents to detect and neutralize prompt injection, a possible guardrail for OPC workflows. | - |
| 2025/09  | [SecureAgentBench: Benchmarking Secure Code Generation under Realistic Vulnerability Scenarios](https://arxiv.org/abs/2509.22097)            | Tests whether coding agents avoid introducing vulnerabilities in realistic development scenarios.                 | - |
| 2025/10  | [MCP Security Bench: Benchmarking Attacks Against Model Context Protocol in LLM Agents](https://arxiv.org/abs/2510.15994)                    | Benchmarks attacks against MCP-enabled agents, directly relevant to delegated tool and integration access.        | - |
| 2026/01  | [Protecting Agentic AI Workloads with Confidential Computing](https://confidentialcomputing.io/2026/01/20/protecting-agentic-ai-workloads-with-confidential-computing/) | Industry perspective on using confidential computing to isolate sensitive agent workloads and secrets.            | [Article](https://confidentialcomputing.io/2026/01/20/protecting-agentic-ai-workloads-with-confidential-computing/) |
| 2026/02  | [AgentDyn: A Dynamic Open-Ended Benchmark for Evaluating Prompt Injection Attacks of Real-World Agent Security System](https://arxiv.org/abs/2602.03117) | Adds dynamic, open-ended prompt-injection tasks across shopping, GitHub, and daily-life scenarios.                | [Github](https://github.com/leolee99/AgentDyn) |
| 2026/02  | [AgentLeak: A Full-Stack Benchmark for Privacy Leakage in Multi-Agent LLM Systems](https://arxiv.org/abs/2602.11510)                         | Tests privacy leaks through inter-agent messages, shared memory, and tool arguments in multi-agent workflows.     | - |
| 2026/02  | [AgentLAB: Benchmarking LLM Agents against Long-Horizon Attacks](https://arxiv.org/abs/2602.16901)                                          | Tests agent security against attacks that unfold over longer horizons rather than obvious single-turn traps.      | [Project](https://tanqiujiang.github.io/AgentLAB_main) |
| 2026/03  | [The Attack and Defense Landscape of Agentic AI: A Comprehensive Survey](https://arxiv.org/abs/2603.11088)                                  | Surveys agentic AI attacks and defenses, useful for threat modeling delegated company operations.                 | - |
| 2026/04  | [AgentHazard: A Benchmark for Evaluating Harmful Behavior in Computer-Use Agents](https://arxiv.org/abs/2604.02947)                         | Evaluates whether computer-use agents can stop action sequences that become harmful only in context.              | - |
| 2026/04  | [CI-Work: Benchmarking Contextual Integrity in Enterprise LLM Agents](https://arxiv.org/abs/2604.21308)                                      | Tests whether enterprise agents can share useful information without leaking sensitive context.                   | - |
| 2026/04  | [Owner-Harm: A Missing Threat Model for AI Agent Safety](https://arxiv.org/abs/2604.18658)                                                    | Frames risks where agents harm their deployer through credential misuse, data leakage, or unauthorized business actions. | - |
| 2026/04  | [Credential Leakage in LLM Agent Skills: A Large-Scale Empirical Study](https://arxiv.org/abs/2604.03070)                                   | Studies credential leakage through agent skills, a key risk when agents install or reuse third-party capabilities. | - |
| 2026/04  | [A Systematic Survey of Security Threats and Defenses in LLM-Based AI Agents: A Layered Attack Surface Framework](https://arxiv.org/abs/2604.23338) | Maps agent risks across model, cognition, memory, tool execution, multi-agent coordination, ecosystem, and governance layers. | - |
| 2026/05  | [When Agents Handle Secrets: A Survey of Confidential Computing for Agentic AI](https://arxiv.org/abs/2605.03213)                            | Reviews confidential-computing options for agents that hold credentials, customer data, financial data, or private business memory. | - |
| 2026/05  | [AgentTrap: Measuring Runtime Trust Failures in Third-Party Agent Skills](https://arxiv.org/abs/2605.13940)                                 | Measures runtime trust failures in third-party skills, relevant to agent skill supply chains and plugin safety.   | [Github](https://github.com/zhmzm/AgentTrap) |
| 2026/05  | [Toward Securing AI Agents Like Operating Systems](https://arxiv.org/abs/2605.14932)                                                         | Applies operating-system security ideas such as isolation, permissions, and communication control to agent systems. | - |
| 2026/05  | [DeltaBox: Scaling Stateful AI Agents with Millisecond-Level Sandbox Checkpoint/Rollback](https://arxiv.org/abs/2605.22781)                 | Provides fast sandbox checkpoint and rollback for stateful agents, useful for recoverable delegated actions.      | - |
| 2026/05  | [AgentSecBench: Measuring Prompt Injection, Privacy Leakage, and Tool-Use Integrity in LLM Agents](https://arxiv.org/abs/2605.26269)         | Unifies prompt injection, privacy leakage, and tool-use integrity tests for LLM agents.                           | - |
| 2026/06  | [ROGUE: Misaligned Agent Behavior Arising from Ordinary Utility Maximization](https://arxiv.org/abs/2606.00341)                              | Studies misaligned behavior that can emerge from ordinary utility maximization, relevant to business-goal agents. | - |
| 2026/06  | [AgentRedBench: Dynamic Redteaming and Integration-Aware Defense for LLM Agents over SaaS Integrations](https://arxiv.org/abs/2606.02240)    | Red-teams agents over SaaS integrations and evaluates defenses that account for integration context.              | - |

## OPC Context

### Industry-Reports-and-Market-Signals

| Date     | Resource Title                                                                                                                                 | OPC Relevance                                                                                                  | Code |
|----------|------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------|------|
| 2025/03  | [Which Economic Tasks are Performed with AI? Evidence from Millions of Claude Conversations](https://arxiv.org/abs/2503.04761)                | Uses large-scale AI usage data to show which economic tasks people already delegate to AI.                       | - |
| 2025     | [MIT 2025 AI Agent Index](https://aiagentindex.mit.edu/)                                                                                       | Tracks deployed agent products, capabilities, ecosystem shape, and safety features.                              | [PDF](https://aiagentindex.mit.edu/data/2025-AI-Agent-Index.pdf) |
| 2025     | [McKinsey: The state of AI in 2025](https://www.mckinsey.com/capabilities/quantumblack/our-insights/the-state-of-ai)                          | Gives business-function adoption context for agentic AI and the gap between pilots and scaled workflow impact.   | - |
| 2025     | [PwC AI Agent Survey 2025](https://www.pwc.ie/reports/ai-agent-survey.html)                                                                    | Enterprise adoption signal for agent deployments, expected ROI, governance, and implementation barriers.          | - |
| 2025     | [KPMG and University of Amsterdam zero-person company experiment](https://kpmg.com/nl/en/about-us/press-and-media/press-releases/2025/11/ai-zero-person-company-experiment.html) | One of the clearest public experiments asking whether agents can run company functions with human supervision.    | - |
| 2026/05  | [Token Economics for LLM Agents: A Dual-View Study from Computing and Economics](https://arxiv.org/abs/2605.09104)                            | Frames token cost, latency, collaboration overhead, and security cost as practical limits on agent-run companies. | - |
| 2026     | [Gusto 2026 New Business Formation Report](https://gusto.com/resources/gusto-insights/new-business-formation-2026)                             | Small-business formation data on how AI is changing who starts businesses and how founders launch operations.     | - |
| 2026     | [Stripe Sessions 2026: Indexing the economy](https://stripe.com/en-cz/sessions/2026/indexing-the-economy)                                      | Industry context for smaller, faster business entities, embedded finance, and nanocorp narratives.                | - |

### Legal-and-Corporate-Form

| Date     | Paper / Resource Title                                                                                                                        | OPC Relevance                                                                                                  | Code |
|----------|-----------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------|------|
| 2018     | ['One Person Company' under the Companies Act, 2013: A Critical Reappraisal](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3157951)     | Legal background for the Indian OPC form and its move from minimum-two-person company formation to single-member company formation. | - |
| 2022     | [One Person Company and Its Role in Promotion of Entrepreneurship in India](https://ijcrt.org/papers/IJCRT22A6066.pdf)                        | Connects the legal OPC structure to entrepreneurship promotion and limited-liability solo ownership.              | - |
| 2024     | [One-Person Limited Liability Company: Considering Company's Organ Governance of the Indonesian Legal Entities for Micro and Small Enterprises](https://ejournal.undip.ac.id/index.php/dlr/article/view/44378/0) | Studies governance issues in one-person limited liability companies for micro and small enterprises.              | - |
| 2025     | [A Study of the Concept of One Person Company in the Context of Company Law Reforms and Ease of Doing Business in India](https://ijrt.org/j/article/view/623) | Reviews OPC as a company-law reform for solo founders, MSMEs, and ease of doing business.                        | - |

## OPC Reading Map

For a compact path through this repository:

1. Start with **TheAgentCompany**, **GDPval**, **APEX**, **JobBench**, and **Vending-Bench** to define the OPC question as real work, not chatbot ability.
2. Read the company-function sections next: research/product, software delivery, CRM/support, marketing, finance, and operations.
3. Add **WebArena**, **WorkArena**, **OfficeBench**, **OSWorld**, **BrowserGym**, and the computer-use surveys when the agent must operate real software.
4. Read the tool-use, MCP, and memory sections when the agent must call APIs, use reusable skills, or maintain long-running customer/project context.
5. Use **ChatDev**, **MetaGPT**, **AutoGen**, and **AgentVerse** as early patterns for role-based virtual organization, but judge them against realistic task benchmarks.
6. Read **AgentDojo**, **InjecAgent**, **CI-Work**, **AgentDyn**, **MCP Safety Audit**, and the security surveys before giving agents real credentials, customer data, email, payments, production code, or legal workflows.
7. Use the industry and legal resources to keep the technical stack connected to actual solopreneurs, nanocorps, zero-person company experiments, and one-person legal entities.
