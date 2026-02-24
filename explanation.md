# Omni-Agent Workspace Explanation

## 🎯 The North Star
To automate 70-80% of your business ecosystem, spanning four core pillars: **System Pros AI**, **Altus AI (YouTube)**, **Skool Mentorship**, and **Personal Life**.

## 🏗️ The Architecture: Control Tower & Factory Floors (Option C)
We chose a hybrid architecture that provides the benefits of **Strict Data Separation** with the power of **Shared Global Intelligence**.

- **The Control Tower (`GEMINI.md`)**: The root router. It holds the overarching rules, understands that all 4 pillars exist, and orchestrates which specialized "Sub-Agent" is summoned when you type a command.
- **The Factory Floors (`/SystemPros`, `/AltusAI`, etc.)**: Each pillar has its own dedicated directory. The context, memories, and outputs for your business are physically walled off from your YouTube scripts or Personal goals. This creates a massive context window for each without toxic crossover (e.g., your YouTube agent will never accidentally read a sensitive System Pros client proposal).
- **The Tool Shed (`.agent/skills/`)**: Rather than rebuilding an "Apify scraper" 4 times, automations are stored globally as *skills*. Any pillar can borrow a tool from the shed, run it inside its own walled garden, and save the result locally.

## 🔄 Operational Flow
1. **Trigger**: You send a message (soon via Telegram or directly in the IDE). If you use a command like `/prime Skool`, the Master Orchestrator intercepts this.
2. **Context Load**: The Orchestrator loads `.agent/agents/skool.md` to adopt the precise persona, tone, and rules for Skool. It then ingests `/Skool/context/` and `/Skool/knowledge-base/` to understand the current state of that specific business.
3. **Execution**: The Skool agent performs tasks, accesses global skills if needed, and writes outputs securely to `/Skool/outputs/`. When you `/prime SystemPros`, the Skool context is wiped from active memory and replaced with System Pros data.
