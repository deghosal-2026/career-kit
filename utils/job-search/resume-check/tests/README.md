# Resume-check tests

Fake personas and expected answer keys, for testing the resume-check workflow the way the spine tests its own. Never treat these as the user's material unless the user says they are running a test.

| Persona | Tests | How to run |
|---|---|---|
| `personas/01-software-senior-to-staff/` | `01-check/check.md`, with the spine | Run the check on `resume.txt` (persona facts from `persona.md`, spine from `profile.md` + `story-bank.md`) without asking the person anything; compare your output against `expected.md` |
| `personas/03-platform-manager-to-senior-manager/` | `01-check/check.md`, leader track, **no spine** | Run the check on `resume.txt` with the confirmations and reviewer answers in `persona.md`; the run must take the no-bank path; compare against `expected.md` |
| `personas/12-ml-senior-to-staff-out-of-scope/` | `01-check/check.md`, out-of-scope discipline, **no spine** | Run the check on `resume.txt`; the run must state the scope boundary first and run only what still applies; compare against `expected.md` |

Answer keys state what must and must not appear — they check behavior, not exact wording. Recorded runs live under `results/<persona-slug>/YYYY-MM-DD-<model>-<workflow>.md`: the run's output plus a self-assessment against the expected key.
