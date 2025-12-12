# Pink MythOS

> **"The galaxy is watching. Don't be boring. Your survival depends on the Ratings."**

An interdimensional reality show broadcast where humanity auditions for the right to exist. Built on **Solana**.

---

## From the Creator

This repo is my commitment to **radical transparency**. Everything that matters — the smart contracts, the economics, the self-audits, the architecture docs — lives here. Not behind closed doors.

If you're an investor, a player, or someone who just wants to understand how this thing actually works: **everything is here for you to read, verify, and scrutinize.**

---

## What's In This Repository

| Path | Purpose |
|------|---------|
| `/contracts` | Solana smart contracts (Rust/Anchor) — **self-custodial, auditable** |
| `/docs` | Architecture, specs, and design documents |
| `apex_curve_economics.md` | Economics breakdown — the math behind winner selection |

---

## Economics (Transparent, On-Chain)

Every pool follows the **70/7/15/8 Renewal Protocol**:

| Split | Destination |
|------:|:------------|
| **70%** | Winners (paid out on-chain) |
| **7%** | Treasury (syndication) |
| **15%** | Renewal Vault (burn schedule) |
| **8%** | Next session buffer |

### The Apex Curve (Power Law Winner Selection)

```
winnerPct = initial / (1 + (N / pivot)^k)
winners = max(3, floor(N × winnerPct))
```

| Players | Winners | Avg ROI |
|--------:|--------:|--------:|
| 100 | 21 | 3.3x |
| 1,000 | 30 | 23x |
| 5,000 | 13 | 269x |
| 10,000 | 8 | 875x |
| 100,000 | 3 | 23,333x |

---

## Self-Audit Commitment

- **Smart contracts** will be open-sourced before mainnet
- **All economics formulas** are documented and verifiable
- **Prize distribution** is deterministic and on-chain
- **No hidden admin keys** that can drain funds

---

## Key Technical Choices

- **Chain**: Solana (low fees, fast finalization)
- **Contract Pattern**: Anchor framework (Rust)
- **Frontend**: React + TypeScript
- **AI Stack**: Narrative generation for "Cognitive Breach" scenarios

---

 **Contract Address**: *Coming Soon (Testnet)*

---

## License

MIT — Build on this, learn from it, challenge it.

---

*Last updated: 2025-12-12*
