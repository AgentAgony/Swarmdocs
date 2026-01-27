<div align="center">


  [![Python](https://img.shields.io/badge/Python-3.11+-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://python.org)
  [![Docker](https://img.shields.io/badge/Docker-Ready-2496ED?style=for-the-badge&logo=docker&logoColor=white)](https://docker.com)
  [![MCP](https://img.shields.io/badge/MCP-Compatible-00ADD8?style=for-the-badge&logo=data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMjQiIGhlaWdodD0iMjQiIHZpZXdCb3g9IjAgMCAyNCAyNCIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KPHBhdGggZD0iTTEyIDJMMiA3TDEyIDEyTDIyIDdMMTIgMloiIGZpbGw9IndoaXRlIi8+CjxwYXRoIGQ9Ik0yIDEyTDEyIDE3TDIyIDEyIiBzdHJva2U9IndoaXRlIiBzdHJva2Utd2lkdGg9IjIiLz4KPC9zdmc+)](https://modelcontextprotocol.io)
  [![License](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge)](LICENSE)


<div align="center">
  


## 🚀 The Vision

**Vexorbis** is a high performance squad of specialized AI agents that live inside your IDE. It uses algorithms to find bugs, audit your Git flow, and verify logic before you even hit save. It handles the grunt work so you can focus on building software.

### Origins & Inspiration

Vexorbis was born from the realization that while LLMs are powerful, they lack the deterministic rigor required for professional software engineering. Inspired by the orchestration patterns of OpenAI's original Swarm research, we've evolved those concepts into a production ready workforce that combines:
- **Algorithmic Precision**: AST analysis, formal verification, and statistical debugging.
- **Autonomous Workflows**: Self driven Git management and task synchronization.
- **Stateful Memory**: Context that survives across sessions and agents.



## 🏗️ Core Architecture

Vexorbis operates as a centralized **Orchestrator** that coordinates a decentralized squad of **Algorithmic Workers**.

```mermaid
graph TD
    subgraph "Workspace"
        User([Human])
        IDE([Antigravity / Cursor])
        PLAN[PLAN.md]
    end

    subgraph "Vexorbis Engine"
        Orchestrator[Orchestrator Loop]
        Blackboard[(Blackboard)]
        Memory[(Telemetry DB)]
    end

    subgraph Workers ["Specialized Workers"]
        HippoRAG[HippoRAG - Understanding]
        SBFL[Ochiai - Debugging]
        Z3[Z3 - Verification]
        GitRoles[Git Roles - Ship]
    end

    User --> IDE --> Orchestrator
    PLAN <--> Orchestrator
    Orchestrator <--> Blackboard
    Orchestrator --> Workers
```

## 🧠 The Three Pillars

1.  **Algorithmic Core**: We use deterministic algorithms (HippoRAG, Ochiai SBFL, Z3) to ensure that agent actions are grounded in codebase reality, not just probabilistic guesses.
2.  **Autonomous Workforce**: Specialized Git roles (Auditor, Scout, Triage) handle mundane project management and code quality tasks autonomously.
3.  **Active Governance**: Every action is audited via a Telemetry system. Self-healing loops detect and mitigate repeated failures automatically.


## 🤖 Specialized Workforce

Vexorbis assigns roles based on the task at hand. You can trigger them directly in your `PLAN.md` using flags.

| Role | Trigger Flag | Responsibility |
| :--- | :--- | :--- |
| **Feature Scout** | `feature_discovery=True` | Scans TODOs, proposes new features, and creates issues. |
| **Code Auditor** | `code_audit=True` | Performs security reviews and ensures adherence to style guides. |
| **Issue Triage** | `issue_triage_needed=True` | Analyzes backlog, suggests priorities, and applies labels. |
| **Branch Manager** | `git_create_pr=True` | Handles PR creation, merge conflicts, and branch hygiene. |

## ⚡ Get Moving

Getting set up takes less time than a coffee break.

1.  **[Lock In](./getting-started/installation.md)** — Grab the Docker image and get running.
2.  **[First Ship](./getting-started/quickstart.md)** — Run your first autonomous task and see the magic.
3.  **[Sync Your Editor](./getting-started/installation.md#ide-configuration)** — Support for Antigravity, Cursor, and Claude Desktop.

## 📖 The Deep Dive

Everything you need to master the workforce:

| Quick Start | The Vibe | Playbook | Reference |
|-----------------|----------|--------|-----------|
| [Intro Guide](getting-started/introduction.md) | [How it Works](concepts/architecture.md) | [Using PLAN.md](guides/plan-syntax.md) | [Tools List](reference/tools.md) |
| [Setup](getting-started/installation.md) | [Agent Logic](concepts/decision-logic.md) | [Git Workflow](guides/git-workflows.md) | [Config Settings](reference/configuration.md) |
| [First Mission](getting-started/quickstart.md) | [The 3 Pillars](concepts/three-pillars.md) | [Expert Debugging](guides/debugging.md) | [API Specs](reference/api.md) |
| | | [Custom Tools](guides/custom-tools.md) | [FAQ](reference/troubleshooting.md) |

---
</div>

