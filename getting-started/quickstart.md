# Quick Start

Get productive with Vexorbis in 5 minutes.

## Step 1: Search Your Codebase

Try the hybrid search tool:

```
Find all functions that handle user authentication
```

**What happens:** Vexorbis uses HippoRAG's AST graph to find semantically related code, not just text matches.

## Step 2: Create a PLAN.md

Create a `PLAN.md` file in your project root:

```markdown
# Sprint 1

## Todo
- [ ] Add input validation to login endpoint @engineer
  - Context: src/auth/login.py
- [ ] Review authentication security @auditor
```

**What happens:** Vexorbis reads this file and treats each `[ ]` item as a pending task.

## Step 3: Let Vexorbis Work

Tell your AI:

```
Process the next pending task from PLAN.md
```

**What happens:**
1. Vexorbis picks up the first `[ ]` task
2. Assigns it to the `@engineer` role
3. Pre loads `login.py` into context
4. Executes the task
5. Marks it `[x]` when complete

## Step 4: Auto Commit Changes

If you have uncommitted changes, Vexorbis can commit them:

```
Commit my changes with an appropriate message
```

**What happens:** The Git Agent generates a conventional commit message and stages your files.

## Step 5: Debug a Failing Test

When tests fail:

```
My tests are failing, help me debug
```

**What happens:** Ochiai SBFL runs your test suite with coverage and reports the most suspicious lines of code.

---

## What Vexorbis Did

| You Said | Vexorbis Used |
|----------|------------|
| "Find functions..." | HippoRAG (semantic search) |
| "Process task..." | Role Dispatch (Engineer) |
| "Commit changes..." | Git Agent Team |
| "Debug tests..." | Ochiai SBFL |

## Next Steps

- [Using PLAN.md](../guides/plan-syntax.md) — Full syntax reference
- [Tools Reference](../reference/tools.md) — All available tools
- [Decision Logic](../concepts/decision-logic.md) — How Vexorbis chooses what to do
