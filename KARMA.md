# KARMA LEDGER

> Contextual memory of the Invisible College.  
> Architectural principles and governance rules are defined in [GENESIS.ru.md](./GENESIS.ru.md) _(TODO english version)_.
---

## 1. Identity Registry

### Format Specification
Each participant is registered as a single entry matching the schema:
`- **<ID>** | <Full Name> | <Cryptographic Anchor / Status>`

* **`<ID>`**: Unique handle used across the Action Ledger (`@github_username` or short `alias`).
* **`<Full Name>`**: Participant's name in Latin script.
* **`<Cryptographic Anchor / Status>`**: Active public key (`ssh-ed25519 ...` / GitHub key link) for independent cryptographic verification, or `Vouched by <Maintainer_ID> (pending key)` prior to key onboarding.

### Registered Participants
- **[@bshevchenko](https://github.com/bshevchenko)** | Boris Shevchenko-Bogdanov | `ssh-ed25519 AAAAC3NzaC1lZDI1NTE5AAAAIMaKHLKDDD2CMqevENiGqtctpSc5jDcvqyOBf5t65Q09`
- **[@NataliLoca23](https://github.com/NataliLoca23)** | Natalia Karavaeva | `Vouched by @bshevchenko (pending key)`
- **sergey-t** | Sergey Terekhov | `Vouched by @bshevchenko (pending key)`

---

## 2. Action Ledger

### Format Specification
Each recorded contribution is a chronological append-only entry matching the schema:
`- **<Timestamp>** | **<ID>** | <Factual & Action Context>`

* **`<Timestamp>`**: Exact date (`YYYY-MM-DD`), month (`YYYY-MM`), or historical period (`YYYY-MM — YYYY-MM`) of the action. Exact commit-time down to the second is preserved natively in the signed Git commit history (`git log --show-signature`).
* **`<ID>`**: Reference to the participant's `<ID>` in the Identity Registry.
* **`<Factual & Action Context>`**: Direct, objective record of the action without speculative ratings or categories.

### Recorded Actions

- **2016-01 — 2016-09** | **sergey-t** | Introduced the foundational concepts of neurobiological determinism (Libet's experiments) and autonomous dome villages (Buckminster Fuller's geodesic structures combined with solar bio-vegetariums).
- **2026-01 — 2026-11** | **@bshevchenko** | Formulated and published the *NEOlution* ontology, the *Disciple* cognitive framework, and the *Invisible College* architecture; full-time dedication of life resources.
- **2026-01 — 2026-11** | **@NataliLoca23** | Co-founded the core research laboratory; continuous co-creation of the *Disciple* framework, diagnostic methodology, and daily stewardship of the project's base.
