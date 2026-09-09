<p align="center">
  <img src="docs/assets/logo.png" alt="Open AIoT" width="120">
</p>

# Open AIoT 开放规范（spec）

**设备 × AI 的开放标准** —— Open AIoT 项目的核心仓库，包含全部规范文档、RFC 提案与治理文件。

本仓库回答三个问题：设备如何向 AI 描述自己的能力（L0 设备能力模型）、这些能力以什么协议形态出现在 AI 面前（L1 协议绑定，首个绑定为 MCP）、AI 操控物理设备时如何授权与审计（L2 授权与安全模型）。

> 项目状态：规范起草中（Phase 0，v0.x Draft 阶段）。v0.x 允许快速迭代，兼容性承诺自 1.0 起生效（见 VERSIONING.md）。

## 仓库结构

```
specs/                  规范文档（按主题分目录，含 specVersion 与状态标识）
  capability-model/     L0 设备能力模型（v0.1 草案，经实现对照评审修订）
  mcp-binding/          L1 MCP 绑定规范（v0.1 草案）
  tool-description/     L1 工具描述写作规范 LLM-first（v0.1 草案）
  auth-security/        L2 授权与安全模型（v0.1 草案）
VERSIONING.md           版本与兼容性政策（最高纪律）
rfcs/                   RFC 提案与决议记录
docs/assets/            品牌资源
```

## 读者导航

- **设备厂商/实现者**：从 `specs/capability-model/` 开始——你的设备如何描述自己的能力；
- **平台接入者**（AI 平台、连接器作者）：L0 之后读 `specs/mcp-binding/` 与 `specs/tool-description/`；
- **Skill 作者**：先读 L0 与 L1，Skill 格式规范见 [skills 仓库](https://github.com/Open-AIoT/skills)（规划中）；
- **提案人**：读 VERSIONING.md 与 rfcs/，按 RFC 流程提交。

## 参与与提案

规范变更走 RFC 流程（见 rfcs/ 与治理文件）。破坏性变更只有一条通道：RFC + 公示期。

## 声明

**Open AIoT（开放AIoT）**——"Open"即"开放"。本项目是芯步（ThingBoot）主导的开放 AIoT 标准与生态品牌，与 OpenAI 公司无任何关联。

## License

规范文档以 [CC-BY-4.0](LICENSE) 发布。

---

*Open AIoT is an open device×AI standard led by ThingBoot. This repository holds the specifications, RFCs and governance documents. Not affiliated with OpenAI.*
