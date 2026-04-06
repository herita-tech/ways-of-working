Pull the comments from the Github Pull request for the current branch.

For each comment, evaluate it and decide if it should be fixed or not.

Use your own judgement to decide. The comments aren't automatically right, but many are.

For each comment, you should reply to that comment on Github.co with a categorised response using the severity and emoji from the table below, plus a disposition:

Format: `{emoji} {Category} · #{WillFix|WontFix} — [reason]`

Example: `🧨 Production Risk · #WillFix — missing null check will crash on empty input`

If there's already a response comment from us, don't duplicate it — but update it if the category or disposition should change.

---

## Severity & Category Reference

### 🔴 Critical

| Emoji | Category        | Use when                                                                          |
| ----- | --------------- | --------------------------------------------------------------------------------- |
| 💥    | Breaking        | Breaks API contracts, migrations, backward compatibility, or core flows           |
| 🧨    | Production Risk | Likely to cause outage, data corruption, or major instability                     |
| 🔐    | Security        | Auth flaws, injection risks, secrets exposed, privilege escalation, unsafe crypto |
| 🧬    | Data Integrity  | Race conditions, ledger imbalance, non-idempotent operations, transaction bugs    |

### 🟠 Major

| Emoji | Category        | Use when                                                      |
| ----- | --------------- | ------------------------------------------------------------- |
| 🧱    | Architecture    | Violates layering, leaks domain logic, breaks boundaries      |
| 🧵    | Concurrency     | Async bugs, missing awaits, deadlocks, race potential         |
| 🧮    | Financial Logic | Rounding errors, precision loss, incorrect fee calculation    |
| 📉    | Performance     | N+1 queries, unnecessary re-renders, heavy loops, blocking IO |
| 🧪    | Missing Tests   | Critical path change without adequate coverage                |

### 🟡 Minor

| Emoji | Category         | Use when                                                 |
| ----- | ---------------- | -------------------------------------------------------- |
| 🧹    | Cleanup          | Refactor opportunity, simplify logic, remove duplication |
| 🏷️    | Naming           | Confusing variable/function names                        |
| 🧭    | DX / Readability | Hard to follow logic, unclear intent, magic numbers      |
| 📝    | Docs             | Missing or outdated comments, README updates needed      |

### 🟢 Nit / Style

| Emoji | Category           | Use when                           |
| ----- | ------------------ | ---------------------------------- |
| 🎨    | Formatting         | Linting, spacing, stylistic tweaks |
| 🔤    | Typo               | Spelling, grammar, copy issues     |
| 🧊    | Micro-optimization | Tiny improvement, non-blocking     |

### 🟣 Optional / Suggestion

| Emoji | Category        | Use when                             |
| ----- | --------------- | ------------------------------------ |
| 💡    | Idea            | Alternative approach suggestion      |
| 🚀    | Enhancement     | Nice-to-have improvement             |
| 🔮    | Future-proofing | Will matter when scaling / extending |

---

## Rules

- Pick the single most fitting category per comment.
- Always lead with the emoji so the thread is scannable.
- Default to `#WillFix` when the comment is valid. Use `#WontFix` with a clear reason.
- For 🔴 Critical items, prioritise fixing immediately.
- For 🟣 Optional items, it's fine to `#WontFix` with acknowledgement.

Finally, update the title + description of the PR as the scope might have changed since we first created it.
