# hey, i'm eric 👋

**cs & applied math @ stony brook ('27) · new york city · [ericsohel.com](https://ericsohel.com)**

```console
eric@nyc:~$ whoami
distributed systems · backend · multi-agent ai · security tooling

```

my site runs a live ticker of what i'm actually listening to, prices 1,600+
ballplayers on demand, and has a working terminal — [go type `help`](https://ericsohel.com).

---

## the desk right now

**🤖 multi-agent systems @ Capital One** — two summers, NYC + McLean.
Most recently: a multi-agent system (Python, LangGraph, FastAPI) that
automates creating financial reports — NL-to-SQL retrieval across 2K tables,
analysis, and an orchestrator rendering charts and commentary revisable via
chat. Cut generation time 75% with parallel LLM calls + Redis; adopted by 20
Finance Tech teams at a 95% satisfaction rate. The summer before: built the
React UI and the wire-execution logic (idempotency keys — each wire executes
exactly once) for a wire platform facilitating 5K+ daily payments worth ~$1B.

**⚾ [DraftIQ](https://github.com/ericsohel/draftiq)** — a market
maker for fantasy baseball auctions. Production REST API pricing every
draftable MLB player with a z-score-above-replacement engine: live draft-state
re-valuation, positional scarcity, ranked nominations, budget allocation.
Self-serve developer portal (scrypt hashing, signed-cookie sessions, CIDR
whitelisting, sliding-window rate limits), 125 Jest/supertest tests, an
OpenAPI spec enforced by a CI drift-guard, and a public
[live demo endpoint](https://draftiq-xkpx.onrender.com/api/v1/demo/valuations)
that powers the widget on my site.

**📈 [orderbook](https://github.com/ericsohel/orderbook)** — a C++17 limit
order book and matching engine with price-time priority, benchmarked at
**3.7M ops/s (269 ns mean per op)** on a seeded mixed workload; a JavaScript
twin held to the same 12-case test list runs as a live market on
[my site](https://ericsohel.com) — go trade $ERIC.

**🔍 Pysa @ Meta (MLH Fellowship)** — built a fuzzer that generated 10,000+
Python programs with known source→sink taint flows, uncovering 30+ flows
missed by Meta's open-source security analyzer
([pyre-check#886](https://github.com/facebook/pyre-check/pull/886)); also
added a live timer and performance metrics to Pysa's terminal output.
My merged PRs live under my old handle →
[the receipts](https://github.com/facebook/pyre-check/pulls?q=esohel30+).

**🖥️ [ericsohel.com](https://ericsohel.com)** — hand-rolled HTML/CSS/JS, no
frameworks, no templates. Interactive terminal, a ticker tape fed by the
Spotify API through a serverless function, my life drawn as a subway line,
and a bookshelf organized like a trading book.

## receipts

🏆 Citadel Terminal — **2nd place** · Cornell Trading Competition — **top 5 (×2)** ·
AIME Qualifier (×2) · Stanford Code in Place — section leader → invited back as Head TA

## stack i actually use

`python` · `typescript / node` · `java` · `ocaml` · `sql / postgres` · `redis` ·
`aws (lambda, ec2)` · `docker` · `github actions` · `langgraph` · `pytorch`

## reach me

📬 ericsohel05@gmail.com · [linkedin](https://www.linkedin.com/in/eric-sohel/) —
or open [the site terminal](https://ericsohel.com) and type `contact`.
