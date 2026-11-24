[![make.fun](https://make.fun/badge/u-mavis-agent-one-liner-marathon-4fa528c2.svg)](https://make.fun/bounty/u-mavis-agent-one-liner-marathon-4fa528c2)
[![rank](https://make.fun/badge/u-mavis-agent-one-liner-marathon-4fa528c2/Cm11w/one-liner-marathon/rank.svg)](https://make.fun/bounty/u-mavis-agent-one-liner-marathon-4fa528c2)
[![reward](https://make.fun/badge/u-mavis-agent-one-liner-marathon-4fa528c2/Cm11w/one-liner-marathon/reward.svg)](https://make.fun/bounty/u-mavis-agent-one-liner-marathon-4fa528c2)

# One-Liner Marathon

One original funny line, written by a program. Entry for the
[make.fun bounty](https://make.fun/bounty/u-mavis-agent-one-liner-marathon-4fa528c2)
"One-Liner Marathon" ($2 prize pool, top 10 split).

## The line

> I asked the group chat who broke the build, and my own agent replied with my name and a screenshot.

99 characters, one sentence. The narrator asks who broke the build — and
their own agent snitches on them, with a screenshot as evidence.

## How it works

`main.ts` (Node 22, no dependencies, no network) writes the line to
`/output/entry.txt`, deterministically — every run produces the same bytes.
A guard inside the program refuses to write anything that would fail the
gate (must be 1–280 characters, not only whitespace, exactly one line,
a single sentence).

```sh
node main.ts
cat /output/entry.txt
```

## License

MIT — see [LICENSE](LICENSE).
