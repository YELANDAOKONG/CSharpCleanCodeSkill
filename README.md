# C# Clean Code Skill

An AI agent skill that enforces C# clean code conventions across any .NET project.

## Overview

This skill provides a comprehensive C# style guide with **12 mandatory rules** (blockers) and **18 recommended rules** (strongly encouraged). When loaded by an AI coding agent, it guides code review, refactoring, and generation to follow consistent, readable C# patterns.

## Structure

```
.agents/skills/csharp-clean-code/
  SKILL.md    # Full style guide with rules, examples, and quick-review checklist
```

## Highlights

**Mandatory rules** include:
- File-scoped namespaces
- English for all user-facing messages
- PascalCase/camelCase/`_camelCase` naming conventions
- Language keywords over CLR types (`string` not `String`)
- Braces on all control flow; `switch` must have default
- Explicit `Main` method (no top-level statements)
- No magic numbers; one type per file
- Exceptions only for exceptional conditions, with `nameof(param)`

**Recommended rules** include:
- `using` declarations, expression-bodied members, pattern matching
- Null-conditional operators, string interpolation, collection expressions
- `nameof()`, records for immutable data, proper async/await
- Comment "why" not "what", avoid double negatives and nested loops
- Declare variables late, one per statement, avoid `ref`/`out`

## Usage

This skill works with any AI coding agent (OpenCode, Claude, Cursor, etc.). Once installed, the agent applies these rules automatically when writing, reviewing, or refactoring C# code.
