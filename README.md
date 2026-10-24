# Awesome-Scripting-IDE-Automation

# Top Scripting IDE & Automation Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on AI-Assisted Scripting, Terminal-Native Agents & Self-Hosted Visual Automation*  
**Last updated: March 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Scripting IDE & Automation**. These tools combine code editing with automation execution — letting you write a script, run it, inspect the output, and iterate without leaving the editor — with a spectrum running from AI-powered coding agents to visual automation IDEs and headless workflow engines.

**Examples** include Cline, Windsurf, Script Kit, DevChat, and OculiX (the category leaders).

**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, terminal-native agent execution, and transparent automation workflows — ideal for developers who want AI-assisted scripting without vendor lock-in, and automation engineers who need visual or code-first tooling they can run locally.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **Windsurf** — **The AI-powered code editor built around the Cascade agent.** Combines repository-aware context, multi-file editing, terminal actions, and conversational task planning in an IDE-style workspace . **Cascade can plan and apply multi-step coding changes**, run commands, inspect output, and iterate on implementation without leaving the editor . **Free entry option** alongside paid individual and team plans . **Best for developers wanting an agentic coding workspace** for repository-aware scripting, refactoring, and debugging, accepting that agent output still requires careful diff review and that large repositories make context selection less predictable .

- **Qoder** — **Alibaba's agentic coding platform with an IDE, JetBrains plugin, and CLI.** Built around **Quest Mode for long-running, multi-step delegation**, with **Repo Wiki** documenting project structure and architecture . **Free plan with bring-your-own API key** and a two-week Pro trial; Quest Mode and Repo Wiki require a paid plan . **Best for developers wanting to hand long, multi-step coding tasks to an agent**, especially those already inside JetBrains IDEs .

## Open-Source GitHub Projects

- **Cline** — **The battle-tested open-source autonomous coding agent for VS Code.** Apache 2.0 licensed, **5M+ installs** . **Step-by-step permission gating** for every file edit, command, and browser action — humans stay in the loop . **Works with any LLM** — Claude, OpenAI, Google, or local models via Ollama . **Full MCP support** with a built-in marketplace for extending agent capabilities . **Browser automation via Computer Use** lets the agent launch a browser, click, type, and capture screenshots for interactive debugging . **Terminal integration** with direct command execution and approval . **The honest trade-offs**: **VS Code only** (JetBrains arrives with the Teams plan), **pay-per-token costs add up for heavy agentic workloads**, and newer forks (Kilo, Roo) ship features faster than upstream . **Best for developers wanting a proven, permission-gated agent** inside VS Code with full model freedom and no extension cost .

- **Script Kit** — **The script-driven automation toolkit for macOS (and beyond).** Open-source core with **Script Kit Pro** sponsorship features . **Create, manage, and execute scripts efficiently** with a comprehensive SDK and user-friendly application that integrates with development environments . **Built-in debugger, script logging, and remote script execution** are shipped or planned . **Highly customizable** — extend functionality with custom scripts and integrations . **Best for developers on macOS** wanting a focused scripting automation tool with a polished launcher experience, accepting that Pro features require sponsorship and the setup is developer-oriented .

- **DevChat** — **The open-source workflow engine for crafting AI-powered scripts inside your IDE.** **Engage users through a chat panel within VS Code or IntelliJ**, facilitating completion of development tasks . **Create intelligent, automated workflows** utilizing various LLMs, tailored to your team's specific coding formats and processes . **Example workflows**: generating unit tests of a function, writing well-formatted commit messages, and automatically renaming poorly-named local variables . **Combines script flexibility, LLM capabilities, and a chat GUI** in one framework . **Best for teams needing bespoke AI workflows** that existing products don't support — especially those with specific coding conventions or multi-step automation needs .

- **OculiX** — **The visual automation IDE that drives any graphical interface by what it looks like.** MIT licensed, with **twenty years of lineage** from SikuliX and **91+ organizations** using it in production . **Pixel-perfect OpenCV-based template matching** with DPI awareness and five cascaded matching strategies . **Embedded Tesseract OCR** for text recognition, with PaddleOCR available for multilingual workloads . **Cross-platform** — Windows, macOS, and Linux with one script running everywhere . **Jython scripting** with full JVM interop, drop-in compatible with legacy SikuliX scripts . **Full VNC stack** for remote machine automation, **native SSH tunneling**, and **Android via ADB** without Appium or accessibility APIs . **Auditable execution** with optional Ed25519-signed, SHA-256-chained JSONL audit journal . **Best for anyone automating native desktop apps, virtualized desktops (Citrix, RDP, VNC), or Canvas/WebGL UIs** where selector-based tools cannot reach .

