# Atreus Labs

> Google-login wallet with privacy-preserving payment links and programmable ZK rules on Stellar.
> No seed phrase. No identity leak. No double-claim. No proof sniping.

**Send money with rules only the right wallet can satisfy — without anyone learning who that wallet is.**

---

## Monorepo

All code now lives in a single monorepo at [github.com/atreus-lab/atreus](https://github.com/atreus-lab/atreus):

| Directory | Tech | Purpose |
|-----------|------|---------|
| \`frontend/\` | Next.js 15 | Wallet UI, link create/claim |
| \`backend/\` | Express + TS | Link management API, tx relay |
| \`contracts/\` | Rust (Soroban) | Escrow + ZK verifier contracts |
| \`docs/\` | Markdown | Vision, architecture, design |

## Features

- **Sign in with Google** — derive a Stellar wallet instantly, no seed phrase
- **ZK payment links** — attach rules like \"only wallets holding >50 XLM can claim\"
- **Zero-knowledge proofs** — recipient proves eligibility without revealing balance
- **Auto-swaps** via Soroswap on deposit
- **Passkey (WebAuthn)** — hardware-grade transaction security

---

*Bringing link-as-wallet to Stellar with ZK privacy.*