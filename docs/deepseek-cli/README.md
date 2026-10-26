# DeepSeek CLI (`deepseek`)

[DeepSeek CLI](https://github.com/surf1k/deepseek-cli) is a blazing-fast, open-source autonomous coding agent, terminal assistant, and Git workflow tool for DeepSeek-V3 and DeepSeek-R1 reasoning models written in pure Rust.

It brings the **full Claude Code & OpenCode experience** to the terminal, powered by DeepSeek API and local LLMs.

## Features

- 🤖 **Autonomous Coding Agent (`deepseek agent`)**: Replicates the Claude Code agentic loop. Autonomously reads files, performs surgical string edits, runs shell commands, searches code, and iterates until the task is solved.
- 🎨 **Visual Diff Engine**: Surgical file edits are previewed in color-coded unified diff format (`+`/`-`) before applying.
- 🛡️ **Interactive Safety & Permissions**: Read-only tools run safely; mutating actions (`edit_file`, `write_file`, `bash`) require approval (`[y/n/a]`), with an `--auto` flag for background tasks.
- 🧠 **Project Memory**: Automatically detects and reads `DEEPSEEK.md`, `CLAUDE.md`, or `AGENTS.md` instructions from your repository.
- ⚡ **Blazing Fast**: Starts in milliseconds (<10ms) with zero runtime dependencies.
- 💭 **DeepThink / R1 Reasoning Stream**: Live visualization of inner reasoning tokens with timer and token count.
- 🛠️ **Git Assistant**: Automated Conventional Commits (`deepseek commit`) and deep diff reviews (`deepseek review`).
- 🐚 **Natural Language Shell**: Convert prompt to executable shell commands (`deepseek sh "find large files"`).
- 💬 **Interactive REPL**: Multi-turn dialog with tab-autocompletion, clipboard copy (`/copy`), token statistics (`/tokens`), and session export (`/save`).
- 📊 **Context Caching & Speed Stats**: Real-time tokens/sec, elapsed time, and cache hit ratio.
- 📂 **Flexible File Attachments**: Supports line ranges (`-f main.rs:10-50`) and globs (`-f "src/**/*.rs"`).

## Quick Start

```bash
cargo install --git https://github.com/surf1k/deepseek-cli
export DEEPSEEK_API_KEY="your-api-key"

# Autonomous coding agent (Claude Code in pure Rust)
deepseek agent "Fix the timeout panic in src/api.rs and run cargo test"

# Interactive REPL
deepseek

# Git commit message generator
deepseek commit

# Code review
deepseek review
```

🔗 **Repository**: https://github.com/surf1k/deepseek-cli
