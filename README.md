# Copilot Helper Pro

<p align="center">
  <img src="logo_ai.png" alt="Copilot Helper Pro" width="128" height="128">
</p>

<p align="center">
  <strong>Supercharge your GitHub Copilot with multiple AI providers</strong>
</p>

<p align="center">
  <a href="https://marketplace.visualstudio.com/items?itemName=vicanent.copilot-helper-pro">
    <img src="https://img.shields.io/visual-studio-marketplace/v/vicanent.copilot-helper-pro?style=for-the-badge&logo=visual-studio-code&logoColor=white&label=Version&color=007ACC" alt="Version">
  </a>
  <a href="https://marketplace.visualstudio.com/items?itemName=vicanent.copilot-helper-pro">
    <img src="https://img.shields.io/visual-studio-marketplace/d/vicanent.copilot-helper-pro?style=for-the-badge&logo=visual-studio-code&logoColor=white&label=Downloads&color=28A745" alt="Downloads">
  </a>
  <a href="https://marketplace.visualstudio.com/items?itemName=vicanent.copilot-helper-pro">
    <img src="https://img.shields.io/visual-studio-marketplace/r/vicanent.copilot-helper-pro?style=for-the-badge&logo=visual-studio-code&logoColor=white&label=Rating&color=FFC107" alt="Rating">
  </a>
</p>

<p align="center">
  <a href="LICENSE">
    <img src="https://img.shields.io/badge/License-MIT-blue.svg?style=for-the-badge" alt="License">
  </a>
  <a href="https://code.visualstudio.com/">
    <img src="https://img.shields.io/badge/VS%20Code-1.104.0+-007ACC.svg?style=for-the-badge&logo=visual-studio-code&logoColor=white" alt="VS Code">
  </a>
  <a href="https://nodejs.org/">
    <img src="https://img.shields.io/badge/Node.js-20.0+-339933.svg?style=for-the-badge&logo=node.js&logoColor=white" alt="Node.js">
  </a>
</p>

---

## Overview

An extension that provides model support for GitHub Copilot Chat, including **ZhipuAI**, **MiniMax**, **MoonshotAI**, **DeepSeek**, **Antigravity (Google Cloud Code)**, **Codex (OpenAI)**, and custom **OpenAI/Anthropic** compatible models.

---

## Supported Providers

| Provider        | Description          | Features                                     |
| --------------- | -------------------- | -------------------------------------------- |
| **ZhipuAI**     | GLM Coding Plan      | Web Search, MCP SDK                          |
| **MiniMax**     | Coding Plan          | Web Search, Domestic/International endpoints |
| **MoonshotAI**  | Kimi For Coding      | High-quality responses                       |
| **DeepSeek**    | DeepSeek AI          | Fast inference                               |
| **Antigravity** | Google Cloud Code    | Gemini models, Quota tracking                |
| **Codex**       | OpenAI               | GPT-5, Apply Patch, Shell execution          |
| **Compatible**  | OpenAI/Anthropic API | Custom models support                        |

---

## Key Features

### Multi-Account Management

<table>
<tr>
<td width="60">
<img src="https://img.icons8.com/fluency/48/user-group-man-man.png" width="48"/>
</td>
<td>

**Manage multiple accounts per provider**

- Add unlimited accounts for each AI provider
- Quick switch between accounts with `Ctrl+Shift+Q` / `Cmd+Shift+Q`
- Visual account status in the status bar
- Secure credential storage using VS Code Secret Storage

</td>
</tr>
</table>

### Load Balancing & Auto-Switching

<table>
<tr>
<td width="60">
<img src="https://img.icons8.com/fluency/48/load-balancer.png" width="48"/>
</td>
<td>

**Automatic load distribution across accounts**

- When one account hits rate limits or quota exhaustion, automatically switch to another available account
- Intelligent retry with exponential backoff strategy
- Real-time quota monitoring and usage statistics
- Seamless failover without interrupting your workflow

</td>
</tr>
</table>

### Antigravity (Google Cloud Code)

<table>
<tr>
<td width="60">
<img src="https://img.icons8.com/fluency/48/google-cloud.png" width="48"/>
</td>
<td>

**Access Gemini models via Google Cloud Code**

- Streaming responses with real-time output
- Rate limit monitoring with automatic fallback to backup endpoints
- Quota tracking with detailed usage statistics
- Multi-account support with intelligent auto-switching
- Signature-based request validation for security
- Backoff and retry strategies for quota limits

</td>
</tr>
</table>

