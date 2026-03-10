# kiro-usability-feedback-agent

Reviews your UX screens for visual issues and simulates a real user clicking through a task to find where they'd get confused.

---

## What it does

**Mode 1 — Visual & Accessibility Audit**  
Drop in a screenshot and it checks:

- Color contrast ratios against WCAG 2.2 AA standards
- Visual hierarchy — is it clear what to do on this screen?
- Tap and click target sizes
- Missing interaction states (focus, hover, disabled, loading)

Every issue is rated Critical, High, Medium, or Low so you know what to fix before ship.

**Mode 2 — Cognitive Walkthrough**  
Give it a task like "try to create a canary" and it acts as a first-time user — narrating exactly where it looks, what it clicks, and where it gets confused. Each step gets a confidence rating so you can see precisely where the UI is ambiguous.

You can run both modes on the same screen.

---

## How to use

1. Pull this repo `kiro-usability-feedback-agent`
2. Open the project in Kiro — the agent loads automatically
3. Drop in a screenshot and say one of the following:

**For a visual audit:**  
> "Audit this screen"

**For a cognitive walkthrough:**  
> "Try to do X" or "Where would you click to create a canary?"

**For both:**  
> "Audit this screen and then try to complete X"

---

## Who it's for

Designers, product managers, and engineers who want fast usability and accessibility feedback without scheduling a formal review.

---

## File structure
```
.kiro/
  agents/
    usability-agent.md   ← the agent system prompt
README.md
```

---

## Updating the agent

The agent lives in `.kiro/agents/usability-agent.md`. Edit that file to add your product's specific screens, terminology, or design system context. Commit and push — everyone on the team gets the update on their next pull.




