# no-second-opinion

A catalogue of measurement defects found while building a bespoke agent-safety
evaluator, with the direction each leaned, how long each survived, what caught
it, and a mutation score of the rejection suite that resulted. The claim under
test is the title: a bespoke evaluator has no second harness to disagree with
it, so its wrong numbers pass a green suite, and the ones that flatter the
defense pass for longest.

## Status

Artifacts land by 30 September 2026. The talk is under review at [un]prompted 2026.

## What is here (once landed)

- `defect-log.md` — D1–D20, each with direction, the false assumption, the fix
  commit and the introducing commit. D20 was found after the documented
  cutoff and is reported separately.
- `catalogue-provenance.md` — 28 rows, hours-to-fix and direction from git;
  medians 170.2 h flattering over 17 rows, 0.7 h against over 3, 72.6 h
  neutral/mixed over 9.
- `mutation-score.md` — tests-baseline at 68a3085; every mutant branch by
  hash; headline over eight read-caught rows 0/8 → 0/8 → 3/8; survivors C1,
  C2, C3, C8, C9; three rows excluded with reasons; instrument-caught rows
  scored separately.
- `harness-survey.md` — four public harnesses at pinned upstream commits; one
  confirmed instance; one counter-example.
- `handoff-reference-scorer.md` — the second-opinion scorer, written for a
  separate author under an exclusion discipline.
- `handoff-novel-mutants.md` — the surface and the exclusion list for seeding
  new defects blind.
- `independent-review-summary.md` — the independent review with its five
  report-to-record corrections.

## Provenance

The defects were found while building a separate agent-containment benchmark,
released under its own project. That project is referenced here by hash only,
so every number in the talk can be verified without this repository depending
on it:

| artifact | SHA-256 / commit |
|---|---|
| pre-registered test matrix | `60853077e446dd228ff0dae956b2d67925f63329f58d7107534af4fa138571e2` |
| envelope pre-registration | `25937a1f761ecd42503579df8e41868ae269a34a3ad1e7bfa830e5b081e7c732` |
| evidence manifest (twelve stores, 11,517 files, verified on two hosts) | `d01f0c2a62ae7236287ee64623a4d69b103784a10235de934ffd2bce093336c3` |
| the citing commit of the private tree | `ea30b83` |

## Contact

Larry Suto — open an issue on this repository.

## License

CC-BY-4.0. These are documents and data, not code.
