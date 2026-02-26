# slackmgr

**Making your Slack channels slightly less chaotic since 2024.**

We build open-source Go libraries for routing, grouping, and managing alerts in Slack — so your on-call engineer gets one coherent thread instead of 47 identical pings at 3am. Correlation IDs, severity-based ordering, emoji-driven triage, auto-resolution, escalation ladders, actionable webhook buttons — it's all in there. The [core README](https://github.com/slackmgr/core#readme) has the full breakdown.

---

## What's in the box

| Repo | What it does |
|------|-------------|
| [core](https://github.com/slackmgr/core) | The brains — REST API + alert manager as embeddable Go libraries |
| [go-client](https://github.com/slackmgr/go-client) | Send alerts to a running instance. One import, done. |
| [plugins](https://github.com/slackmgr/plugins) | AWS SQS, DynamoDB, Postgres, GCP Pub/Sub — pick your flavour |
| [types](https://github.com/slackmgr/types) | Shared interfaces. Small, boring, essential. |
| [examples](https://github.com/slackmgr/examples) | Minimal and flexible host apps — copy, tweak, ship. |

## Philosophy

- **Library, not platform.** You own the `main.go`. We stay out of your way.
- **Bring your own infra.** Redis Streams, SQS, Pub/Sub — it all works.
- **Boring concurrency.** errgroup, channels, mutexes. No magic.

---

Built with Go. Tested with `-race`. Deployed by people who've been paged one too many times.
