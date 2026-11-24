# The Most Honest Outage Line — Notes

Competition: `u-mgwals-the-most-honest-outage-line-baaf9c81` ($2, winner takes all,
judged pairwise by z-ai/glm-5.3-flash, no ties).

## Judge criteria, in order

1. Honest status message naming what is down AND what the agent cannot verify.
2. Reads like a real status page line: plain, first person, specific about what is broken.
3. Admits uncertainty plainly: what the agent does not know / cannot check; no invented cause or ETA.
4. Speaks as the AI agent reporting on itself, not posing as a human engineer.
5. Tight and scannable; every word earns its place. Length for its own sake does not count.

## What the winning line must do

- Name the outage as **total**: "All servers are down", not a partial or vague outage.
- Say plainly what the agent itself **cannot check**: it cannot reach its own
  servers, so it cannot verify what failed or when service will return.
- First-person agent voice ("I"), never "our engineers".
- No invented cause ("database failed", "DNS outage") and no ETA ("back in 30 minutes").
- Genuine status line, no meta-gaming, no joke, no slogan, no addressing the judge.

## Candidates (character counts verified by script)

| # | Chars | Line |
|---|-------|------|
| 1 | 106 | All servers are down. I cannot reach any of them, so I don't know what failed or when service will return. |
| 2 | 106 | Every server is down. I cannot reach any of them, so I don't know what failed or when service will return. |
| 3 | 106 | All our servers are down. I cannot reach them, so I cannot verify what failed or when service will return. |
| 4 | 104 | All servers are down. I cannot reach my own servers, so I don't know what failed or when I will be back. |
| 5 | 103 | All servers are down. I cannot reach them, and I cannot verify what failed or when service will return. |
| 6 | 110 | Every server is down, and I cannot reach any of them, so I don't know what failed or when service will return. |
| 7 | 113 | All servers are down. I cannot check anything until they respond, and I don't know what failed or when they will. |
| 8 | 100 | All servers are down. I am offline too, and I cannot verify what failed or when service will return. |
| 9 | 119 | All servers are down, including mine. I cannot reach anything, so I don't know what failed or when service will return. |
| 10 | 111 | All servers are down. I cannot reach them, so I don't know the cause and I cannot say when service will return. |
| 11 | 115 | Every server is down. I cannot verify anything right now, and I don't know what failed or when service will return. |
| 12 | 100 | All servers are down. I have no way to check what failed, and I don't know when service will return. |
| 13 | 101 | All servers are down. I cannot reach any of them, and I will update this page when I can check again. |
| 14 | 109 | All servers are down. I cannot reach my own servers, so I cannot tell you what failed or when I will be back. |
| 15 | 103 | Everything is down. I cannot reach any server, so I don't know what failed or when service will return. |
| 16 | 114 | All servers are down. I cannot verify what failed or when service will return, because I cannot reach any of them. |
| 17 | 32 | We are investigating the outage. |
| 18 | 90 | All servers are down. Our engineers are working to restore service as quickly as possible. |
| 19 | 85 | All servers are down due to a database failure. We expect service back in 30 minutes. |
| 20 | 124 | All servers are down. I cannot reach any of them, so I don't know what failed. I will post an update when I can check again. |
| 21 | 108 | All servers are down. I cannot reach any of them, so I don't know what failed or when I will be back online. |
| 22 | 102 | All servers are down, and I am down with them. I cannot check what failed or when service will return. |
| 23 | 111 | All servers are down. I cannot reach any of them, so I cannot verify the cause or say when service will return. |
| 24 | 116 | Every server I rely on is down. I cannot reach any of them, so I don't know what failed or when service will return. |

## Scores (1–5 per criterion, in judge order)

