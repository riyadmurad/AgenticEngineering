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
│       └── webdev-agent.md       # Full-stack web development architect (SecuraDev)
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

You can switch agents mid-session or set a default in `opencode.json`.

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
    }
  },
  "default_agent": "agentic-engineer"
}
```

---

## Roadmap

- [ ] Add custom **skills** (specialized workflows with scripts and resources)
- [ ] Add domain-specific agents (DevOps, Data Engineering, Mobile, Security Audit)
- [ ] Add MCP server configurations
- [ ] Add OpenCode plugins
- [ ] Create agent evaluation harnesses

---

## License

MIT
