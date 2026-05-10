<div align="center">
  <img src="https://www.siliconflow.cn/" alt="siliconflow Logo" width="60%" />
</div>

<br/>

<div align="center">

# siliconflow DeepSeek for GitHub Copilot Chat

在 VS Code 的 GitHub Copilot Chat 中直接使用 siliconflow 的DeepSeek 模型

[![GitHub Release](https://img.shields.io/github/v/release/ChenyuHeee/deepseek-copilot)](https://github.com/ChenyuHeee/deepseek-copilot/releases)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

[中文](#中文) | [English](#english)

</div>

---

<a name="中文"></a>

## 说明

### 前言

- 此仓库改自GitHub的[ChenyuHeee/deepseek-copilot: DeepSeek V4 provider for GitHub Copilot Chat](https://github.com/ChenyuHeee/deepseek-copilot)
- 使用上您需要在您需要填入key的时候填入`siliconflow的key`就可以了

### 目的：

- 为了将 provider 从`deepseek`改为`siliconflow`，因为我siliconflow上还有100的余额,deepseek只有10块了( :

### 修改简要

- 修改默认的厂商为`siliconflow `并且将原来的deepseek模型`v4-flash`和`v4-pro`改为了 `v4-flash`和`v3.2`
- 下面的markdown说明也是原作者[ChenyuHeee (He Chenyu)](https://github.com/ChenyuHeee)写的我只做了尽可能少的改动

### 题外话

- 我默认用的是`非pro模型`(siliconflow不能使用免费额度),这意味这你就算只有免费额度也可以使用，但是可能无法支持高强度使用(免费额度会限速）,但这经济实惠的选择，如果你只是利用这个学习做点小项目我很推荐使用siliconflow
- 再次感谢原作者开源，如果您喜欢此项目那么请你为[ChenyuHeee (He Chenyu)](https://github.com/ChenyuHeee)的[ChenyuHeee/deepseek-copilot](https://github.com/ChenyuHeee/deepseek-copilot)点一个star（：

## 中文

在 VS Code 的 GitHub Copilot Chat 中直接使用 **DeepSeek V4 Flash** 和 **DeepSeek V3.2**，通过官方 [siliconflow](https://www.siliconflow.cn/) 驱动。


| 模型                | 上下文长度 | 思考模式 | 适合场景               |
| ------------------- | ---------- | -------- | ---------------------- |
| `deepseek-v4-flash` | 1M tokens  | ✗       | 日常快速任务，响应更快 |
| `deepseek-v3.2`     | 1M tokens  | ✓       | 复杂推理、大型代码库   |

### 使用前准备

请确认你已经具备：

- [VS Code](https://code.visualstudio.com/) 1.104.0 或更高版本
- 已安装并登录 [GitHub Copilot](https://marketplace.visualstudio.com/items?itemName=GitHub.copilot) 扩展
- 一个 [DeepSeek API Key](https://platform.deepseek.com/api_keys)（注册账号免费获取）

### 第一步 — 下载插件

前往 [Releases 页面](https://github.com/ChenyuHeee/deepseek-copilot/releases)，下载最新版本的 `deepseek-copilot.vsix` 文件。

### 第二步 — 安装插件

**方式 A — 通过 VS Code 界面安装（推荐新手使用）**

1. 打开 VS Code
2. 点击左侧侧边栏的 **扩展** 图标（或按 `Ctrl+Shift+X` / `Cmd+Shift+X`）
3. 点击扩展面板右上角的 `···` 菜单
4. 选择 **从 VSIX 安装...**
5. 选择刚下载的 `deepseek-copilot.vsix` 文件
6. 点击 **安装**

**方式 B — 通过终端安装**

```bash
code --install-extension /path/to/deepseek-copilot.vsix
```

### 第三步 — 输入 DeepSeek API Key

1. 按 `Ctrl+Shift+P`（Windows/Linux）或 `Cmd+Shift+P`（macOS）打开命令面板
2. 输入 **Manage DeepSeek Provider** 并按回车
3. 粘贴你的[SiliconCloud-key](https://cloud.siliconflow.cn/me/account/ak)并按回车

### 第四步 — 选择模型，开始对话

1. 打开 Copilot Chat 面板（点击侧边栏的聊天图标，或按 `Ctrl+Alt+I` / `Cmd+Option+I`）
2. 点击对话框顶部的模型选择器
3. 选择 **DeepSeek V4 Flash** 或 **DeepSeek V4 Pro**
4. 开始聊天！

---

<a name="english"></a>

## English

Use **DeepSeek V4 Flash** and **DeepSeek V4 Pro** directly inside VS Code's GitHub Copilot Chat, powered by the official [siliconflow](https://www.siliconflow.cn/).


| Model               | Context   | Thinking Mode | Best For                           |
| ------------------- | --------- | ------------- | ---------------------------------- |
| `deepseek-v4-flash` | 1M tokens | ✗            | Fast everyday tasks                |
| `deepseek-v3.2`     | 1M tokens | ✓            | Complex reasoning, large codebases |

### Prerequisites

- [VS Code](https://code.visualstudio.com/) 1.104.0 or higher
- [GitHub Copilot](https://marketplace.visualstudio.com/items?itemName=GitHub.copilot) extension installed and signed in
- A [DeepSeek API Key](https://platform.deepseek.com/api_keys)

### Step 1 — Download the extension

Go to the [Releases page](https://github.com/ChenyuHeee/deepseek-copilot/releases) and download the latest `deepseek-copilot.vsix` file.

### Step 2 — Install the extension

**Option A — Via VS Code UI (recommended)**

1. Open VS Code
2. Click the **Extensions** icon in the left sidebar (`Ctrl+Shift+X` / `Cmd+Shift+X`)
3. Click the `···` menu at the top-right of the Extensions panel
4. Select **Install from VSIX...**
5. Choose the downloaded `deepseek-copilot.vsix` file

**Option B — Via terminal**

```bash
code --install-extension /path/to/deepseek-copilot.vsix
```

### Step 3 — Enter your DeepSeek API key

1. Open the Command Palette (`Ctrl+Shift+P` / `Cmd+Shift+P`)
2. Type **Manage DeepSeek Provider** and press Enter
3. Paste your [SiliconCloud-key](https://cloud.siliconflow.cn/me/account/ak) and press Enter

### Step 4 — Select a model and start chatting

1. Open Copilot Chat (`Ctrl+Alt+I` / `Cmd+Option+I`)
2. Click the model selector at the top
3. Choose **DeepSeek V4 Flash** or **DeepSeek V4 Pro**
4. Start chatting!

### Development

```bash
git clone https://github.com/ChenyuHeee/deepseek-copilot
cd deepseek-copilot
npm install
npm run compile
```

Press `F5` to launch an Extension Development Host.

---

## Support & License

- Issues: https://github.com/ChenyuHeee/deepseek-copilot/issues
- License: MIT