### Codex (OpenAI)

<table>
<tr>
<td width="60">
<img src="https://img.icons8.com/fluency/48/chatgpt.png" width="48"/>
</td>
<td>

**Full access to OpenAI Codex capabilities**

- **Full Access Sandbox Mode**: Unrestricted filesystem and network access
- **Apply Patch Tool**: Efficient batch file editing with unified diff format
- **Shell Command Execution**: Run terminal commands directly
- **Todo List Management**: Track tasks and plan your work session
- **Thinking Blocks**: View model reasoning in real-time
- **Rate Limit Monitoring**: Auto-switch accounts when limits are reached

</td>
</tr>
</table>

### Advanced Completion

<table>
<tr>
<td width="60">
<img src="https://img.icons8.com/fluency/48/code.png" width="48"/>
</td>
<td>

**Smart code completion features**

- **FIM (Fill In the Middle)**: Intelligent code completion based on context
- **NES (Next Edit Suggestions)**: Predictive editing suggestions
- **Web Search Integration**: Real-time information via ZhipuAI and MiniMax
- **Token Usage Tracking**: Monitor your API usage in real-time

</td>
</tr>
</table>

---

## Installation

### From VS Code Marketplace

```
1. Open VS Code
2. Go to Extensions (Ctrl+Shift+X / Cmd+Shift+X)
3. Search for "Copilot Helper Pro"
4. Click Install
```

### From .vsix File

```bash
# Download from releases page
# Then in VS Code:
# Cmd+Shift+P > "Extensions: Install from VSIX..."
```

### Build from Source

```bash
git clone https://github.com/nhatbien/copilot-helper.git
cd copilot-helper
npm install
npm run compile
npm run package
```

---

## Quick Start

### 1. Configure Provider

| Provider    | Command                                                 |
| ----------- | ------------------------------------------------------- |
| ZhipuAI     | `Cmd+Shift+P` > `ZhipuAI Configuration Wizard`          |
| MiniMax     | `Cmd+Shift+P` > `Start MiniMax Configuration Wizard`    |
| MoonshotAI  | `Cmd+Shift+P` > `Start MoonshotAI Configuration Wizard` |
| DeepSeek    | `Cmd+Shift+P` > `Set DeepSeek API Key`                  |
| Antigravity | `Cmd+Shift+P` > `Antigravity Login`                     |
| Codex       | `Cmd+Shift+P` > `Codex Login`                           |
| Custom      | `Cmd+Shift+P` > `Compatible Provider Settings`          |

### 2. Add Multiple Accounts (Optional)

```
Cmd+Shift+P > "Copilot Helper Pro: Manage Accounts"
```

### 3. Enable Load Balancing

```
Cmd+Shift+P > "Copilot Helper Pro: Open Account Manager"
Toggle "Load Balance" for your provider
```

---

## Keybindings

| Shortcut                       | Action                           |
| ------------------------------ | -------------------------------- |
| `Alt+/`                        | Trigger inline completion        |
| `Shift+Alt+/`                  | Toggle NES manual mode           |
| `Ctrl+Shift+A` / `Cmd+Shift+A` | Attach selection to Copilot Chat |
| `Ctrl+Shift+H` / `Cmd+Shift+H` | Insert handle reference          |
| `Ctrl+Shift+Q` / `Cmd+Shift+Q` | Quick switch account             |

---

## Requirements

| Requirement         | Version    |
| ------------------- | ---------- |
| VS Code             | >= 1.104.0 |
| Node.js             | >= 20.0.0  |
| npm                 | >= 9.0.0   |
| GitHub Copilot Chat | Required   |

---

## License

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.

---

## Credits

Special thanks to these amazing projects:

<table>
<tr>
<td align="center">
<a href="https://github.com/Pimzino/LLMux">
<img src="https://github.com/Pimzino.png" width="60" style="border-radius: 50%"/><br/>
<strong>LLMux</strong>
</a>
</td>
<td align="center">
<a href="https://github.com/VicBilibily/GCMP">
<img src="https://github.com/VicBilibily.png" width="60" style="border-radius: 50%"/><br/>
<strong>GCMP</strong>
</a>
</td>
<td align="center">
<a href="https://github.com/wusimpl/AntigravityQuotaWatcher">
<img src="https://github.com/wusimpl.png" width="60" style="border-radius: 50%"/><br/>
<strong>AntigravityQuotaWatcher</strong>
</a>
</td>
</tr>
</table>

---

<p align="center">
  Made with love for the developer community
</p>
