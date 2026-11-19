# Spine tests

Fake personas and expected answer keys, for testing the spine workflows. Never treat these as the user's material unless the user says they are running a test.

| Persona | Tests | How to run |
|---|---|---|
| `personas/01-software-senior-capture/` | `01-capture/capture.md` | Run the capture workflow on `persona.md` without asking the person anything; compare your output against `expected.md` |

Add one persona per workflow when a new workflow ships. Answer keys state what must and must not appear, they check behavior, not exact wording. Recorded runs live under `results/<persona-slug>/YYYY-MM-DD-<model>-<workflow>.md`: the run's output plus a self-assessment against the expected key.
