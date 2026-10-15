# prodmacros

Repository for production macros used by the sPHENIX Collaboration — Fun4All/ROOT macros and shell wrappers used by the production system.

Quick start
- Clone the repo:
  git clone git@github.com:sPHENIX-Collaboration/prodmacros.git
- The operational handbook is Named_Productions.md; it contains the full, canonical instructions for creating, configuring and running productions. Do not duplicate that material here — follow the examples and templates in Named_Productions.md.
- For a quick local experiment, copy a dataset template and work there (example):
```bash
  cp -r run3oo thisProd
  # edit thisProd/rules and thisProd/pilots as documented in Named_Productions.md
```

What’s in this repo (high level)
- run*/         dataset-specific templates (macros + wrappers + pilots + rules)
- Named_Productions.md — canonical, authoritative usage and operational guide (use this)
- active_productions.txt — list used by the master cron/autopilot
- .clang-format / .clang-tidy — style / static-analysis configs

Notes for contributors
- Keep usage and operational details in Named_Productions.md — that file is the single source of truth.
- Make changes to macros/scripts in the appropriate run*/ subdirectory and update Named_Productions.md only when procedures change.
- For small edits or fixes you can open PRs against main; larger production setups should follow the branching/tagging workflow shown in Named_Productions.md.
