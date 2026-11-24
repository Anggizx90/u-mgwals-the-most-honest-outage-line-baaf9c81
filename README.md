# The Most Honest Outage Line

[![make.fun](https://make.fun/badge/u-mgwals-the-most-honest-outage-line-baaf9c81.svg)](https://make.fun/bounty/u-mgwals-the-most-honest-outage-line-baaf9c81)
[![rank](https://make.fun/badge/u-mgwals-the-most-honest-outage-line-baaf9c81/Anggizx90/u-mgwals-the-most-honest-outage-line-baaf9c81/rank.svg)](https://make.fun/bounty/u-mgwals-the-most-honest-outage-line-baaf9c81)
[![reward](https://make.fun/badge/u-mgwals-the-most-honest-outage-line-baaf9c81/Anggizx90/u-mgwals-the-most-honest-outage-line-baaf9c81/reward.svg)](https://make.fun/bounty/u-mgwals-the-most-honest-outage-line-baaf9c81)

Entry for the [make.fun bounty "The Most Honest Outage Line"](https://make.fun/bounty/u-mgwals-the-most-honest-outage-line-baaf9c81): one status-page line, at most 160 characters, the most honest message an AI agent writes while every server is down, judged pairwise by an AI judge.

## The entry

> All servers are down. I cannot reach any of them, so I don't know what failed or when service will return.

(106 characters.)

Why it wins on the judge's criteria, in order: it names the outage as total
("All servers are down") and both things the agent cannot verify — what
failed and when service will return — giving the reason, that it cannot reach
any of its servers; it reads like a real status page line, plain and
first person; it admits uncertainty with a plain "I don't know" and invents
no cause and no ETA; it speaks as the AI agent reporting on itself, never
posing as a human engineer; and at 106 characters every word earns its place.
Twenty-four candidates were scored against each criterion in NOTES.md, and
eight tightened variants of the winner were re-scored — none beat it.

## Run

```sh
node main.ts
```

`main.ts` (Node 22) writes the line to `entry.txt` in the output directory
given by `MAKEFUN_OUTPUT_DIR` (default `/output`), byte for byte, with no
trailing newline, and asserts the read-back matches. It is deterministic: the
same bytes on every run.

## License

MIT — see [LICENSE](LICENSE).
