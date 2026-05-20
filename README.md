
# ClaudeVSGui: Claude Code in Visual Studio

**Use top AI coding CLIs directly inside Visual Studio.**

ClaudeVSGui integrates **Claude Code CLI, Copilot CLI, Codex CLI, and Gemini CLI** into Visual Studio 2022 and 2026, so you can work with your preferred agent without leaving the IDE.

## Core Features

- **Quick model switching**  
  Switch between Claude models via hotkeys: Alt+1, Alt+2, Alt+3, Alt+4 by default, rebindable.
- **Hands-free input**  
  Press `Alt+S` to use Windows speech recognition for voice commands.
- **Run multiple agents in parallel with tabs**  
  Run multiple agents at the same time, each in its own tab
- **Faster development loop**  
  Send editor context, task lines/comments, and debugger exceptions straight to an agent.
- **Native CLI experience inside Visual Studio**  
  Agents run in integrated console windows, preserving their original behavior and controls. Support for custom programs in addition to supported CLIs.
- **Theme-aware UI**  
  Supports Light, Dark, and System themes.
- **Privacy-first architecture**  
  The extension does **not** save any credentials, conversation history, or other user data.

## Usage

**Voice input**: press `Alt+S`, speak your command, then press Enter to send. Recording stops automatically when Windows speech recognition detects you are done speaking.

| Menu Item | Description |
| --- | --- |
| **View → ClaudeVSGui** | Launch Claude Code CLI (requires an open project/solution) |
| **View → Send Location to Agent** | Send active file path, line number, and selected text |
| **View → Send Task to Agent** | Execute current line as a command |
| **View → Send Exception to Agent** | Send debugger exception/error details from debugger |

## Keyboard Shortcuts

All actions are hotkey-configurable:

- `ClaudeVSGui.SpeechCommand`
- `View.ClaudeVSGui`
- `View.SendLocationtoAgent`
- `View.SendTasktoAgent`
- `View.SendDebuggerExceptiontoAgent`

ClaudeVSGui can also capture and forward key combinations commonly used by Claude Code CLI (for example `Ctrl+B`, `Ctrl+O`, `Ctrl+R`). Configure these in:

**Tools → Options → Environment → Keyboard**

- `ClaudeVSGui.AgentAction1`
- `ClaudeVSGui.AgentAction2`
- `ClaudeVSGui.AgentAction3`
- `ClaudeVSGui.AgentAction4`
