<div align="center">

# Ocean Han

**后端工程师 · 把成熟系统拆开，按自己的判断重做一遍**

`Java` · `Spring Boot` · `MyBatis-Plus` · `Vue 3` · `MySQL` · `Redis` · `Playwright`

</div>

---

## 当前主线

### [openpm](https://github.com/OceanHAN/openpm) — 参考禅道思路重做的研发协作平台

产品 · 项目 · 执行 · 需求 · 任务 · 缺陷 · 测试 · 文档 · 工时 · 看板 · 度量 · BI · 报表

| 维度 | 规模 |
| --- | --- |
| 后端 | Java 25 · Spring Boot 4.1 · MyBatis-Plus · **537 个 Java 文件 / 约 5.7 万行** |
| 前端 | Vue 3 · TypeScript · Element Plus · Vite · **130 个文件 / 约 2.4 万行** |
| 数据 | MySQL 8 · Redis 7 · **67 张 `zt_*` 表** |
| 覆盖 | 禅道开源版 99 个模块，**已实现 48 个**，明确不迁移 47 个 |
| 验证 | **43 个接口回归脚本 / 1704 项断言** · 21 个页面巡检 · 20 个浏览器专项 |
| 许可 | AGPL-3.0 |

这个项目的价值不在功能表，在三个被写清楚的东西：

**一、什么不做，以及为什么。** 47 个模块明确不迁移，逐条给理由 —— 23 个上游本就没有可搬的实现，18 个框架已有等价能力（审批流 → 工作流引擎、站内信 → 系统通知、SSO → OAuth2），6 个依赖外部服务。

**二、决策连同失败一起留下。** 58 条踩坑记录写在仓库里，包括改错又改回来的那些。

**三、验证可以重跑。** 不靠「我本地点过没问题」，而是一套接口回归加 Playwright 巡检脚本，CI 一把跑完。

→ [实现说明](https://github.com/OceanHAN/openpm/blob/main/docs/IMPLEMENTATION-NOTES.md) · [模块可行性审计](https://github.com/OceanHAN/openpm/blob/main/docs/MODULE-FEASIBILITY-AUDIT.md) · [迁移清单](https://github.com/OceanHAN/openpm/blob/main/docs/MIGRATION-INVENTORY.md)

## 我在意的事

**取舍要留证据。** 说「这个不做」很容易，难的是把不做的成本与收益写下来，让别人能反驳你。

**验证要能重跑。** 手工验收会腐烂，脚本和 CI 不会。

**别重造框架已有的东西。** 能交给框架的能力，自己做就是负债。

## 技术栈

| | |
| --- | --- |
| 后端 | Java · Spring Boot · MyBatis-Plus · MySQL · Redis · Maven |
| 前端 | Vue 3 · TypeScript · Element Plus · Vite |
| 工程 | Docker Compose · systemd · GitHub Actions · Playwright · pytest |

## 其他公开项目

| 仓库 | 说明 |
| --- | --- |
| [filename-export-tool](https://github.com/OceanHAN/filename-export-tool) | 批量提取多层文件夹下的文件名并导出 Excel。面向零基础用户，打包成绿色单 exe，双击即用 |
| [sz-archives-platform](https://github.com/OceanHAN/sz-archives-platform) | 智慧档案平台 monorepo：移动端 Web + 管理后台 + 后端服务 |

---

<div align="center">
<sub>中文提问、issue、PR 都欢迎。</sub>
</div>
