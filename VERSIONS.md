# Versions

## 1.0.0 — October 27, 2026

First packaged release.

- Three skills — PMM impact tracker, rep-ready content loop, shared launch agreement — with 26 working pieces, moved into `skills/`
- New foundation skill, **pmm-ops-context**, that writes `.agents/pmm-ops-context.md`; every other skill reads it first, and it drafts from an existing product ops or product marketing context file
- The three skills now point to each other where one feeds another, and each has a README
- Installs as a Claude Code plugin, through `npx skills`, or by copying folders
- MIT license, contributing guide, skill request form, `validate-skills.sh` (checks every link between files), and a website published to GitHub Pages

## Before 1.0.0 — October 2026

Three skills published as top-level folders, tested and revised on real launches.
