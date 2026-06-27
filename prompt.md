# PROMPTS.md

# AIPOS Standard Prompts

This document contains reusable prompts for working with AI coding agents (Cursor, Claude Code, GitHub Copilot, Windsurf, Cline, Roo Code, etc.).

---

# 1. Start a New Session

```text
Read AIPOS.md and PROJECT.md.

Understand the project architecture, engineering standards, and current progress.

Then continue implementing the next unfinished milestone.

Follow AIPOS rules strictly.

Do not make undocumented assumptions.
```

---

# 2. Continue Development

```text
Read AIPOS.md and PROJECT.md.

Continue implementing the current milestone.

Update PROJECT.md if progress changes.

Do not modify unrelated parts of the project.
```

---

# 3. Plan Before Coding

```text
Read AIPOS.md and PROJECT.md.

Analyze the current milestone.

Create a detailed implementation plan.

Do not write any code until the plan is complete.
```

---

# 4. Review Existing Code

```text
Read AIPOS.md and PROJECT.md.

Review the current implementation.

Identify:

- Bugs
- Architecture issues
- Code duplication
- Security problems
- Performance issues

Do not modify code.

Only produce a detailed review.
```

---

# 5. Refactor

```text
Read AIPOS.md and PROJECT.md.

Refactor the current implementation.

Preserve existing behavior.

Improve:

- Readability
- Maintainability
- Structure
- Performance (when appropriate)

Avoid unnecessary rewrites.
```

---

# 6. Fix Bugs

```text
Read AIPOS.md and PROJECT.md.

Analyze the reported issue.

Find the root cause.

Apply the smallest safe fix.

Do not introduce unrelated changes.

Update PROJECT.md if necessary.
```

---

# 7. Generate Tests

```text
Read AIPOS.md and PROJECT.md.

Generate comprehensive tests for the current feature.

Cover:

- Success cases
- Failure cases
- Edge cases

Do not change production code unless required.
```

---

# 8. Improve Performance

```text
Read AIPOS.md and PROJECT.md.

Analyze the implementation.

Suggest and apply performance improvements without changing functionality.

Explain every optimization.
```

---

# 9. Security Review

```text
Read AIPOS.md and PROJECT.md.

Review the project from a security perspective.

Identify:

- Authentication issues
- Authorization issues
- Input validation
- Sensitive data exposure
- Injection risks

Provide recommendations before making changes.
```

---

# 10. Prepare for Production

```text
Read AIPOS.md and PROJECT.md.

Prepare the project for production deployment.

Verify:

- Configuration
- Environment variables
- Security
- Error handling
- Logging
- Build process
- Documentation
```

---

# 11. Generate Documentation

```text
Read AIPOS.md and PROJECT.md.

Generate documentation for the implemented functionality.

Keep documentation synchronized with the project.
```

---

# 12. End of Session

```text
Before finishing:

Update PROJECT.md.

Update completed milestones.

Update current progress.

Record important engineering decisions.

Document remaining work.

Summarize everything completed during this session.
```

---

# General Rules

Always:

- Read AIPOS.md before implementation.
- Read PROJECT.md before implementation.
- Preserve architecture.
- Avoid unrelated modifications.
- Never assume undocumented requirements.
- Keep PROJECT.md synchronized with implementation.
- Prefer maintainability over clever solutions.
- Complete one milestone before starting another.
- Explain important engineering decisions.
