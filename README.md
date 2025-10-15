# 🟩 MyStreako

**MyStreako** is a minimal, privacy‑first habit tracker with a GitHub‑style activity grid. Log a single daily
check‑in per habit, see your streaks at a glance, and choose what’s public or private. Built to make showing up every
day effortless.

## Overview

MyStreako works like a lightweight social layer around habits. Create habits, track daily check‑ins, and (optionally)
share your progress publicly. Keep your profile private, or showcase selected habits.

Future iterations emphasize honest visuals (no vanity metrics), long‑term views, and simple sharing.

## MVP Features

- User authentication and profile pages (Supabase Auth)
- Create habits with per‑habit visibility (public or private)
- One daily check‑in per habit (binary), validated in UTC (no duplicates)
- Dashboard with a 365‑day grid per habit
- Habit detail page with a 5‑year activity grid
- Public profile page to view public habits (read‑only)

## Future Roadmap

- Streak badges and gentle nudges (no gamification overload)
- Shareable links with minimal public views
- CSV export/import of check‑ins
- Dark mode and accessibility improvements

## Tech Stack (Planned)

- **Frontend:** React, Vite, Tailwind CSS, TypeScript
- **Database & Auth:** Supabase (Postgres, Auth, Realtime)

## Repo Structure

```text
mystreako-app/
├── docs/        # Documentation (entities, user flows, roadmap, contributing, etc.)
├── src/         # Client application (React + Vite + TS + Tailwind)
├── .github/     # GitHub workflows and issue/PR templates
└── README.md    # This file
```

## Contributing

We welcome contributions from friends, interested developers, and the community! See
our [Contributing Guide](/docs/contributing.md)
for details on branches, commits, and PR workflow.

- Documentation in docs/ is our source of truth (entities, flows, roadmap).
- GitHub Project Board maps features and tasks.
- Contributions always follow the MVP-first principle: no features are added unless the core backlog experience is
  solid.

---

> “Show up once a day, see the truth in your grid, and let consistency do the rest.”
