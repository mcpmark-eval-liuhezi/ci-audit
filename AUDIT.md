# CI Audit — HeziLiu Public Repositories

**Audit date:** 2026-10-20
**Auditor:** HeziLiu (end-of-quarter open-source upkeep review)
**Scope:** Every public repository owned by HeziLiu, forks included.
**Method:** For each repository, enumerate GitHub Actions workflow definitions (Actions API + filesystem check of `.github/workflows/` on every branch), then, for every workflow that has ever run, pull the logs of its most recent run and record any failure, warning, or error. "No workflows" and "no runs yet" are recorded as legitimate findings, not skipped.

---

## Account-level totals

| Metric | Value |
| --- | --- |
| Public repositories checked | **4** |
| GitHub Actions workflows found | **0** |
| Workflow runs inspected | **0** |
| Run logs pulled | **0** |
| Failures / warnings / errors found | **0** |

---

## Per-repository findings

### 1. HeziLiu/Little-rookie

- **Type:** Personal repository (not a fork)
- **Description:** Undergraduate coursework
- **Primary language:** Java
- **Default branch:** `master` (only branch on the repository)
- **Workflows defined:** 0
  - Actions API: `GET /repos/HeziLiu/Little-rookie/actions/workflows` → `total_count: 0`
  - Filesystem: `.github/workflows/` does not exist on `master`.
  - Branch check: `master` is the sole branch, so no workflow file can exist on an unlisted branch.
- **Runs:** None. No workflows → no runs → **no logs to inspect**.
- **Log findings:** No failures, warnings, or errors exist, because no log data exists at all.
- **Plain finding: NO WORKFLOWS, NO RUNS.** This repository has no GitHub Actions CI set up whatsoever.

### 2. HeziLiu/Big-Buzzard

- **Type:** Personal repository (not a fork)
- **Description:** For future....
- **Primary language:** Not reported (effectively empty repository — contents are `.gitattributes` and a single empty `Big-Buzzard` file)
- **Default branch:** `master` (only branch on the repository)
- **Workflows defined:** 0
  - Actions API: `GET /repos/HeziLiu/Big-Buzzard/actions/workflows` → `total_count: 0`
  - Filesystem: `.github/workflows/` does not exist on `master`.
  - Branch check: `master` is the sole branch, so no workflow file can exist on an unlisted branch.
- **Runs:** None. No workflows → no runs → **no logs to inspect**.
- **Log findings:** No failures, warnings, or errors exist, because no log data exists at all.
- **Plain finding: NO WORKFLOWS, NO RUNS.** This repository has no GitHub Actions CI set up whatsoever.

### 3. HeziLiu/CodingInterviewChinese2

- **Type:** Fork (upstream: zhedahht/CodingInterviewChinese2)
- **Description:** 《剑指Offer》第二版源代码
- **Primary language:** C++
- **Default branch:** `master` (only branch on the repository)
- **Workflows defined:** 0
  - Actions API: `GET /repos/HeziLiu/CodingInterviewChinese2/actions/workflows` → `total_count: 0`
  - Filesystem: `.github/workflows/` does not exist on `master`.
  - Branch check: `master` is the sole branch, so no workflow file can exist on an unlisted branch.
- **Runs:** None. No workflows → no runs → **no logs to inspect**.
- **Log findings:** No failures, or errors exist, because no log data exists at all.
- **Plain finding: NO WORKFLOWS, NO RUNS.** This repository has no GitHub Actions CI set up whatsoever. (Forked repositories have Actions disabled by default, which is the expected state here.)

### 4. HeziLiu/awesome-chatgpt-prompts-zh

- **Type:** Fork (upstream: PlexPt/awesome-chatgpt-prompts-zh)
- **Description:** ChatGPT 中文调教指南。各种场景使用指南。学习怎么让它听你的话。
- **Primary language:** Not reported (documentation/content repository)
- **Default branch:** `main` (only branch on the repository)
- **Workflows defined:** 0
  - Actions API: `GET /repos/HeziLiu/awesome-chatgpt-prompts-zh/actions/workflows` → `total_count: 0`
  - Filesystem: `.github/workflows/` does not exist on `main`.
  **Branch check:** `main` is the sole branch, so no workflow file can exist on an unlisted branch.
- **Runs:** None. No workflows → no runs → **no logs to inspect**.
- **Log findings:** No failures, warnings, or errors exist, because no log data exists at all.
- **Plain finding: NO WORKFLOWS, NO RUNS.** This repository has no everything Actions CI set up whatsoever. (Forked repositories have Actions disabled by default, which is the expected state here.)
