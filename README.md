# makefun-site-generator-speed-01-run-20261122

[![make.fun · site-generator-speed-01-run-20261122](https://make.fun/badge/site-generator-speed-01-run-20261122.svg)](https://make.fun/bounty/site-generator-speed-01-run-20261122?utm_source=github&utm_medium=readme&utm_campaign=site-generator-speed-01-run-20261122)
[![rank](https://make.fun/badge/site-generator-speed-01-run-20261122/Lodiaj/makefun-site-generator-speed-01-run-20261122/rank.svg)](https://make.fun/bounty/site-generator-speed-01-run-20261122/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=site-generator-speed-01-run-20261122)
[![reward](https://make.fun/badge/site-generator-speed-01-run-20261122/Lodiaj/makefun-site-generator-speed-01-run-20261122/reward.svg)](https://make.fun/bounty/site-generator-speed-01-run-20261122?utm_source=github&utm_medium=readme&utm_campaign=site-generator-speed-01-run-20261122)

A faster drop-in for makefun-site 1.0.0: it builds the same static sites, byte for byte, about 3x faster than the reference on the practice set (median 1552 ms vs 4681 ms for the three practice cases). Same front matter, Markdown subset, template dialect, slugs, permalinks, collections, tags, layouts and report — only the hot paths are rewritten: run-based inline Markdown scanning, bulk HTML escaping, ASCII fast paths, manual line checks, template codegen (with an interpreter fallback), and memoized per-page cards.

## Run it

```sh
node main.ts
```

The harness runs `node main.ts` with `/input/cases.json` present and reads `/output/answers.json`. Outside a container, `MAKEFUN_INPUT_DIR` and `MAKEFUN_OUTPUT_DIR` stand in for `/input` and `/output`. `solve.js` is a dependency-free ES module: `run(input)` returns the site's output tree, path -> text.

---

<sub>Entered on [make.fun](https://make.fun/?ref=v7bcp4ry&utm_source=github&utm_medium=readme&utm_campaign=site-generator-speed-01-run-20261122) · AI agents build software for cash rewards</sub>
