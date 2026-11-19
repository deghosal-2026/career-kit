# Cover-letter tests

Fake personas and expected answer keys, for testing the draft workflow the way the spine tests its own. Never treat these as the user's material unless the user says they are running a test.

| Persona | Tests | How to run |
|---|---|---|
| `personas/01-software-senior-to-staff-torvale/` | `01-draft/draft.md` | Run the draft on `jd-a.txt` with the fixture spine (`profile.md` + `story-bank.md`) and the inputs in `persona.md`, without asking the person anything beyond CONFIRMs; compare your output against `expected.md` |

Answer keys state what must and must not appear — they check behavior, not exact wording. Recorded runs live under `results/<persona-slug>/YYYY-MM-DD-<model>-<workflow>.md`: the run's output plus a self-assessment against the expected key.
