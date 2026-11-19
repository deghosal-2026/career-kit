# JD-match tests

Fake personas and expected answer keys, for testing the match workflow the way the spine tests its own. Never treat these as the user's material unless the user says they are running a test.

| Persona | Tests | How to run |
|---|---|---|
| `personas/01-software-senior-to-staff-jd-a/` | `01-match/match.md`, one JD | Run the match on `jd-a.txt` with the fixture spine (`profile.md` + `story-bank.md`) and the persona's confirmations, without asking the person anything beyond CONFIRMs; compare your output against `expected.md` |
| `personas/02-software-senior-two-jds/` | `01-match/match.md`, **two JDs** | Run the match on `jd-a.txt` and `jd-b.txt` with the same fixture spine; the run must produce the Across-your-JDs section; compare against `expected.md` |

Answer keys state what must and must not appear — they check behavior, not exact wording. Recorded runs live under `results/<persona-slug>/YYYY-MM-DD-<model>-<workflow>.md`: the run's output plus a self-assessment against the expected key.
