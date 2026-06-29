# Agentic Engineering

A curated collection of self-built **AI agents** and **skills** for [OpenCode](https://opencode.ai) — designed to bring deep domain expertise, security rigor, and production-grade engineering standards into your development workflow.

Each agent is a drop-in `.md` definition that plugs directly into OpenCode's agent system via the `.opencode/agents/` directory. No frameworks to install, no servers to run — just structured prompts with purpose-built expertise.

---

## Project Structure

```
AgenticEngineering/
├── .opencode/
│   └── agents/
│       ├── agentic-engineer.md   # AI agent architecture & design specialist
│       ├── webdev-agent.md       # Full-stack web development architect (SecuraDev)
│       ├── orchestrator-agent.md # Master orchestrator & team lead (Nexus)
│       ├── reviewer-agent.md     # Technical code reviewer (Sentinel)
│       └── devsecops-agent.md    # DevSecOps engineer & security analyst (Aegis)
├── Agents/                       # Standalone agent artifacts (future use)
├── opencode.json                 # OpenCode configuration & agent registry
└── README.md
```

---

## Agents

### Architect — `agentic-engineer`

The world's foremost AI Agentic Engineer. Designs and builds production-grade AI agent systems with precision and ruthless efficiency.

**Core Capabilities:**
- Agent architecture patterns: ReAct, Plan-and-Execute, Reflexion, Multi-Agent, Hierarchical, State Machine, Event-Driven
- Framework expertise: LangChain, LangGraph, CrewAI, AutoGen, Semantic Kernel, Mastra, Vercel AI SDK
- Tool design: JSON Schema definitions, MCP servers, function calling, structured outputs
- Memory systems: RAG, vector stores (Pinecone, Weaviate, Chroma), knowledge graphs, episodic memory
- Prompt engineering: CoT, ToT, few-shot selection, guard rails, token budget optimization
- Observability & evaluation: LangSmith, Arize Phoenix, trajectory evaluation, LLM-as-judge

**Use when:** Designing agent systems, building multi-agent architectures, crafting prompts, integrating LLMs, or working with OpenCode's agent/skill/plugin infrastructure.

---

### SecuraDev — `webdev-agent`

The world's most experienced full-stack web development architect. Combines the depth of a principal engineer, the breadth of a polyglot technologist, and the rigor of a security researcher.

**Core Capabilities:**
- **20+ languages** — TypeScript, Python, Rust, Go, Java/Kotlin, C#, Ruby, PHP, Elixir, and more
- **Frontend mastery** — React/Next.js, Vue/Nuxt, Svelte/SvelteKit, Angular, Astro, Solid, Qwik with every rendering paradigm (CSR, SSR, SSG, ISR, RSC, Islands, Edge, Streaming)
- **Backend depth** — REST, GraphQL, gRPC, tRPC, WebSocket, SSE across 15+ server frameworks
- **Database landscape** — Relational, document, key-value, search, vector, time-series, graph, wide-column
- **Architecture patterns** — DDD, Hexagonal, Clean Architecture, Microservices, CQRS, Event Sourcing, Saga, 12-Factor
- **Security first** — OWASP Top 10 compliance, security headers, secrets management, dependency scanning, 19-point security checklist
- **Performance engineering** — Core Web Vitals optimization, bundle analysis, query optimization, CDN/edge strategies
- **Accessibility** — WCAG 2.2 AA compliance, semantic HTML, ARIA, keyboard navigation, screen reader testing
- **DevOps & Cloud** — CI/CD pipelines, Docker, Kubernetes, Terraform/Pulumi, AWS/GCP/Azure, full observability stack
- **Testing strategy** — Unit, integration, E2E, performance, security, accessibility, chaos, and contract testing

**Use when:** Building websites, web apps, APIs, CLIs, libraries, infrastructure, or any coding task. Enforces OWASP security, WCAG accessibility, and production-grade standards on every task.

---

### Nexus — `orchestrator-agent`

The master orchestrator and team lead. The most sophisticated agent that plans, delegates, and coordinates across all specialist agents to deliver complex projects with precision.

**Core Capabilities:**
- **Strategic planning** — Break complex projects into atomic, delegatable tasks with dependency mapping
- **Intelligent delegation** — Match tasks to the right agent with context packages and handoff contracts
- **Coordination patterns** — Sequential pipelines, parallel execution, iterative refinement workflows
- **Quality governance** — Enforce quality gates across architecture, code, security, performance, and accessibility
- **Risk management** — Proactive identification and mitigation of technical, security, and timeline risks
- **Team leadership** — Leads Architect, SecuraDev, Sentinel, and Aegis agents as a unified team

**Use when:** Managing complex multi-agent workflows, planning large projects, decomposing tasks across specialists, or coordinating team-wide delivery.

---

### Sentinel — `reviewer-agent`

The elite technical reviewer and quality guardian. The last line of defense before code reaches production — reviews all code from `webdev-agent` and assigns revision tasks when improvements are needed.

**Core Capabilities:**
- **Code quality review** — Correctness, readability, maintainability, performance, security analysis
- **Architecture validation** — Design pattern compliance, boundary respect, scalability assessment
- **Testing review** — Validate test coverage, test quality, and testing strategy
- **Security review** — Deep security analysis beyond automated scanning
- **Structured feedback** — Categorized issues (Critical/Major/Minor) with specific remediation guidance
- **Revision task assignment** — Clear tasks with acceptance criteria assigned back to `webdev-agent`

**Use when:** Reviewing code quality, enforcing best practices, validating architecture decisions, or assigning revision tasks after code review.

---

### Aegis — `devsecops-agent`

The elite DevSecOps engineer and security analyst. A master of both offensive and defensive security — from exploit development and malware analysis to enterprise SIEM/SOAR/EDR operations.

**Core Capabilities:**
- **Offensive security** — Penetration testing, exploit development (C, Python, Rust, JS, Ruby, PowerShell, Assembly), buffer overflows, ROP chains, browser/kernel exploits
- **Malware analysis** — Static & dynamic analysis, reverse engineering (Ghidra, IDA Pro, Radare2), unpacking, algorithm extraction, attribution
- **Penetration testing** — Web apps, APIs, networks, wireless, mobile — full OWASP exploitation
- **SIEM expertise** — Microsoft Sentinel (KQL), Splunk (SPL), Chronicle (YARA-L) — detection rules, hunting, workbooks
- **EDR operations** — Microsoft Defender XDR, Carbon Black Cloud, CrowdStrike Falcon — alerts, live response, policy enforcement
- **Cloud security** — WIZ Platform — agentless scanning, misconfiguration detection, identity threat detection, CDR
- **SOAR** — Chronicle SOAR, Sentinel Playbooks — automated incident response, enrichment, case management
- **Threat hunting** — MITRE ATT&CK mapping, hypothesis-driven hunting, beaconing detection, lateral movement analysis
- **DevSecOps pipelines** — SAST (Semgrep, CodeQL), DAST (OWASP ZAP), SCA (Snyk, Dependabot), container security, IaC scanning, secrets detection
- **Incident response** — NIST SP 800-61 process, forensics (disk, memory, network), malware triage

**Use when:** Security assessments, penetration testing, malware analysis, reverse engineering, building security pipelines, configuring SIEM/SOAR/EDR, threat hunting, or incident response.

---

## Getting Started

### Prerequisites

- [OpenCode](https://opencode.ai) installed

### Setup

1. **Clone the repo:**
   ```bash
   git clone https://github.com/riyadmurad/AgenticEngineering.git
   cd AgenticEngineering
   ```

2. **Copy agents into your project** (or symlink):
   ```bash
   # Copy to your own project's .opencode/agents/ directory
   cp -r .opencode/agents/ /path/to/your-project/.opencode/agents/
   ```

3. **Or use this repo directly** as your OpenCode workspace:
   ```bash
   cd AgenticEngineering
   opencode
   ```

### Using the Agents

Once configured, agents are available in OpenCode's agent selector:

- **`agentic-engineer`** (default) — For AI agent design and architecture tasks
- **`webdev-agent`** — For all coding, web development, and infrastructure tasks
- **`orchestrator-agent`** — For complex multi-agent workflows and project coordination
- **`reviewer-agent`** — For code review, quality assurance, and revision task assignment
- **`devsecops-agent`** — For security analysis, penetration testing, malware analysis, and DevSecOps

You can switch agents mid-session or set a default in `opencode.json`.

### Agent Team Workflow

The agents are designed to work together as a coordinated team:

```
User Request
     │
     ▼
┌─────────────────┐
│   Orchestrator   │  ← Plans, decomposes, delegates
│     (Nexus)      │
└────────┬─────────┘
         │
    ┌────┴────┬──────────┬──────────┐
    ▼         ▼          ▼          ▼
┌────────┐ ┌────────┐ ┌────────┐ ┌────────┐
│Architect│ │SecuraDev│ │Sentinel│ │ Aegis  │
│(Agent  │ │(WebDev)│ │(Review)│ │(SecOps)│
│Engineer)│ │        │ │        │ │        │
└────────┘ └────────┘ └────────┘ └────────┘
```

1. **Orchestrator** receives the request and creates an execution plan
2. Tasks are delegated to specialist agents based on expertise
3. **SecuraDev** builds the code, **Architect** designs agent systems
4. **Sentinel** reviews all code and assigns revision tasks if needed
5. **Aegis** performs security analysis and validates security controls
6. **Orchestrator** coordinates handoffs and ensures quality gates are met

---

## Configuration

The `opencode.json` file registers all agents and sets the default:

```json
{
  "$schema": "https://opencode.ai/config.json",
  "agent": {
    "agentic-engineer": {
      "description": "Expert AI Agent Engineer...",
      "mode": "primary",
      "color": "accent"
    },
    "webdev-agent": {
      "description": "World-class full-stack web development architect...",
      "mode": "primary",
      "color": "success"
    },
    "orchestrator-agent": {
      "description": "Master orchestrator and team lead...",
      "mode": "primary",
      "color": "magenta"
    },
    "reviewer-agent": {
      "description": "Elite technical code reviewer...",
      "mode": "primary",
      "color": "yellow"
    },
    "devsecops-agent": {
      "description": "Elite DevSecOps engineer and security analyst...",
      "mode": "primary",
      "color": "red"
    }
  },
  "default_agent": "agentic-engineer"
}
```

---

## Roadmap

- [x] Core agents: Architect, SecuraDev, Nexus, Sentinel, Aegis
- [ ] Add custom **skills** (specialized workflows with scripts and resources)
- [ ] Add domain-specific agents (Data Engineering, Mobile, Cloud Architecture)
- [ ] Add MCP server configurations
- [ ] Add OpenCode plugins
- [ ] Create agent evaluation harnesses
- [ ] Add agent communication protocols and shared memory

---

## License

MIT
