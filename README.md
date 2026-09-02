# IC Coder

> 让 FPGA 开发者因 AI 而更强大

**IC Coder 是面向 FPGA 设计与验证的 AI Agent 研发平台。**

*IC Coder is an AI Agent R&D platform for FPGA design and verification.*

[官方网站](https://www.iccoder.com/) · [VS Code Marketplace](https://marketplace.visualstudio.com/items?itemName=ICCoderAgenticVerilogPlatform.iccoder) · [安装与使用教程](https://rcn4uafl8j9j.feishu.cn/docx/Sa9md6TGIoYyMgxAwTgcuhoWnDe?from=from_copylink)

> **仓库说明**
>
> 本仓库当前是 IC Coder 的产品信息与公共资源入口，用于发布产品介绍、公开文档、使用指引和经审核的公共资料。
>
> 本仓库不包含 IC Coder 商业产品源码、模型权重、企业交付包、客户工程配置或内部研发资料，也不构成任何开源许可或产品授权。

## 什么是 IC Coder

IC Coder 面向真实 FPGA 工程任务，将专业模型能力与工程执行能力结合起来，协助开发者贯通需求理解、架构设计、RTL、TestBench、仿真、智能 Debug、EDA 工具交互与工程交付。

IC Coder 不只是生成一段 Verilog 代码，而是围绕工程上下文、执行证据和验证结果开展持续协作，让研发过程更可运行、可验证、可追溯、可交付。

## 两大核心

| 核心 | 定义 | 主要作用 |
| --- | --- | --- |
| **IC Coder 模型** | FPGA 领域专用微调模型 | 理解 FPGA 工程语义，辅助分析需求、生成内容并解读工程结果 |
| **IC Coder Harness** | FPGA 原生 Harness | 管理项目上下文与任务，读写获准的工程文件，调用已配置的工具，并组织验证与迭代闭环 |

**IC Coder = IC Coder 模型 + IC Coder Harness**

## FPGA 研发闭环

在相应功能已开通、工程环境满足要求且用户完成授权的前提下，IC Coder 可协助开展：

- **需求理解**：阅读需求、协议、器件资料和已有工程，提炼目标、约束与验收条件。
- **架构设计**：梳理模块边界、接口、时钟与复位、数据流、状态机和验证策略。
- **RTL 开发**：辅助编写、解释、检查和维护 Verilog / SystemVerilog RTL。
- **验证与 Debug**：构建 TestBench，运行仿真，分析日志、报告与波形，定位问题并推动复验。
- **EDA 工具交互**：在工具、许可证和工程配置可用时，调用获准的 EDA 流程并读取真实执行结果。
- **工程交付**：组织需求、设计、RTL、验证资产、脚本、报告和工程产物，帮助团队沉淀可复用的研发资产。

典型任务链：

`需求理解 → 架构设计 → RTL → TestBench → 仿真 → 智能 Debug → EDA → 工程交付`

## 在 VS Code 中使用

IC Coder 当前以 VS Code 插件形态提供。

1. 打开 [IC Coder 的 VS Code Marketplace 页面](https://marketplace.visualstudio.com/items?itemName=ICCoderAgenticVerilogPlatform.iccoder)，核对发布信息后安装。
2. 按照[安装与使用教程](https://rcn4uafl8j9j.feishu.cn/docx/Sa9md6TGIoYyMgxAwTgcuhoWnDe?from=from_copylink)完成账号及工程环境配置。
3. 打开目标工程，说明任务、输入资料、执行范围和验收要求，开始协作。

你可以从这类任务开始：

> 阅读当前需求和工程目录，先列出模块接口、关键约束、风险与验收计划；未经确认，不要修改文件。

> 基于现有 RTL 和接口协议设计 TestBench，说明覆盖场景、检查方法和预期结果。

> 在我授权的范围内运行已配置的仿真工具，读取返回码、日志和波形，定位失败原因并给出复验方案。

## 工具、许可证与工程边界

IC Coder 能够执行的具体任务取决于产品版本、账号权限、工程环境及相应功能是否开通。

调用仿真、综合、布局布线、时序分析、Bitstream 或配置文件生成等 EDA 流程前，需要同时满足：

- 对应工具及器件支持包已经正确安装和配置；
- 工具许可证合法、有效且当前可用；
- 用户明确授权 IC Coder 执行本次操作；
- 工程脚本、约束、目标器件和运行环境满足任务要求；
- 实际工具、版本和工程配置处于当前产品支持范围内。

IC Coder 会尽可能依据真实的返回码、日志、报告、波形和工程产物推进分析与复验，但生成 Bitstream 或配置文件不等于已经完成烧写、真板验证或最终工程验收。关键设计结论和交付结果仍应由具备相应职责的工程人员审核确认。

第三方软件、EDA 工具、IP、器件库及相关许可证由各自权利人提供，使用者应自行取得合法授权并遵守相应条款。

## 产品与公共资源

- [IC Coder 官方网站](https://www.iccoder.com/)：了解产品能力、企业方案与合作方式。
- [VS Code Marketplace](https://marketplace.visualstudio.com/items?itemName=ICCoderAgenticVerilogPlatform.iccoder)：安装当前公开插件。
- [IC Coder 安装与使用教程](https://rcn4uafl8j9j.feishu.cn/docx/Sa9md6TGIoYyMgxAwTgcuhoWnDe?from=from_copylink)：查看插件安装、配置和使用说明。

具体功能、版本、服务范围和交付方式，以官方网站、正式产品界面、双方协议及实际交付内容为准。

## 仓库与授权说明

本仓库的公开可见性不表示 IC Coder 产品、源码、模型、Harness、文档或其他专有资料已获得开源授权。

除非具体文件中附有明确的许可证或授权声明，否则：

- 不应将本仓库视为 IC Coder 产品源码的分发渠道；
- 不应据此推定获得复制、修改、再分发或商业使用 IC Coder 产品的权利；
- 产品使用、企业部署、技术服务和商业合作以单独签署的协议及正式授权为准；
- 后续新增的公共示例或资源，以其所在目录中的具体许可说明为准。

## 反馈与安全问题

如需提交功能建议或文档纠错，请通过[官方网站](https://www.iccoder.com/)提供的联系入口反馈。提交前请移除账号、Token、密钥、客户名称、私有源码、内部网络地址、工程日志及其他敏感信息。

如果发现可能影响 IC Coder、用户数据或工程安全的问题，请勿公开披露漏洞细节、复现脚本或敏感证据。请通过官网联系入口进行私下反馈，以便团队安全确认和处理。

## 发起人与团队

- **发起人**：蔡杰涛（Ryan）
- **公开头衔**：IC Coder 创始人、鹏野嘉途 CEO
- **公司**：成都鹏野嘉途科技有限公司
- **长期方向**：AI for EDA、Agentic FPGA 与 FPGA 研发智能化

我们将持续推进专业模型、FPGA 原生 Harness、真实 EDA 工程闭环与产业生态建设。

**让 FPGA 开发者因 AI 而更强大。**

