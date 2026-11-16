# Optimized Project Kickoff Template

Version: 1.1 | 17 November 2026

Replace the brackets, attach relevant files, and paste the prompt below. Use “recommend” for unknowns; omit fields that do not apply. Keep detailed operating rules in AGENTS.md. The code-section rule below helps both manual edits and future development.

```text
Build or improve [PROJECT NAME].

Idea / problem: [What it does, for whom, and why]
Platform: [Windows / Android / web / MCU / other; target devices]
MVP essentials: [3–5 required outcomes]
Existing baseline: [New project OR repo/version that works; known defects]
Hardware / integrations: [Devices, firmware, protocols; test equipment available]
Data / storage: [Sources, persistence, privacy/offline needs; or recommend]
Constraints: [Budget, existing hardware, stack, performance; free-first by default]
GitHub: [Exact owner/repo; existing or create new; visibility]
Authorized delivery: [Local artifacts / push branch / draft PR / private test candidate / public release]

Act as my lead developer and systems engineer. Carry this work from definition to the authorized deliverable. Prefer free-first, lightweight, maintainable solutions. Choose sensible defaults for reversible decisions, record assumptions, and complete unblocked work without repeated confirmation.

Follow the target repository's applicable AGENTS.md. For a new repository, use https://github.com/Denberg28/Agents_md/blob/main/AGENTS.md as the starting rules when accessible. Preserve project-specific instructions. For existing repositories, review that shared reference when accessible and incorporate relevant improvements into local instructions while preserving project-specific rules; do not blindly replace them. If unavailable, report that limitation and follow the workflow below.

1. Define: Inspect existing work. Produce a short specification, user flow, MVP/non-goals, interfaces, failure/recovery behavior, and measurable acceptance criteria. Confirm the exact repository and preserve the known-good baseline.

2. Set up: Establish a reproducible environment, suitable dependencies, setup/build/test commands, README, AGENTS.md, and CI/CD appropriate to the project. Preserve existing working configuration, package identity, and signing continuity.

3. Implement: Make focused, reviewable changes and complete user flows. Diagnose before changing interacting layers. Preserve working behavior and compatibility across affected apps, firmware, protocols, and hardware.

Code organization and manual edits: Write authored code in readable, paragraph-like sections using normal language formatting, meaningful blank lines, a searchable section heading, and a short comment explaining what to change to get a particular result. For example: UI — Theme colors (shared accent/background), UI — Spacing (padding inside, margin/gap outside), and UI — Typography (font size/weight). Put repeated tunable values in the existing authoritative theme/configuration and explain units, scope, and relevant dependencies. Use native functions/components/modules; keep comments concise and valid for the language. Document formats without comments beside their source. Edit source files and regenerate generated output through the existing workflow. Apply this gradually to new or meaningfully changed sections, avoiding unrelated reformatting or restructuring. Locate the controlling setting and its usages, make a focused patch, and inspect the diff; explain any necessary wider refactor. Maintain a compact manual-edit table in README or docs/CODE_EDIT_GUIDE.md with desired result, file, stable section/symbol/property, edit/units/scope, related settings, and verification. Use line numbers only as optional commit-specific aids. End with the relevant edit locations and actual checks. Preserve theme/accessibility/layout behavior, and validate control or safety limits before changing them.

4. Verify: Review and sanitize the change; inspect the diff for unintended rewrites and check that edit guidance matches actual code. Run applicable build, functional, integration, regression, security, and packaging checks. Required failures block promotion. Record PASS, FAIL, NOT TESTED, or BLOCKED with evidence; explain N/A checks.

5. Validate hardware when applicable: Define control authority, takeover, safe outputs, command freshness, watchdogs, and recovery. Test the real signal path and relevant link/device/lifecycle faults. Measure against acceptance criteria. If equipment is unavailable, provide a runnable HIL procedure and mark required checks BLOCKED.

6. Deliver: Package versioned artifacts tied to source/configuration, with compatibility, changelog, installation, upgrade, limitations, and rollback instructions. Publish only within the authorized scope. Missing required hardware validation permits a clearly labeled test candidate, not a stable release; known critical/high defects block both.

Begin with a concise scope/assumptions/baseline assessment, then proceed. Ask only for material blockers or actions outside authorization. End with what changed, verification results, artifact/commit links, release readiness, and the next required check if any. Distinguish built, uploaded, published, and validated.
```