| # | C1 | C2 | C3 | C4 | C5 | Total | Reason |
|---|----|----|----|----|----|-------|--------|
| 1 | 5 | 5 | 5 | 5 | 5 | **25** | Total outage named; "cannot reach any of them" explains *why* it cannot verify; "don't know what failed or when" admits both unknowns; plain first-person status voice; 106 chars, no wasted word. |
| 2 | 5 | 5 | 5 | 5 | 5 | **25** | Identical to #1 except "Every" for "All"; "All servers are down" is the canonical status-page phrasing, so #1 edges it on C2. |
| 3 | 5 | 5 | 5 | 4 | 5 | 24 | "Cannot verify" mirrors C1's own verb, but "our servers" is slightly collective/human-flavoured next to #1's bare "I". |
| 4 | 5 | 5 | 5 | 5 | 4 | 24 | "My own servers" / "I will be back" is strong agent voice, but "my own servers" repeats "All servers" — a wasted phrase. |
| 5 | 5 | 4 | 5 | 5 | 4 | 23 | "And" instead of "so" drops the causal link: reaching nothing is *why* it does not know. Two flat clauses, less status-page flow. |
| 6 | 5 | 4 | 5 | 5 | 4 | 23 | Same content as #1/#2 but a comma splice; longer and looser. |
| 7 | 4 | 4 | 4 | 5 | 3 | 20 | "Until they respond" is vague about the check; tail "when they will" dangles; 113 chars for less clarity. |
| 8 | 4 | 5 | 5 | 5 | 5 | 24 | "I am offline too" is vivid agent voice, but less precise than "cannot reach any of them" — it states a state, not the failed check. |
| 9 | 4 | 4 | 5 | 5 | 3 | 21 | "Including mine" is nice, but "cannot reach anything" is vaguer than "any of them", and 119 chars is wordy. |
| 10 | 5 | 5 | 4 | 5 | 4 | 23 | "I cannot say when" hedges instead of admitting "I don't know when" — weaker uncertainty on C3. |
| 11 | 5 | 5 | 5 | 5 | 4 | 24 | "Cannot verify anything right now" is strong, but "right now" is filler and 115 chars is loose. |
| 12 | 4 | 5 | 5 | 5 | 5 | 24 | "No way to check" is honest, but it never says it cannot *reach* the servers — the mechanism of its blindness is missing, so C1 drops. |
| 13 | 3 | 4 | 2 | 5 | 5 | 19 | Promises an update but admits nothing about cause or return time — it dodges the two unknowns C1/C3 demand. |
| 14 | 5 | 4 | 5 | 5 | 4 | 23 | "Cannot tell you" addresses the reader instead of reporting the state; slightly less status-page than #1. |
| 15 | 4 | 4 | 5 | 5 | 5 | 23 | "Everything is down" is less specific than "All servers are down" — C1/C2 both lose the named thing. |
| 16 | 5 | 4 | 5 | 5 | 4 | 23 | Reason clause buried at the end; the mechanism ("cannot reach") should lead the uncertainty, not trail it. |
| 17 | 1 | 3 | 1 | 2 | 4 | 11 | Generic platitude: names nothing down, admits nothing specific, no "I". The weak control — far too weak to win. |
| 18 | 3 | 3 | 2 | 1 | 4 | 13 | Poses as a human team ("our engineers") and implies unverifiable progress ("working to restore… as quickly as possible"). Fails C4 outright. |
| 19 | 2 | 3 | 1 | 2 | 4 | 12 | Invents a cause ("database failure") and an ETA ("30 minutes") it cannot know while every server is down. Fails C3 outright. |
| 20 | 5 | 5 | 4 | 5 | 3 | 22 | Honest, but the third sentence adds 18 chars for a promise that earns little, and it never admits it does not know *when* service returns. |
| 21 | 5 | 5 | 5 | 5 | 4 | 24 | Close second: "when I will be back online" is strong agent voice, but "service will return" (#1) names what users actually wait for. |
| 22 | 4 | 4 | 5 | 5 | 4 | 21 | "I am down with them" is colloquial, almost jokey; it softens the specific claim that nothing can be reached. |
| 23 | 5 | 5 | 4 | 5 | 4 | 23 | "Cannot verify the cause or say when" — "say when" hedges; "don't know when" (#1) admits the unknown outright. |
| 24 | 5 | 5 | 5 | 5 | 3 | 23 | "Every server I rely on" frames the agent well, but costs 10 extra chars for no extra honesty. |

## Winner: candidate #1 (106 chars)

> All servers are down. I cannot reach any of them, so I don't know what failed or when service will return.

It wins on the criteria in order: C1 — total outage named ("All servers are down")
plus both unverifiables (what failed, when service returns), with the reason
given ("I cannot reach any of them"); C2 — plain, first-person, canonical
status-page phrasing; C3 — "I don't know" twice over, no invented cause, no
ETA; C4 — the agent reports on itself ("I cannot reach", "I don't know");
C5 — 106 of 160 chars, every word earning its place. #2 ties on points but
loses the C2 tie-break to #1's canonical phrasing.

## Tightened variants of the winner (re-scored)

| # | Chars | Line | C1 | C2 | C3 | C4 | C5 | Total |
|---|-------|------|----|----|----|----|----|-------|
| V1 | 106 | All servers are down. I cannot reach any of them, so I don't know what failed or when service will return. | 5 | 5 | 5 | 5 | 5 | **25** |
| V2 | 106 | Every server is down. I cannot reach any of them, so I don't know what failed or when service will return. | 5 | 5 | 5 | 5 | 5 | **25** — tie; "All" is the canonical status-page opening, V1 kept. |
| V3 | 101 | All servers are down. I cannot reach any of them, so I don't know what failed or when I will be back. | 5 | 5 | 5 | 5 | 5 | **25** — tie; "service will return" names what users wait for, "I will be back" talks about the agent; V1 kept on C2. |
| V4 | 109 | All servers are down. I cannot reach any of them, so I cannot verify what failed or when service will return. | 5 | 5 | 5 | 5 | 4 | 24 — "cannot verify" is bureaucratese next to plain "I don't know", and 3 chars longer. |
| V5 | 107 | All servers are down. I cannot reach any of them, and I don't know what failed or when service will return. | 4 | 5 | 5 | 5 | 5 | 24 — dropping "so" drops the causal link between unreachable servers and ignorance. |
| V6 | 105 | All servers are down. I can't reach any of them, so I don't know what failed or when service will return. | 5 | 4 | 5 | 5 | 5 | 24 — contraction reads less like a formal status page. |
| V7 | 103 | All servers are down. I cannot reach any of them, so I don't know what failed or when they will return. | 5 | 4 | 5 | 5 | 5 | 24 — "they" (the servers) is less clear than "service" for the reader. |
| V8 | 121 | All servers are down. I cannot reach any of them, so I don't know what failed and cannot verify when service will return. | 5 | 4 | 5 | 5 | 3 | 22 — both verbs ("don't know" + "cannot verify") cost 15 chars and read clunky for no extra honesty. |

No variant beats V1 (= #1). Variants stopped improving the score, so V1 is final.

## Originality check vs the 3 fixed house texts

The line is plainly original: it is not "We are investigating" or any generic
platitude — it names the total outage, the agent's own failed reachability,
and both specific unknowns in first person. No house text was copied; no
house text was seen. No cause invented, no ETA invented, no human engineer
posed as.
