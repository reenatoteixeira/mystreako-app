# MyStreako Contributing Guide

Welcome 👋 and thank you for your interest in contributing to **MyStreako**!
This guide explains how we work so collaboration stays smooth and productive.

---

## Prerequisites

- Node.js ≥ 18 (LTS recommended)
- npm (repo assumes npm scripts; adapt if using pnpm/yarn)
- Git
- Supabase project (only needed for features that touch the DB)

## Quick Setup

```bash
git clone https://github.com/reenatoteixeira/mystreako-app.git
cd mystreako-app
npm install
cp .env.example .env.local  # if available
npm run dev
```

## Useful Scripts

```bash
npm run dev          # Start the development server
npm run build        # Build for production
npm run preview      # Preview the production build
npm run lint         # Run ESLint
npm run format       # Run Prettier
```

> Husky is set up to run lint and format checks on commits.

## Git Flow Overview

We use a **branch-based workflow** where development happens in short-lived feature branches.
The general flow is:

1. Branch from `stage`
2. Work on your changes in a `feature/*` (or `fix/*`, `chore/*`) branch
3. Open a Pull Request (PR) into `stage`
4. After review and tests, changes are merged into `stage`
5. From time to time, `stage` is promoted into `main`

> This way:
>
> - `main` is stable, with production-ready code.
> - `stage` is the integration branch, where new changes come together before production.
> - `feature/*` is where individual development happens.

## Creating a Branch

All new work should happen in a **feature branch**:

```bash
git checkout stage
git pull origin stage
git checkout -b feature/short-description
```

> Examples:
>
> - feature/auth-flow
> - feature/games-search
> - fix/navbar-overlap
> - chore/setup-tailwind

## Commit Messages

We follow the [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/) specification for commit messages.
This makes the history cleaner and allows us to generate changelogs automatically.

Format:

```text
type: short description
```

Types we use:

```text
feat: a new feature
fix: a bug fix
docs: documentation changes
chore: configs, dependencies, maintenance
refactor: code improvement without feature change
test: add or update tests
```

> Examples:
>
> - feat: implement basic Supabase login
> - fix: handle empty search results gracefully
> - docs: add contributing guide

## Pull Requests

When your feature is ready:

1. Push your branch to the remote repository:
   ```bash
   git push origin feature/short-description
   ```
2. Open a Pull Request (PR) from your feature branch into `stage`.
3. Fill out the PR template with relevant details.
4. Request reviews from team members.

> After review and approval, it will be merged into `stage`. Eventually, `stage` will be promoted to `main` for
> production releases.

## Issues & Labels

Open issues for bugs, improvements, or ideas. We use labels to categorize and prioritize them.

## Final Note

Contributions from friends, the community, or curious developers are welcome! Even small changes, like fixing a typo,
improving documentation, adding comments, make a big difference.

Thank you for helping make MyStreako better! 💚
