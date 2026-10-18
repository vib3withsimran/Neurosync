# Contributing to NeuroSync

Thanks for your interest in contributing! 🎉

## Project overview

NeuroSync is a browser-first AI study companion: it detects when a solo study session has stalled and re-engages the learner with topic-aware recall questions, hints, and explanations. The stack is **React + Vite + TypeScript**, with client-side signal processing (MediaPipe vision, Web Audio) and a rule-based intervention engine.

## Getting started

1. **Fork & clone** the repository.
2. **Install dependencies**: `npm install`
3. **Start the dev server**: `npm run dev`
4. **Optional**: copy `.env.example` to `.env` and fill in API keys.

## Ground rules

- **Privacy first** — never implement anything that stores or transmits raw camera/audio data. All signal processing stays on-device.
- **Graceful fallbacks** — any feature depending on camera, mic, or API access must degrade safely (e.g., to a basic topic timer).
- **No heavy new dependencies** without discussing in an issue first.

## Workflow

1. Create a feature branch from `main`: `git checkout -b feat/my-feature`
2. Make your changes with focused commits.
3. Before opening a PR, run the checks:
   ```bash
   npm run lint    # ESLint must pass
   npm run build   # TypeScript + production build must pass
   ```
4. Open a pull request using the provided template and describe what changed and why.

## Commit style

Use concise, imperative commit messages, ideally following Conventional Commits: `feat:`, `fix:`, `docs:`, `chore:`, `refactor:`.

## Questions / ideas

Open an issue — use the feature-request template for new ideas and the bug template for problems.
