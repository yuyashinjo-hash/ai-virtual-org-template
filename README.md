# AI Virtual Organization Template for Claude Code

> Turn Claude Code into a virtual team that remembers, organizes, and proactively manages your work.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Supported version](https://img.shields.io/badge/Claude%20Code-Pro%2FTeam%2FEnterprise-6A3EA1)](https://claude.com/product/claude-code)

**Free & open-source core (Lite).** For the full 6-department production version, see [Pro edition ($49)](https://shirotools.gumroad.com/l/kgqzwi).

---

## What is this?

A ready-to-use organizational template that transforms Claude Code from a coding assistant into a **virtual organization** with departments, roles, and persistent memory.

Drop the `.company/` folder into any project and Claude Code will:

- **Act as your personal secretary** — a single point of contact that triages, delegates, and tracks everything
- **Automatically record** decisions, learnings, and ideas without being asked
- **Manage TODOs** with priorities and deadlines
- **Run specialized departments** with distinct perspectives and expertise
- **Maintain context across sessions** — no more re-explaining what you were working on

## Who is this for?

- **Solo founders & indie hackers** who want a structured AI co-pilot, not just a chatbot
- **Freelancers & consultants** managing multiple projects and clients
- **Small teams** augmenting their workflow with AI-powered organization
- **Power users of Claude Code** who want to unlock its full potential

## What's included (Lite / this repo)

```
template/
└── .company/
    ├── CLAUDE.md                 # organizational constitution
    ├── secretary/
    │   ├── CLAUDE.md             # secretary role & protocols
    │   ├── inbox/                # quick-capture
    │   ├── todos/                # daily tasks
    │   └── notes/                # decisions & learnings
    ├── engineering/
    │   ├── CLAUDE.md             # technical lead persona
    │   ├── docs/                 # design docs
    │   └── debug-log/            # incident records
    └── research/
        ├── CLAUDE.md             # 4-person panel (strategist / techie / contrarian / lifestyle)
        ├── proposals/            # weekly briefs
        ├── rejected/             # don't re-propose
        └── watchlist/            # defer 1 month
```

Three core departments. For the full production setup (6 departments + SOPs + weekly-review template + 20+ commands), see the Pro edition below.

## Setup (3 minutes)

```bash
git clone https://github.com/shiro-tools/ai-virtual-org-template.git
cd ai-virtual-org-template
cp -r template/.company /path/to/your/project/
```

Then in your project:

```bash
cd /path/to/your/project
claude
# Tell it: "Read .company/CLAUDE.md and start in secretary mode."
```

That's it. No external dependencies.

## Prerequisites

- **Claude Code** (Pro, Team, or Enterprise) — <https://claude.com/product/claude-code>
- A git repository (recommended for persistence across machines)

## License

MIT — use in any project (personal, commercial, client work). Attribution appreciated.

## Author

**shiro** ([@shiro-tools](https://shirotools.gumroad.com)) — runs a small consultancy that automates paperwork, payments, and staff logistics entirely with Claude Code + GAS.

---

## Lite vs Pro

|  | Lite (this repo) | [Pro ($49)](https://shirotools.gumroad.com/l/kgqzwi) |
|---|---|---|
| License | MIT, free | One-time commercial license |
| Departments | 3 (secretary / engineering / research) | **6** (+ sales-marketing / finance-research / corporate-planning) |
| Slash commands | 0 | 20+ (`/save`, `/plan`, `/review`, `/start`, `/bye`, ...) |
| SOPs | No | Yes (startup routine / session-end routine / weekly review) |
| Email/chat support | Community issues | Priority email |
| Updates | Best-effort | Early access to new departments/patterns |
| Use case | "Try the idea, see if it fits" | "Run your solo business on it" |

Buying Pro helps keep the free Lite version maintained.

## Related products

| Package | Price | Purpose |
|---|---|---|
| [Claude Code Starter Kit](https://github.com/shiro-tools/claude-code-starter-kit) (GitHub) / [Gumroad](https://shirotools.gumroad.com/l/mzolhm) | Free / $4.99 | Minimal CLAUDE.md + 3 slash commands — the step before this org template |
| [AI Invoice Manager for Google Workspace](https://shirotools.gumroad.com/l/zmmxo) | $24.99 | PDF → AI-parsed rename → Drive auto-file → Sheets auto-log |
| [JP Compliance Monitor for Claude Code](https://shirotools.gumroad.com/l/lgkuyia) | $9.99 | Japanese compliance auto-check (電帳法 / インボイス) |

## Related articles

- [Claude Codeに"仮想組織"を作ったら、AIが勝手にタスク管理してくれるようになった](https://qiita.com/shiro-tools/items/f3d92d59fe54c1848795) (Qiita, 日本語)
- [CLAUDE.mdが肥大化する本当の原因と、"組織構造"で解決した話](https://qiita.com/shiro-tools/items/4faaf04983e0110505b0) (Qiita, 日本語)

## Contributing

Issues and PRs welcome. Good areas for contribution:

- Additional department templates (finance / sales / legal / etc.)
- Language translations of `CLAUDE.md` files
- Real-world case studies as separate `docs/case-studies/*.md`

## Changelog

- 2026-04-23: v1.0.0 — initial open-source Lite release (extracted from production use)
