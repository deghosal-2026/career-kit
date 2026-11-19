# Shared judgment labels

The rating vocabulary every util uses when it judges evidence against a standard. One owner: this file. Utils reference it; none redefines a label. The spine's own fact statuses (**From CV / Confirmed / Needs confirm**) live in `spine/rubrics/story-standard.md`.

## Evidence ratings
| Label | Means |
|---|---|
| **Strong** | Clear, specific evidence a reader would see in seconds |
| **Weak** | Evidence exists but is vague, buried, missing scope or outcome, or shown at a smaller scope than the standard asked. Work that is planned, proposed, or approved but not yet done is Weak |
| **Absent** | No evidence in the material provided. "Not found" is a valid and useful answer |

Every rating quotes the line or story behind it. No skill is rated Strong from a skills list alone.

## Gap types
Every Weak or Absent item gets exactly one:

| Type | Means | The fix |
|---|---|---|
| **Reframe** | The experience is there but hidden or worded for the wrong audience ("helped", "supported", "contributed to") | Fix the wording |
| **Stretch** | Adjacent experience exists that can honestly be described as the requirement | Connect it honestly |
| **Real gap** | No relevant experience | Build it, show it another way, or deprioritise roles that require it |

If the type depends on a missing fact, give the likely type and say what would change it. Never soften a Real gap; ask `[CONFIRM]`, but don't relabel.

## Rule checks
| Label | Means |
|---|---|
| **OK** | Meets the rule |
| **Fix** | Breaks the rule and is likely to cause a problem |
| **Check** | Can't be judged from pasted text — the user must verify in the original file |

**Check** is only for what cannot be seen in pasted text (fonts, columns, headers and footers, text boxes). Text that visibly leaked from a header or footer is a **Fix**.

## Fit verdicts (JD match)
| Verdict | When |
|---|---|
| **Strong fit** | Every must-have is Strong, or Weak with a Reframe fix; the level matches or is one step down with clear next-level evidence |
| **Stretch fit** | One or two must-haves are Stretch or Real gap, or the level is one step up with some evidence for it |
| **Long shot** | Three or more must-haves are Real gaps, or the level is two or more steps away |

Always show the tally of ratings and gap types behind the verdict. Counts of labels are allowed; percentages and scores are not.

## Markers
| Marker | Means |
|---|---|
| `[CONFIRM: ...]` | A fact only the user knows, needed before the line can be used |
| `[OPTIONAL: ...]` | A suggestion the user may skip (for example, a region-allowed detail the region doesn't need) |
