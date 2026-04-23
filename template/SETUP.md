# Setup Guide

Get your AI Virtual Organization running in 5 minutes.

## Prerequisites

- **Claude Code** installed and working (requires Claude Pro, Team, or Enterprise)
- A project directory (new or existing -- the template won't interfere with your code)

## Step 1: Copy the Template

Copy the entire `.company/` folder into your project root:

```
your-project/
├── .company/          <-- Copy this here
│   ├── CLAUDE.md
│   ├── secretary/
│   ├── engineering/
│   └── research/
├── your-existing-files...
```

## Step 2: Edit Your Profile

Open `.company/CLAUDE.md` and fill in the **Owner Profile** section:

```markdown
## Owner Profile

- **Name**: Jane Smith
- **Business / Activity**: SaaS startup building project management tools
- **Goals**: Ship MVP by Q3, automate customer onboarding, reduce manual ops
- **Created**: 2026-04-07
```

This helps the Secretary and other departments tailor their responses to your context.

## Step 3: Customize Departments (Optional)

The template comes with 3 departments. You can:

### Keep as-is
The defaults work well for most solo founders and small teams.

### Modify existing departments
Edit any department's `CLAUDE.md` to adjust:
- **Tone**: Make it more formal, more casual, or match your company culture
- **Virtual team members**: Rename them, change their perspectives, add domain expertise
- **Rules**: Add department-specific conventions

### Add new departments
1. Create a new folder: `.company/your-department/`
2. Add a `CLAUDE.md` with Role, Rules, and Folder Structure sections
3. Register it in `.company/CLAUDE.md` under the Departments table
4. Create any subfolders the department needs (e.g., `docs/`, `reports/`)

**Example departments you might add:**
- `marketing/` -- Content calendar, brand voice guidelines, campaign tracking
- `finance/` -- Budget tracking, invoice management, expense categorization
- `sales/` -- Pipeline management, client notes, proposal templates
- `legal/` -- Contract reviews, compliance checklists, policy documents

## Step 4: Add Integrations (Optional)

The Secretary department supports optional external integrations. Edit `.company/secretary/CLAUDE.md` to add:

```markdown
### Optional: External Integrations
- **Task database**: Notion DB `your-database-id-here`
- **Calendar**: Google Calendar `your-calendar-id@group.calendar.google.com`
```

## Step 5: Start Using It

Launch Claude Code in your project directory and say:

> "Read .company/CLAUDE.md and operate as my virtual organization."

From that point on, the Secretary will be your primary interface. Try:

- **"What should I work on today?"** -- Secretary reviews TODOs and priorities
- **"I need to design a new API. Let's discuss."** -- Engineering team debates the approach
- **"I had an idea about expanding to Europe."** -- Captured in inbox, Research dept analyzes it
- **"Add a TODO: finish onboarding flow by Friday, high priority"** -- Task tracked
- **"Let's wrap up for today."** -- Session end routine: log decisions, update TODOs, prepare handoff

## Tips for Best Results

1. **Be consistent**: Start and end sessions with the routines. Context compounds over time.
2. **Let it record**: Don't worry about manually noting things. The system captures decisions and ideas automatically.
3. **Use the inbox**: When you have a thought that doesn't fit anywhere, just say it. The Secretary puts it in inbox for later processing.
4. **Review weekly**: Check `secretary/notes/` and `research/proposals/` once a week to see what's been captured and proposed.
5. **Commit regularly**: The `.company/` folder works best under version control. Commit after each session to preserve history.

## Folder Reference

```
.company/
├── CLAUDE.md                          # Organization config (edit this first)
├── secretary/
│   ├── CLAUDE.md                      # Secretary department config
│   ├── inbox/                         # Quick captures, unsorted ideas
│   │   └── YYYY-MM-DD.md             # Daily inbox entries
│   ├── todos/                         # Daily task files
│   │   └── YYYY-MM-DD.md             # Today's task list
│   └── notes/                         # Decision logs, memos
│       ├── YYYY-MM-DD-decisions.md    # Decisions made on this date
│       ├── YYYY-MM-DD-learnings.md    # Learnings captured on this date
│       └── topic-name.md             # Topic-specific notes
├── engineering/
│   ├── CLAUDE.md                      # Engineering department config
│   ├── docs/                          # Technical docs & design docs
│   └── debug-log/                     # Bug investigation logs
└── research/
    ├── CLAUDE.md                      # Research department config
    ├── proposals/                     # Research proposals
    ├── rejected/                      # Rejected ideas (don't repeat)
    └── watchlist/                     # Deferred ideas (revisit later)
```
