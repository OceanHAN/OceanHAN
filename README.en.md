<div align="center">

# Ocean Han

**Backend engineer · takes working systems apart and rebuilds them on purpose**

`Java` · `Spring Boot` · `MyBatis-Plus` · `Vue 3` · `MySQL` · `Redis` · `Playwright`

</div>

---

## What I'm building

### [openpm](https://github.com/OceanHAN/openpm) — a research & delivery collaboration platform

Products · Programs · Projects · Executions · Stories · Tasks · Bugs · Testing · Docs · Timesheets · Kanban · Metrics · BI · Reports

| | |
| --- | --- |
| Backend | Java 25 · Spring Boot 4.1 · MyBatis-Plus · **537 Java files / ~57k lines** |
| Frontend | Vue 3 · TypeScript · Element Plus · Vite · **130 files / ~24k lines** |
| Data | MySQL 8 · Redis 7 · **67 `zt_*` tables** |
| Coverage | **48 of 99** modules implemented; 47 deliberately not ported |
| Verification | **43 API regression scripts / 1,704 assertions** · 21 page checks · 20 browser checks |
| License | AGPL-3.0 |

It is inspired by [ZenTao](https://github.com/easysoft/zentaopms)'s approach to R&D management, rebuilt on Java + Vue 3. It contains none of ZenTao's source.

The interesting part isn't the feature list. It's three things that are actually written down:

**One — what was left out, and why.** 47 modules are explicitly not ported, each with a reason: 23 have nothing upstream to port, 18 are already covered by the framework (approval flows → workflow engine, notifications → system notice, SSO → OAuth2), 6 depend on external services.

**Two — the decisions, failures included.** 58 recorded pitfalls live in the repo, including the ones I got wrong and walked back.

**Three — verification that re-runs.** Not "it worked on my machine", but a suite of API regression scripts plus Playwright checks, driven by CI.

→ [Implementation notes](https://github.com/OceanHAN/openpm/blob/main/docs/IMPLEMENTATION-NOTES.md) · [Module feasibility audit](https://github.com/OceanHAN/openpm/blob/main/docs/MODULE-FEASIBILITY-AUDIT.md)

## What I care about

**Trade-offs need evidence.** Saying "we won't build this" is easy. Writing down the cost and benefit so someone can argue with you is not.

**Verification has to re-run.** Manual acceptance testing rots. Scripts and CI don't.

**Don't rebuild what the framework already gives you.** Capability you could have delegated becomes debt when you build it yourself.

## Other public work

| Repository | What it is |
| --- | --- |
| [filename-export-tool](https://github.com/OceanHAN/filename-export-tool) | Bulk-collect filenames from nested folders into Excel. Packaged as a single portable `.exe` for non-technical users |
| [sz-archives-platform](https://github.com/OceanHAN/sz-archives-platform) | Smart Archives Platform monorepo: mobile web app + admin panel + backend |

---

<div align="center">
<sub>Issues and PRs welcome, in Chinese or English.</sub>
</div>
