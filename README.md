# Copilot Helper Pro

[![Version](https://img.shields.io/visual-studio-marketplace/v/vicanent.copilot-helper-pro?style=flat-square)](https://marketplace.visualstudio.com/items?itemName=vicanent.copilot-helper-pro)
[![Downloads](https://img.shields.io/visual-studio-marketplace/d/vicanent.copilot-helper-pro?style=flat-square)](https://marketplace.visualstudio.com/items?itemName=vicanent.copilot-helper-pro)
[![Rating](https://img.shields.io/visual-studio-marketplace/r/vicanent.copilot-helper-pro?style=flat-square)](https://marketplace.visualstudio.com/items?itemName=vicanent.copilot-helper-pro)
[![License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat-square)](LICENSE)
[![VS Code](https://img.shields.io/badge/VS%20Code-1.104.0%2B-blue.svg?style=flat-square)](https://code.visualstudio.com/)

An extension that provides model support for GitHub Copilot Chat, including ZhipuAI, MiniMax, MoonshotAI, DeepSeek, Alibaba Cloud Bailian, and custom OpenAI/Anthropic compatible models.

## Features

- Multiple AI Model Support
    - ZhipuAI (GLM Coding Plan)
    - MiniMax (Coding Plan)
    - MoonshotAI (Kimi For Coding)
    - DeepSeek
    - Antigravity (Google Cloud Code)
        - Streaming responses with real-time output
        - Rate limit monitoring and automatic fallback
        - Quota tracking with usage statistics
        - Multi-account support with auto-switching
        - Signature-based request validation
        - Backoff and retry strategies for quota limits
    - Codex (OpenAI)
        - Full access sandbox mode with unrestricted filesystem and network access
        - Apply patch tool for efficient batch file editing
        - Shell command execution for terminal operations
        - Manage todo list for task tracking and planning
        - Streaming responses with thinking blocks
        - Rate limit monitoring and automatic account switching
        - Custom OpenAI/Anthropic Compatible models

- Advanced Features
    - Web Search integration (ZhipuAI, MiniMax)
    - FIM (Fill In the Middle) completion
    - NES (Next Edit Suggestions) completion
    - Account management with multi-account support
    - Token usage tracking
    - Quota monitoring

## Installation

### From VSCode Marketplace

1. Open VSCode
2. Go to Extensions view (`Ctrl+Shift+X` / `Cmd+Shift+X`)
3. Search for "Copilot Helper Pro"
4. Click Install

### From .vsix File

1. Download the latest `.vsix` file from the [Releases](https://github.com/nhatbien/copilot-helper/releases) page
2. Open VSCode
3. Run command: `Extensions: Install from VSIX...`
4. Select the downloaded `.vsix` file

### Build from Source

```bash
# Clone the repository
git clone https://github.com/nhatbien/copilot-helper.git
cd copilot-helper

# Install dependencies
npm install

# Compile the extension
npm run compile

# Package the extension
npm run package
```

## Requirements

- Visual Studio Code >= 1.104.0
- GitHub Copilot Chat extension
- Node.js >= 20.0.0
- npm >= 9.0.0

## Configuration

### ZhipuAI

```bash
Cmd+Shift+P > "ZhipuAI Configuration Wizard"
```

### MiniMax

```bash
Cmd+Shift+P > "Start MiniMax Configuration Wizard"
```

### MoonshotAI

```bash
Cmd+Shift+P > "Start MoonshotAI Configuration Wizard"
```

### DeepSeek

```bash
Cmd+Shift+P > "Set DeepSeek API Key"
```

### Custom Models

```bash
Cmd+Shift+P > "Compatible Provider Settings"
```

## Keybindings

- `Alt+/` - Trigger inline completion
- `Shift+Alt+/` - Toggle NES manual trigger mode
- `Ctrl+Shift+A` / `Cmd+Shift+A` - Attach selection to Copilot Chat
- `Ctrl+Shift+H` / `Cmd+Shift+H` - Insert handle reference
- `Ctrl+Shift+Q` / `Cmd+Shift+Q` - Quick switch account

## License

MIT

## Credits

Special thanks to:

- [LLMux](https://github.com/Pimzino/LLMux)
- [GCMP](https://github.com/VicBilibily/GCMP)
- [AntigravityQuotaWatcher](https://github.com/wusimpl/AntigravityQuotaWatcher)
