# DeepSeek CLI (`deepseek`)

[DeepSeek CLI](https://github.com/surf1k/deepseek-cli) is a blazing-fast, lightweight command-line client and terminal coding assistant for DeepSeek-V3 and DeepSeek-R1 reasoning models written in pure Rust.

## Features

- **Blazing Fast**: Starts in milliseconds with minimal resource footprint.
- **DeepThink / R1 Reasoning Stream**: Live visualization of inner reasoning tokens before the final answer.
- **Interactive REPL**: Multi-turn dialog with command history, multiline input, and session saving (`/save`).
- **Unix Piping**: Seamless integration with pipes (`git diff | deepseek "Write a commit message"`).
- **Multi-File Context**: Attach local code files with `-f <file>`.
- **Zero-Friction Setup**: Easy configuration with `deepseek config set-key <KEY>` or `DEEPSEEK_API_KEY`.

## Quick Start

```bash
cargo install --git https://github.com/surf1k/deepseek-cli
export DEEPSEEK_API_KEY="your-api-key"
deepseek "Explain the difference between Arc and Rc in Rust"
```

🔗 **Repository**: https://github.com/surf1k/deepseek-cli
