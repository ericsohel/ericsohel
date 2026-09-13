# hey, i'm eric 👋

**cs & applied math @ stony brook ('27) · new york city · [ericsohel.com](https://ericsohel.com)**

```console
eric@nyc:~$ whoami
backend · market data · multi-agent ai · security tooling

```

my site streams a live kalshi order book, runs a ticker of what i'm actually
listening to, prices 1,500+ ballplayers on demand, and has a working terminal —
[go type `help`](https://ericsohel.com).

---

## the desk right now

**📼 [Kalshi Tape](https://github.com/ericsohel/KalshiTradingProject)** — an
order-book flight recorder for Kalshi, which exposes no historical depth. Raw
WebSocket frames from 200 markets land on an append-only zstd tape before any
parser runs, and every price and count is a fixed-point integer — floats never
touch money. The exchange client signs with RSA-PSS and mirrors Kalshi's
token-bucket rate limits client-side; a ZeroMQ bus feeds a Starlette API and a
React + WebGL2 viewer drawing a live liquidity heatmap, deployed on Azure behind
Caddy — [watch it live](https://kalshi-tape-live.northcentralus.cloudapp.azure.com).
Measured over three days of tape: 220M records baked to Parquet with no gaps,
**99.95%** of rebuilt books match the next keyframe, and 99.3% of REST snapshot
audits pass; 771 Python tests at 96% branch coverage. Next up: deterministic
replay, a calibrated simulator, and a market maker on the same engine.

**🤖 multi-agent systems @ Capital One** — two summers, NYC + McLean.
Most recently: a multi-agent system (Python, LangGraph, FastAPI) that
automates creating financial reports — NL-to-SQL retrieval across 2K tables,
analysis, and an orchestrator rendering charts, tables, and commentary
revisable via chat, with strict output validation that diagnoses each failure
and applies a tailored fix. Cut generation time 75% with parallel LLM calls and
cost with Redis caching; adopted by 20 Finance Tech teams at a 95% satisfaction
rate. The summer before: built the React UI and the wire-execution logic
(idempotency keys — each wire executes exactly once) for a wire platform
facilitating 5K+ daily payments worth ~$1B, plus a PostgreSQL-backed state
machine coordinating checks across 4 verification services.

**⚾ [DraftIQ](https://github.com/ericsohel/draftiq)** — a market
maker for fantasy baseball auctions. Production REST API pricing every
draftable MLB player with a z-score-above-replacement engine: live draft-state
re-valuation, positional scarcity, ranked nominations, budget allocation.
Self-serve developer portal (scrypt hashing, signed-cookie sessions, CIDR
whitelisting, sliding-window rate limits), 131 Jest/supertest tests, an
OpenAPI spec enforced by a CI drift-guard, and a public
[live demo endpoint](https://draftiq-xkpx.onrender.com/api/v1/demo/valuations)
that powers the widget on my site.

**🔍 Pysa @ Meta (MLH Fellowship)** — built a fuzzer that generated 10,000+
Python programs with known source→sink taint flows, uncovering 30+ flows
missed by Meta's open-source security analyzer
([pyre-check#886](https://github.com/facebook/pyre-check/pull/886)); also
added a live timer and performance metrics to Pysa's terminal output.
The fuzzer landed upstream as
[`scripts/pysa_fuzzer`](https://github.com/facebook/pyre-check/tree/main/scripts/pysa_fuzzer)
(commit [`99a07a24`](https://github.com/facebook/pyre-check/commit/99a07a24),
authored under my old handle esohel30) and has since been extended by Meta's
Pysa team.

**🖥️ [ericsohel.com](https://ericsohel.com)** — hand-rolled HTML/CSS/JS, no
frameworks, no templates. Interactive terminal, a live Kalshi heatmap pulled
from the recorder's own API, a $ERIC market you can trade, a ticker tape fed by
the Spotify API through a serverless function, my life drawn as a subway line,
and a bookshelf organized like a trading book.

## receipts

🏆 Citadel Terminal AI Competition — **2nd place** · Cornell Trading Competition — **top 5 (×2)** ·
USACO — **Silver** · AIME Qualifier (×3) · Stanford Code in Place — section leader → invited back as Head TA

## stack i actually use

`python` · `asyncio` · `fastapi / starlette` · `langgraph` · `typescript / react` ·
`node` · `sql / postgres` · `redis` · `zeromq` · `docker` · `aws` · `azure` · `github actions`

## reach me

📬 ericsohel05@gmail.com · [linkedin](https://www.linkedin.com/in/eric-sohel/) —
or open [the site terminal](https://ericsohel.com) and type `contact`.