- **ECA (Editor Code Assistant)** — **The editor-agnostic AI coding tool via an LSP-inspired protocol.** Free, open-source (Clojure), supporting **VS Code, Emacs, Neovim, and IntelliJ** . **Multiple LLM providers** — OpenAI, Anthropic, GitHub Copilot, and Ollama for local models . **Chat, rewrite, and completion modes** . **Best for developers using non-mainstream editors** who want AI assistance without vendor lock-in, accepting that enterprise-grade polish and setup simplicity favor Cline or Windsurf .

### Additional Strong Open-Source Options

- **flyto-ai** — **Natural language to executable automation workflows.** Apache 2.0 licensed, **412 pre-built automation modules** across 78 categories (browser, HTTP, string, image, file, database, notification) . **Produces reusable YAML workflows** — not throwaway scripts — with **self-learning blueprints** that remember what worked (second-run tasks drop from 15s to 3s) . **Webhook and HTTP server** for triggering from Slack, n8n, or any HTTP client . **Best for non-developers** wanting to automate tasks through natural language and get schedulable, shareable workflows, or developers wanting an AI agent that builds automation rather than code changes .

- **Ducky IDE** — **The Ducky Script IDE with a built-in AI agent.** Open-source, IntelliJ-inspired layout with **multi-tab editor, syntax highlighting, autocomplete, and a beefier Ducky linter** . **Built-in AI agent powered by Google Gemini** with four modes (Agent, Ask, Plan, Ducky), streaming responses, tool calling, and slash commands . **Cursor-style power moves**: `Ctrl+K` inline AI edit, `Ctrl+L` focus chat, `Ctrl+P` quick-open . **Run controller** with live progress, stop/cancel, and problems panel . **Single-file Windows EXE** via PyInstaller . **Best for security researchers and automation enthusiasts** working with Ducky Script, especially those wanting AI assistance inside a lightweight IDE .

- **PyBreeze** — **The Python automation IDE with isolated subprocess execution.** **The editor process never runs your script** — every automation module launches as `python -m <package>` with `shell=False`, so a crash or infinite loop cannot take down the IDE . **Integrated modules**: APITestka (HTTP testing, mock servers, reports), AutoControl (mouse, keyboard, image recognition, record/playback), WebRunner (browser automation), LoadDensity (concurrent load simulation), MailThunder (SMTP), and TestPioneer (YAML test definitions) . **HTML/JSON/XML report generation** and email delivery . **Best for Python automation engineers** wanting a unified IDE covering API, GUI, web, and load testing with process isolation as a safety net .

- **OpenAF** — **The Java & JavaScript "swiss-army knife" for DevOps automation.** Apache 2.0 licensed, **minimal requirements and footprint**, extensible through opacks . **oJob** for structured job execution, **oafp** for data transformation, **nAttrMon** for monitoring, and **mini-a** for autonomous agent workflows using LLMs and MCP servers . **Self-contained and scriptable** — designed for automation challenges where installing a full stack is overkill . **Best for DevOps engineers** wanting a lightweight, extensible scripting automation runtime that runs anywhere Java runs .

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Scripting IDE and automation tools differ significantly in scope, execution model, and vendor lock-in. **Cline is the most battle-tested open-source coding agent** with permission gating and full model freedom, but its **pay-per-token costs scale with usage** and newer forks may outpace upstream . **Windsurf and Qoder are polished agentic IDEs** but tie you to their platforms and plans . **OculiX is the reference for visual desktop automation** but requires a different mindset than code-first scripting — it sees pixels, not selectors . **DevChat requires writing scripts** — it's a workflow engine, not a no-code tool . **Script Kit's Pro features require sponsorship** and its setup is developer-oriented . **flyto-ai produces workflows, not code changes** — it's for automation tasks, not software development .
- Self-hosted open-source solutions require proper runtime installation (Python for PyBreeze, Java for OpenAF, JVM for OculiX), API key management for AI features, and awareness that agent execution should be sandboxed or permission-gated where possible.

---

**Made for developers, automation engineers, and teams choosing scripting environments that match their workflow and execution model.**
Let's make scripting IDE and automation more open, permission-gated, and workflow-appropriate.
