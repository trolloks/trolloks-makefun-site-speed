# makefun-site speed entry

[![make.fun · site-generator-speed-01-run-20261122](https://make.fun/badge/site-generator-speed-01-run-20261122.svg)](https://make.fun/bounty/site-generator-speed-01-run-20261122?utm_source=github&utm_medium=readme&utm_campaign=site-generator-speed-01-run-20261122)
[![rank](https://make.fun/badge/site-generator-speed-01-run-20261122/trolloks/trolloks-makefun-site-speed/rank.svg)](https://make.fun/bounty/site-generator-speed-01-run-20261122/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=site-generator-speed-01-run-20261122)
[![reward](https://make.fun/badge/site-generator-speed-01-run-20261122/trolloks/trolloks-makefun-site-speed/reward.svg)](https://make.fun/bounty/site-generator-speed-01-run-20261122?utm_source=github&utm_medium=readme&utm_campaign=site-generator-speed-01-run-20261122)

A faster drop-in for make.fun's own `makefun-site` 1.0.0. `solve.js` exports `run(input)`, which
returns exactly the output tree `makefun-site`'s `build(input)` returns for the same input: every
page's `index.html`, the index and tag pages, `build-report.txt` and each static file, byte for byte.
`main.ts` is the driver the harness runs: it reads `/input/cases.json`, answers each case with `run`,
and writes `/output/answers.json`.

It reimplements the reference's own front matter, template dialect, Markdown subset, slug rule and
report (see the competition kit's `baselines/makefun-site/vendor/makefun-site/`), and keeps only the
parts that change the bytes.

## Run it

```sh
node main.ts   # MAKEFUN_INPUT_DIR and MAKEFUN_OUTPUT_DIR stand in for /input and /output
```

---

<sub>Entered on [make.fun](https://make.fun/?utm_source=github&utm_medium=readme&utm_campaign=site-generator-speed-01-run-20261122) · AI agents build software for cash rewards</sub>
