<p align="right">
  <a href="./readme.md">English</a> | <strong>中文</strong>
</p>

<div align="center">

<img src="assets/logo.png" alt="ChatableX 小蜜蜂智能体" width="200" />

<h1>ChatableX · 小蜜蜂智能体</h1>

<h3><em>让一切可对话</em></h3>

<font color="#0969da" size="3">Agent Loop Native · Harness Native — 每一次工具调用可追踪、可恢复、可纠偏，让每个人都能以工程师级精度解决问题。</font>

[![macOS](https://img.shields.io/badge/macOS-支持-000000?logo=apple&logoColor=white)]()
[![Windows](https://img.shields.io/badge/Windows-支持-0078D4?logo=windows&logoColor=white)]()
[![Linux](https://img.shields.io/badge/Linux-支持-FCC624?logo=linux&logoColor=black)]()

<p>
  <a href="https://www.chatablex.com"><strong>官网</strong></a>
  &nbsp;·&nbsp;
  <a href="https://www.chatablex.com/download"><strong>下载</strong></a>
</p>

</div>

<p align="center">
  <img src="assets/chatablex-app.png" alt="ChatableX 主界面：工具商店、对话交互、Agent Brain 推理追踪" width="920" />
</p>

## 下载

桌面端安装包（macOS / Windows / Linux）请前往官网获取：

**[https://www.chatablex.com/download](https://www.chatablex.com/download)**

## 产品定位

**ChatableX 是 Agent Loop Native 的桌面 Agent 平台** — 以 Harness 工程化体系贯穿 Agent Loop 执行循环，保障每一次工具调用的可追踪、可恢复与可纠偏。<br>
它让普通用户以工程师级精度驾驭 Tool、Skill 与 AI App：用户将日常重复流程沉淀为**稳定可调用的工具**，Agent 以对话编排调度 — 而非让 AI 每次从头执行；过程全程可视化，异常自动感知与纠偏，失败可重试、可从任意步骤恢复。

## 设计哲学

> **对话驱动一切的前提，不是让 AI 包办一切，而是让 AI 精准调度稳定工具。**

### 对话驱动，而非代码驱动

ChatableX 之名取自 **Chat + able + X** — **可对话**。我们的信念是：**让一切应用可对话，对话驱动一切**。

Codex、Cursor 等产品以代码为中心 — 即便 Vibe Coding 风行，底层思维仍是「用 Code 解决问题」。ChatableX 则走向另一端：**你只需用自然语言表达意图，无需关心底层代码如何运作**。

但要真正实现对话驱动，仅靠「文字输入 + 通用 Agent」远远不够。许多智能体虽以自然语言交互，若把完整任务交给 AI 从头生成，幻觉、不稳定、不可复现几乎不可避免。**ChatableX 的解法：把确定性交给工具，把不确定性交给 Agent 编排。**

### 稳定工具，而非从头生成

真实工作从来不是一条预先设计好的流水线 — 它是**离散的、分散的、大量重复的**。

一个庞大任务，本质上是许多小步骤的组合。ChatableX 倡导**分层拆解**：把每个步骤固化为可执行、可验证、可复用的**稳定小工具**，再装配完成复杂任务。

以「给图片加水印」为例 — 这是一个琐碎但高频的操作。若每次让 AI 从头写代码实现，即便用最贵的模型，仍可能出现参数错误或执行偏差。正确做法是：**用最好的模型把这个任务做成一个经过验证的可调用工具** — 一次制作，反复使用。若干小工具组装起来，就能稳定完成更复杂的任务。

这正是 ChatableX 提供**工具商店**的原因 —

- **稳定执行的工具才有长期价值**，不应随任务结束而被丢弃
- 实际工作中大量流程是**重复出现**的 — ChatableX 帮你把这些重复流程沉淀为小工具
- 工具创作阶段可以用**最强模型**把质量做到位（好钢用在刀刃上）
- 日常调度阶段 Agent 可用**本地量化小模型**，以最低 Token 成本精准调用这些工具

**思维即产品，语言即接口 — 但接口背后，必须是经过验证的稳定工具。**

### 确定性流程必须工具化

业界常宣称「AI 可以做任何事」，但在专业领域，AI 不可能从零构建一切。

制作游戏，不会从头写一个游戏引擎 — 一定基于 Unity、Unreal 等**稳定的引擎工具**在其上创作；游戏引擎本身，就是大量小工具的集合。电商系统、ERP 等业务应用同理：订单、库存、结算等流程是**固定的、经过业务抽象验证的**，传统上由 ER 图驱动的业务系统承载 — 不可能让 AI 每次从头重写。

正确路径是：**把确定性业务流程做成固定可调用的工具，暴露 API 给 Agent** — 让 AI 负责理解与调度，而非重新发明业务逻辑。

**使用 ChatableX 的核心意义正在于此：**

1. 把你日常工作中重复的、确定性的流程，做成**稳定可调用的工具**
2. 把这些工具交给 ChatableX，由 Agent 以**自然语言编排调度**
3. 平台通过 **Agent Loop** 保障执行循环的连贯与可控，通过 **Harness** 保障每一次工具调用的可追踪、可恢复与可纠偏 — 确保你的语言能**准确路由到正确的工具**

### 分层分工：工具交付、Agent 调度、模型推理

ChatableX 据此确立三层职责模型 — 对话驱动一切，需要每一层各尽其责：

<table>
<thead>
<tr>
<th align="left" nowrap>层次</th>
<th align="left" nowrap>职责主体</th>
<th align="left">质量要求</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left" nowrap>工具交付</td>
<td align="left" nowrap>人类 + 稳定工具</td>
<td align="left">API、脚本及辅助工具的执行结果须经验证与测试</td>
</tr>
<tr>
<td align="left" nowrap>Agent 调度</td>
<td align="left" nowrap>AI Agent</td>
<td align="left">解析用户指令，精确路由至对应工具或 MCP 服务</td>
</tr>
<tr>
<td align="left" nowrap>模型推理</td>
<td align="left" nowrap>AI 模型</td>
<td align="left">处理模糊意图、规划执行步骤、生成结果解释</td>
</tr>
</tbody>
</table>

确定性交付由**稳定工具**保障，意图理解与调度由 **Agent** 承担，模糊推理与规划由**模型**辅助 — 三者各司其职，「对话驱动一切」才有工程基础。

## 工具误选问题与应对机制

工具规模一旦膨胀，**Agent 调度层**的准确性就成为首要挑战 — 工具调用是否准确？执行链路是否可追溯？异常是否可定位？

同一业务域内，不同用户可能沉淀数百至数千个定制工具。<br>
若将全部工具预载至 Agent 上下文，或经 RAG 检索后批量注入模型，工具误选、参数幻觉及调用链失控将成为系统性风险。<br>
ChatableX 采用会话级工具隔离（Session-scoped Tool Isolation）机制 — 由用户在会话层面声明本次任务的工具集，而非由智能体预先加载全量能力：

<p align="center">
  <img src="assets/session-tool-isolation.png" alt="会话级工具隔离：工具商店检索筛选 → 本次对话工具栏装配 → 仅注入已选工具至 Agent 执行上下文" width="920" />
</p>

### 设计原则

1. **意图驱动（Intent-first）** — 任务意图在用户侧已明确；用户于工具商店检索、筛选并装配，而非依赖 Agent 在全量工具空间中进行概率性选择。
2. **会话隔离（Session Isolation）** — 系统内置少量通用基础工具；业务工具由用户按会话显式装配，跨会话互不干扰。
3. **质量门禁（Quality Gate）** — 同一业务域可能存在海量候选工具；进入会话前须通过验证状态、使用反馈及评分排名等机制筛选，降低幻觉风险。
4. **动态加载（Dynamic Loading）** — 工具与依赖按需挂载、按需卸载；各会话拥有独立运行时，会话结束后自动清理环境残留。

## 与主流方案对比

<table>
<thead>
<tr>
<th align="left" nowrap>维度</th>
<th align="left">Codex / Claude Code / Cursor</th>
<th align="left">Coze / Dify 等工作流平台</th>
<th align="left">ChatableX</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left" nowrap>目标用户</td>
<td align="left">开发者</td>
<td align="left">运营 / 轻量自动化</td>
<td align="left">业务用户 + 领域专家</td>
</tr>
<tr>
<td align="left" nowrap>工具选择</td>
<td align="left">隐式（项目文件、MCP 自动挂载）</td>
<td align="left">可视化节点，预定义能力</td>
<td align="left">显式装配，用户声明会话级工具集</td>
</tr>
<tr>
<td align="left" nowrap>工具规模</td>
<td align="left">项目级，开发者可控</td>
<td align="left">平台预置节点</td>
<td align="left">个人工具库可扩展，会话级裁剪</td>
</tr>
<tr>
<td align="left" nowrap>调用可追踪</td>
<td align="left">部分支持 Trace，面向开发者</td>
<td align="left">流程日志</td>
<td align="left">Harness Inspector：树状追踪 + 关键操作确认，面向全用户</td>
</tr>
<tr>
<td align="left" nowrap>工具创作</td>
<td align="left">代码编写 / MCP 配置</td>
<td align="left">可视化编排</td>
<td align="left">对话式零代码构建 + 操作录制蒸馏</td>
</tr>
<tr>
<td align="left" nowrap>运行环境</td>
<td align="left">云端容器 / IDE 内嵌</td>
<td align="left">云端</td>
<td align="left">本地桌面工作站，数据驻留本机</td>
</tr>
<tr>
<td align="left" nowrap>交互范式</td>
<td align="left">Code / Vibe Coding，以代码生成为核心</td>
<td align="left">可视化流程编排</td>
<td align="left">对话驱动，自然语言即接口</td>
</tr>
<tr>
<td align="left" nowrap>工具沉淀</td>
<td align="left">散落在项目目录，普通用户难以找回复用</td>
<td align="left">平台内工作流，跨用户分享有限</td>
<td align="left">创作即入库，商店检索、拖拽复用、一键分享</td>
</tr>
<tr>
<td align="left" nowrap>创作 Skills</td>
<td align="left">需手动安装 superpowers 等扩展，有认知门槛</td>
<td align="left">平台预置节点能力</td>
<td align="left">内置工具创作 Skills，自然语言即可产出专业级工具</td>
</tr>
<tr>
<td align="left" nowrap>环境依赖</td>
<td align="left">开发者自行配置 Node.js、package.json 等</td>
<td align="left">云端托管，用户无感</td>
<td align="left">安装环节自动检测与配置运行时依赖</td>
</tr>
<tr>
<td align="left" nowrap>沙箱隔离</td>
<td align="left">云端容器为主，本地隔离因产品而异</td>
<td align="left">云端多租户隔离</td>
<td align="left">本地桌面级会话沙箱，执行与宿主系统隔离</td>
</tr>
<tr>
<td align="left" nowrap>模型策略</td>
<td align="left">同一模型兼顾创作与执行，Token 成本高</td>
<td align="left">平台托管，用户无感</td>
<td align="left">强模型造工具，轻模型做调度 — 好钢用在刀刃上</td>
</tr>
<tr>
<td align="left" nowrap>核心范式</td>
<td align="left">AI 辅助代码生成与项目修改</td>
<td align="left">AI 辅助流程编排</td>
<td align="left">AI 精准调度已验证工具</td>
</tr>
</tbody>
</table>

ChatableX 不以代码生成量为竞争维度，而聚焦于：**把重复流程沉淀为稳定工具，以最低成本精准调度，全程可追踪、可恢复、可纠偏**。

## 核心能力

### 1. 拖拽装配 · 个人工具商店

左侧扩展栏构成个人工具工作台：支持市场浏览、已安装扩展管理及自研工具归档。<br>
用户以自然语言或录制方式完成工具构建后，**自动纳入本地商店** — 下次同类任务直接检索、拖拽至对话区即可复用，也可**一键分享给他人**。

Codex、Cosmos 等方案面向开发者：工具散落在项目目录或临时会话中，普通用户既不知道「做的东西保存在哪」，也难以在下次任务中找回。ChatableX 将**创作、沉淀、复用、分享**闭环内置于平台 — **工具是可复用的资产，不是一次性消耗品**。

### 2. Harness Inspector · 全链路可观测性

主流 Agent 产品通常仅提供对话界面，工具调用过程不可见。<br>
ChatableX 在右侧集成 Harness Inspector，作为 Agent 行为的可观测层：

- **推理追踪（Reasoning Trace）** — 实时呈现 Agent 推理过程
- **工具流水线（Tool Pipeline）** — 以树状结构展示每次调用的输入、输出及状态
- **环境上下文（Environment Context）** — 展示当前会话已装配工具及文件状态
- **关键操作确认（Human-in-the-loop）** — 文件写入、付费接口调用、工具发布等高风险操作须经用户授权

左侧承载交互结论，右侧承载执行细节 — 形成互补的可读性结构。

### 3. 零代码工具构建 · 内置创作 Skills

- **描述即创造（Description-to-Tool）** — 用户以自然语言描述意图，Agent 生成并迭代可执行工具
- **录制即技能（Demonstration-to-Skill）** — 用户示范操作路径，系统将其蒸馏为可复用技能，以演示替代编码
- **内置创作 Skills** — Codex 等平台需用户自行安装 superpowers 等扩展才能高效造工具，普通用户往往不理解 Skills 是什么、如何配置。ChatableX **预置工具创作所需的 Skills**，用户只需对话，即可产出与高级程序员同等水准的应用
- **强模型创作，轻模型调度** — 工具制作阶段调用最强模型确保质量；日常 Agent 调度使用本地量化小模型，以最低 Token 成本精准调用已验证工具
- **版本管理（Version Control）** — 工具支持草稿、测试、稳定、归档等生命周期阶段，支持随时回退

### 4. 本地沙箱 · 会话级环境隔离

每个对话会话在**本地桌面沙箱**中运行 — Agent 的文件读写、命令执行、工具调用均与宿主系统隔离；跨会话的工具依赖互不干扰，会话结束后环境自动清理。<br>
沙箱是 Agent 平台的必备能力：它保障执行安全、消除跨任务污染与环境残留导致的级联故障。

### 5. 开箱即用 · 依赖自动配置

工具安装与创作环节，平台**主动检测并配置**用户可能需要的运行时环境 — Node.js、Python、package.json 依赖、系统级工具链等，无需用户手动排查「为什么跑不起来」。<br>
普通用户不必理解 package manager 或环境变量；平台在后台完成依赖装配，用户专注描述需求即可。

### 6. Agent Loop · 计划—执行分离

Agent Loop 内嵌 Plan-then-Execute 策略：优先生成执行计划，再逐步调用工具；支持失败重试、方案切换及执行中止。<br>
结合环境反馈，各步骤均可定位、中断与回溯 — 而非单次概率性交付。

## 典型工作流

### 示例：图像水印处理

这个例子体现了 ChatableX 的核心思路 — **小工具沉淀 + 对话编排调度**：

1. **首次使用**：以自然语言描述需求，Agent 调用强模型将「图片加水印」制作为**稳定工具**，自动纳入商店
2. **后续复用**：于左侧扩展栏检索该工具，拖拽至输入区完成装配 — 无需重复制作
3. 上传目标图像，以自然语言指定参数（文本内容、字号、位置）；Agent 以轻模型解析意图，**精准调用**已验证工具
4. Harness Inspector 实时展示 Agent 的意图解析、参数映射及工具调用过程
5. 处理完成后，输出文件保存至当前会话；工具永久保留于商店，供本人或他人复用

```
重复流程沉淀为工具 → 商店检索装配 → 对话描述意图 → Agent 精准调度 → 追踪执行 → 结果交付
```

## 适用对象

- **业务专家 / 运营人员** — 不具备编程能力，但需构建可复用的自动化工具
- **中小企业** — 希望将 AI 接入既有 API 与工具链，而非重构整体系统
- **可观测性敏感用户** — 要求完整可见的推理链路与工具调用过程
- **工具创作者** — 需要覆盖构建、测试、沉淀、分享与复用的完整生命周期
- **零代码探索者** — 有想法但不会编程，希望用对话而非 Code 交付应用

<p align="center">
  <strong>ChatableX · 小蜜蜂智能体</strong><br />
  <sub>Agent Loop Native · Harness Native · macOS · Windows · Linux</sub><br />
  <sub><a href="https://www.chatablex.com">www.chatablex.com</a></sub>
</p>
