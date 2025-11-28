# 🌱 Spec Kit  
**Build high-quality software faster.**  
An open-source toolkit that helps you focus on product scenarios and predictable outcomes — instead of vibe-coding everything from scratch.

---

## 📚 Table of Contents

- 🤔 What is Spec-Driven Development?
- ⚡ Get Started
- 📽️ Video Overview
- 🤖 Supported AI Agents
- 🔧 Specify CLI Reference
- 📚 Core Philosophy
- 🌟 Development Phases
- 🎯 Experimental Goals
- 🔧 Prerequisites
- 📖 Learn More
- 📋 Detailed Process
- 🔍 Troubleshooting
- 👥 Maintainers
- 💬 Support
- 🙏 Acknowledgements
- 📄 License

---

## 🤔 What is Spec-Driven Development?

Spec-Driven Development **flips the traditional software workflow**:

❌ Old way:  
Specs → throwaway → code becomes primary.

✅ New way:  
Specs become **executable**, generating real implementations — not just guidance.

> You focus on *what* and *why*.  
> The system handles the *how*.

---

## ⚡ Get Started

### **1. Install Specify CLI**

#### **Option 1 — Persistent Install (Recommended)**

```bash
uv tool install specify-cli --from git+https://github.com/github/spec-kit.git
```

Use the tool:

```bash
specify init <PROJECT_NAME>
specify check
```

Upgrade:

```bash
uv tool install specify-cli --force --from git+https://github.com/github/spec-kit.git
```

#### **Option 2 — One-time Usage**

```bash
uvx --from git+https://github.com/github/spec-kit.git specify init <PROJECT_NAME>
```

**Benefits of persistent install:**

- Always available in PATH  
- No aliasing required  
- Easy management via `uv tool list`, `uv tool upgrade`, etc.

---

### **2. Establish Project Principles**

In your project folder, launch AI coding assistant.

Run:

```
/speckit.constitution
```

This creates **governing principles** for:

- Code quality  
- Testing  
- UX consistency  
- Performance  
- Architecture rules  

---

### **3. Create the Specification**

Focus on *what* to build, not how.

```
/speckit.specify Build an application that organizes photos into albums…
```

---

### **4. Create a Technical Implementation Plan**

Tell the system your tech stack:

```
/speckit.plan The application uses Vite with minimal libraries…
```

---

### **5. Break Down Into Tasks**

```
/speckit.tasks
```

This generates a **full actionable task list**.

---

### **6. Execute Implementation**

```
/speckit.implement
```

The AI agent will build your feature automatically.

---

## 📽️ Video Overview

Watch the official demo:  
*(Add your link or video thumbnail here)*

---

## 🤖 Supported AI Agents

| Agent | Support | Notes |
|-------|---------|--------|
| Claude Code | ✅ | |
| GitHub Copilot | ✅ | |
| Gemini CLI | ✅ | |
| Cursor | ✅ | |
| Qwen Code | ✅ | |
| opencode | ✅ | |
| Windsurf | ✅ | |
| Kilo Code | ✅ | |
| Auggie CLI | ✅ | |
| CodeBuddy CLI | ✅ | |
| Roo Code | ✅ | |
| Codex CLI | ✅ | |
| Amazon Q Dev CLI | ⚠️ | No custom arg support |
| Amp | ✅ | |

---

## 🔧 Specify CLI Reference

### Commands

| Command | Description |
|---------|-------------|
| `init` | Create new project |
| `check` | Check installed tools |

### Arguments & Options

| Option | Type | Description |
|--------|-------|--------------|
| `<project-name>` | Argument | Project directory |
| `--ai` | Option | AI engine (claude, gemini, copilot, cursor, etc.) |
| `--script` | Option | Script (sh or ps) |
| `--ignore-agent-tools` | Flag | Skip AI agent checks |
| `--no-git` | Flag | Skip git init |
| `--here` | Flag | Use current folder |
| `--force` | Flag | Overwrite existing directory |
| `--skip-tls` | Flag | Disable TLS check |
| `--debug` | Flag | Enable detailed logs |
| `--github-token` | Option | Provide GH token |

### Examples

```bash
specify init my-project
specify init my-project --ai claude
specify init --here --ai copilot
specify init . --force --ai copilot
specify init my-project --ai gemini --no-git
specify init my-project --ai claude --debug
specify check
```

---

## 🧠 Available Slash Commands

### Core Commands

| Command | Description |
|---------|-------------|
| `/speckit.constitution` | Create/update project rules |
| `/speckit.specify` | Define requirements |
| `/speckit.plan` | Create technical plan |
| `/speckit.tasks` | Generate tasks |
| `/speckit.implement` | Build the feature |

### Optional Commands

| Command | Description |
|---------|-------------|
| `/speckit.clarify` | Improve unclear specs |
| `/speckit.analyze` | Consistency checks |
| `/speckit.checklist` | Custom quality checklist |

---

## 🌍 Environment Variables

| Variable | Description |
|----------|--------------|
| `SPECIFY_FEATURE` | Select feature folder when not using branches |

---

## 📚 Core Philosophy

Spec-Driven Development focuses on:

- Intent-driven workflows  
- Multi-step refinement  
- Heavy AI reasoning  
- Technology-agnostic development  
- Clean separation of **spec → plan → tasks → implementation**

---

## 🌟 Development Phases

| Phase | Focus | Activities |
|--------|--------|------------|
| 0→1 / Greenfield | Build from scratch | Specs → plans → implementation |
| Creative Exploration | Try variations | Multiple stacks, UX ideas |
| Iterative Enhancement | Modernization | Improve legacy systems |

---

## 🎯 Experimental Goals

- Tech independence  
- Enterprise constraints  
- User-centric workflows  
- Creative + iterative dev  
- Parallel feature exploration  

---

## 🔧 Prerequisites

- Linux/macOS/Windows  
- Supported AI coding agent  
- Python 3.11+  
- Git  
- `uv` package manager  

---

## 📖 Learn More

- Full methodology  
- Deep-dive guides  
- Tutorials  

*(Add links if needed)*

---

## 📋 Detailed Process

*(Expandable section if needed in GitHub)*

---

## 🔍 Troubleshooting

### Git Credential Manager (Linux)

```bash
#!/usr/bin/env bash
set -e
wget https://github.com/git-ecosystem/git-credential-manager/releases/download/v2.6.1/gcm-linux_amd64.2.6.1.deb
sudo dpkg -i gcm-linux_amd64.2.6.1.deb
git config --global credential.helper manager
rm gcm-linux_amd64.2.6.1.deb
```

---

## 👥 Maintainers

- **Den Delimarsky** (@localden)  
- **John Lam** (@jflam)

---

## 💬 Support

For help, open a GitHub issue.

---

## 🙏 Acknowledgements

Based on the research and work of **Mohsin Raza**.

---

## 📄 License

Licensed under **MIT License**.

