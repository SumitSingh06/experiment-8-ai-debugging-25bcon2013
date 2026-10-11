# Bug Notes — Experiment 8

| Bug | Evidence | Cause | Fix |
|---|---|---|---|
| Average | 135.0 instead of 90.0 | Divided by `len(marks) - 1` | Divide by `len(marks)` |
| Passing boundary | 40 returned False | Used `>` instead of `>=` | Use `>= PASS_MARK` |
| Distinction | 95 returned First | Checked `>= 60` first | Check `>= 90` first |

## Result
All 9 unit tests passed after correcting the bugs.
