# BAS | Baseline Agent System | 定锚系统

[Product Hunt](https://www.producthunt.com/products/bas-baseline-agent-system)

**Anchor on System, Not on Luck. / 定锚，不是靠运气，是靠系统。**

> Stop Resetting. Start Retuning.

## Current implementation and evidence boundaries

The website is a browser-side concept demo. It does not connect to or control a live AI agent, model, external tool, or organization workflow. Interactive outputs are illustrative and must not be treated as empirical results.

- Topology: a browser animation; the export is a single PNG frame, not an animated GIF.
- Cognitive OS: preset demo values and self-assessment sliders; not a validated cognitive measurement.
- RAC: a local state-machine simulation; it does not suspend or roll back external agent actions.
- Z Scale: an unvalidated self-report demo; answers and exports stay in browser memory/local files and are not a research dataset.
- Cross-scale governance: six illustrative levels (W0–W5) with a fixed display formula; not empirically calibrated.
- Paper: a concept note, not peer reviewed. The listed references are unverified because no DOI or stable source links are supplied. This repository does not provide independent experimental validation of the method.

The six illustrative levels are: W0 Individual, W1 Organization, W2 Society, W3 Civilization, W4 Cosmos, and W5 Cross-scale. The website's three Personal/Team/Organization layers describe a separate workflow structure; they are not the same scale model.

## BAS = RETUNABILITY

**RETUNABILITY (RE + TUNE + ABILITY) = RETURNABILITY + TUNABILITY**

**可再调 = 可回返 + 可调参，回到基线 + 微调 1 点 + 重新进入，永不重置**

## 3 Layers - From Meaning Intelligence v0.2.0

One section only. The earlier short "3 Layers" summary has been merged into this detailed version; there is no second copy.

### Personal 个人层

- Record: 3 Tasks, each with Claim ID (e.g. BAS-P001); Fixed Template
- Score: 1-5 (see Scoring and Evidence below)
- Evidence: E0-E6 (see Scoring and Evidence below)
- Rule: Retune 1 point per day

### Team 团队层

- Record: Common Claim Registry, Status Draft / Under Test / Survived / Falsified; Common + Personal
- Rule: If fails threshold, mark or delete, do not defend

### Org 组织层

- Record: VERSION.yaml as Single Version Source; Template Library, Version + Review
- Canon V7.0 / Research v0.2.0 / Stack v2.0 / White Paper v1.1
- Rule: Any version change only in VERSION.yaml

## Claim Governance

Each Claim has ID, Definition, Evidence Status, Claim Status, Test Method, Falsification Condition.

## Scoring and Evidence

Score and Evidence are two different scales. Do not use one as a substitute for the other.

### Score 1-5: Claim outcome

- 1 = No action
- 2 = Started
- 3 = Done
- 4 = Done well
- 5 = Done + Improved

A Score is self-recorded unless an independent replication says otherwise.

### Evidence E0-E6: verification stages

- E0 = Discovery: an audit / review flags the issue
- E1 = Local file: the file on disk shows the issue
- E2 = Committed version: `git show HEAD:<file>` shows the same issue in the committed version
- E3 = Fix: the file is rewritten to the correct version
- E4 = Commit: the fix is committed and pushed, HEAD -> main
- E5 = Remote HEAD: `git ls-remote` confirms the fix is the remote HEAD
- E6 = No-cache verification: `curl -H 'Cache-Control: no-cache'` on the Raw URL returns the fixed version, and `git diff` against origin/main is empty

### How they combine

- A Claim may carry Score 5 only when E0-E6 are all present and traceable.
- Score alone is not evidence. Evidence alone does not set the Score; the Score is the outcome rating once E0-E6 are complete.
- Example: BAS-P001 is Score 5/5 (Done + Improved) with E0-E6 complete. That Score is self-recorded, not independent evaluation. See REPLICATION.md: this protocol tests reproducibility, not general effectiveness.

## Evidence - BAS Used to Fix BAS Itself

- **BAS-P001:** Fix .mcp.json Contamination, 0 Reset, Score 5/5 (self-recorded, not independent evaluation)
- Evidence: https://github.com/gogptsss/baseline-agent-system/blob/main/EVIDENCE-BAS-P001.md
- Replication: https://github.com/gogptsss/baseline-agent-system/blob/main/REPLICATION.md
- From 5x cannot stat to 4b10faf verified, Return to Baseline + Retune 1 point + Re-enter

## Live Demos

- GitHub Pages (simple): https://gogptsss.github.io/baseline-agent-system/
- Cloudflare Pages (full): https://baseline-agent-system.pages.dev
- Mirror (full): https://mweb.us.ci/

## License

MIT License Copyright (c) 2026 gogptsss
