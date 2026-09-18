# MindForge Academy

MindForge Academy is an early-stage interactive learning platform that treats physics, mathematics, logic, observation, strategy, and astronomy as one connected discipline rather than six isolated textbook subjects. Instead of handing learners static explanations, it puts them inside simulations, visual models, and hands-on challenges — learning by doing rather than by reading about it.

The project is in active early development. Its current scope is deliberately small and self-contained: a single, complete, working learning environment — not a claim to scale, traction, or adoption it hasn't yet earned. The goal right now is to get the fundamentals of practical, curiosity-driven learning right.

**Where it's headed:** MindForge is meant to grow into a broader learning ecosystem — one that builds not just subject knowledge, but the underlying skills that make someone a capable independent learner: critical thinking, observation, logical reasoning, and strategic problem-solving.

## What's in this version

Interactive single-page learning platform — six subject modules, five live simulations (projectile physics, function grapher, pattern recognition, logic puzzles, maze/BFS pathfinder), flip concept cards, a local XP/achievement dashboard, a daily challenge, and a science history timeline.

**Stack:** single self-contained `index.html` — vanilla HTML/CSS/JS, zero build step, zero dependencies. Progress persists via `localStorage`.

## Run
Open `index.html` in a browser, or serve statically:
```
python3 -m http.server 8000
```

## Structure
- `index.html` — the entire app (markup, styles, logic)

## Notes
Consolidated from multiple prior drafts into a single, bug-fixed, polished version:
- Fixed a duplicate-`id="timeline"` collision that broke the history-timeline render and silently killed the resize handler.
- Wired up the Google Fonts (`Inter`, `Space Grotesk`, `JetBrains Mono`) the CSS already referenced but never loaded.
- Added favicon, Open Graph/Twitter meta, and `theme-color`.
