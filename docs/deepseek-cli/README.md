# DeepSeek CLI (`deepseek`)

[DeepSeek CLI](https://github.com/surf1k/deepseek-cli) is a blazing-fast, lightweight command-line client, coding assistant, and Git workflow tool for DeepSeek-V3 and DeepSeek-R1 reasoning models written in pure Rust.

## Features

- **Blazing Fast**: Starts in milliseconds (<10ms) with zero runtime dependencies.
- **DeepThink / R1 Reasoning Stream**: Live visualization of inner reasoning tokens with timer and token count.
- **Git Assistant**: Automated Conventional Commits (`deepseek commit`) and deep diff reviews (`deepseek review`).
- **Natural Language Shell**: Convert prompt to executable shell commands (`deepseek sh "find large files"`).
- **Interactive REPL**: Multi-turn dialog with tab-autocompletion, clipboard copy (`/copy`), token statistics (`/tokens`), and session export (`/save`).
- **Context Caching & Speed Stats**: Real-time tokens/sec, elapsed time, and cache hit ratio.
- **Flexible File Attachments**: Supports line ranges (`-f main.rs:10-50`) and globs (`-f "src/**/*.rs"`).
- **Unix Piping**: Seamless integration with pipes (`git diff | deepseek "Explain this"`).

## Quick Start

```bash
cargo install --git https://github.com/surf1k/deepseek-cli
export DEEPSEEK_API_KEY="your-api-key"

# Interactive REPL
deepseek

# Git commit message generator
deepseek commit

# Code review
deepseek review
```

🔗 **Repository**: https://github.com/surf1k/deepseek-cli
