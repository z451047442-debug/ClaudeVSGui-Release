# ClaudeVSGui：在 Visual Studio 中使用 Claude Code

直接在 Visual Studio 内使用顶级 AI 编程命令行工具。

ClaudeVSGui 将 **Claude Code CLI、Copilot CLI、Codex CLI 和 Gemini CLI** 集成到 Visual Studio 2022 与 2026 中，让您无需离开 IDE 即可与偏好的代理协作。

## 核心功能

- **快速切换模型**  
  默认通过 Alt+1、Alt+2、Alt+3、Alt+4 热键切换 Claude 模型，支持重新绑定。
- **免提输入**  
  按 `Alt+S` 使用 Windows 语音识别发出语音命令。
- **通过选项卡并行运行多个代理**  
  同时运行多个代理，各自拥有独立选项卡。
- **更快的开发循环**  
  将编辑器上下文、任务行/注释以及调试器异常直接发送给代理。
- **Visual Studio 内的原生 CLI 体验**  
  代理在集成控制台窗口中运行，保留其原始行为与控件。除所支持的 CLI 外，还支持自定义程序。
- **主题感知 UI**  
  支持浅色、深色和系统主题。
- **隐私优先架构**  
  该扩展不保存任何凭据、对话历史记录或其他用户数据。

## 用法

**语音输入**：按 `Alt+S`，说出命令，然后按 Enter 发送。当 Windows 语音识别检测到您已说完时，录音会自动停止。

| 菜单项 | 描述 |
| --- | --- |
| **视图 → ClaudeVSGui** | 启动 Claude Code CLI（需要打开项目/解决方案） |
| **视图 → 发送位置到代理** | 发送活动文件路径、行号及选中文本 |
| **视图 → 发送任务到代理** | 将当前行作为命令执行 |
| **视图 → 发送异常到代理** | 从调试器发送调试器异常/错误详细信息 |

## 键盘快捷键

所有操作均可配置快捷键：

- `ClaudeVSGui.SpeechCommand`
- `View.ClaudeVSGui`
- `View.SendLocationtoAgent`
- `View.SendTasktoAgent`
- `View.SendDebuggerExceptiontoAgent`

ClaudeVSGui 还能捕获并转发 Claude Code CLI 常用组合键（例如 `Ctrl+B`、`Ctrl+O`、`Ctrl+R`）。在以下位置配置：

**工具 → 选项 → 环境 → 键盘**

- `ClaudeVSGui.AgentAction1`
- `ClaudeVSGui.AgentAction2`
- `ClaudeVSGui.AgentAction3`
- `ClaudeVSGui.AgentAction4`
