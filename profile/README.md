# Knightsbridge AIQ

**Post-quantum cryptography for finance and blockchain — shipped as the KXCO stack.**

We build production-grade, standards-based cryptography that stays secure against both classical and quantum adversaries. Every primitive is [NIST](https://csrc.nist.gov/)-standardized and built on an independently audited foundation. **No custom cryptography.**

**This is the open-source cryptography layer underneath the KXCO platform** — [Nexus](https://kxco.ai/nexus) (identity, legal execution & proof), [Meridian](https://kxco.ai/meridian) (private-capital deal network), [Treasury](https://kxco.ai/treasury), [Sentinel](https://kxco.ai/sentinel) (the quantum-resistant cloud), [KnightsPurse](https://purse.kxco.ai), KnightsVault, and the [Armature L1](https://chain.kxco.ai) settlement network. Audit it before you trust it.

[Website](https://kxco.ai) · [Verify a signature](https://verify.kxco.ai) · [npm](https://www.npmjs.com/package/kxco-pq)

---

## The KXCO post-quantum stack

One meta-package installs everything; each capability is also available à la carte.

```sh
npm install kxco-pq
```

| Package | What it does |
|---|---|
| [`kxco-pq`](https://github.com/KnightsbridgeAIQ/kxco-pq) | The complete stack in one install — identity, HSM, audit, attestation, encrypted channels, file encryption, webhook signing |
| [`kxco-post-quantum`](https://github.com/KnightsbridgeAIQ/kxco-post-quantum) | Core primitives — ML-DSA-65 signatures + ML-KEM-768 key encapsulation. Every other package builds on this |
| [`kxco-pq-sdk`](https://github.com/KnightsbridgeAIQ/kxco-pq-sdk) | Hierarchical identity credentials (institution → user), KYC-gated issuance, audited signing |
| [`kxco-pq-vault`](https://github.com/KnightsbridgeAIQ/kxco-pq-vault) | ML-KEM-768 envelope encryption for files and payloads |
| [`kxco-pq-tls`](https://github.com/KnightsbridgeAIQ/kxco-pq-tls) | Hybrid ML-KEM-768 + X25519 encrypted streams and WebSockets |
| [`kxco-post-quantum-webhook`](https://github.com/KnightsbridgeAIQ/kxco-pq-webhook) | Dual-signed webhooks — HMAC-SHA-256 + ML-DSA-65. Express, Fastify, Hono, Workers, Vercel |
| [`kxco-pq-cli`](https://github.com/KnightsbridgeAIQ/kxco-pq-cli) | Keygen, fingerprinting, and signed key-rotation manifests |
| [`kxco-verify`](https://github.com/KnightsbridgeAIQ/kxco-verify) | Independent, browser-safe verifier for signed deploy attestations |

*(Also published: `kxco-pq-hsm`, `kxco-pq-audit`, `kxco-pq-attest`, `kxco-pq-chain`, and multi-language [verifiers](https://github.com/KnightsbridgeAIQ/kxco-pq-verifiers) in Go, Python, and Rust.)*

---

## Standards & assurance

- **[NIST FIPS 204](https://csrc.nist.gov/pubs/fips/204/final)** — ML-DSA-65 digital signatures
- **[NIST FIPS 203](https://csrc.nist.gov/pubs/fips/203/final)** — ML-KEM-768 key encapsulation
- Built on **[`@noble/post-quantum`](https://github.com/paulmillr/noble-post-quantum)** — audited by Cure53 (2024)
- Packages publish to npm with **build provenance** and Apache-2.0 licensing
- [Armature L1 white paper](https://chain.kxco.ai/whitepaper) · [developer docs](https://chain.kxco.ai/docs) · [network explorer](https://chain.kxco.ai)

**Company:** Knightsbridge Financial Ltd (UK Company No. 15684975) · LEI 213800TMP5DQFDKOZ549 · ICO registered (C1961692)
**Compliance:** NIST FIPS 203/204/205 · UK eIDAS Advanced e-Signature · NIST ACVTS validation active · NSA CNSA 2.0 (Armature L1)
**Memberships:** PKI Consortium · CSA Quantum-Safe Security Working Group

---

## Security

Found a vulnerability? Please report it privately through the affected repository's **Security → Report a vulnerability** tab. Do not open public issues for security reports.

---

<sub>© Knightsbridge AIQ. Building quantum-safe cryptography for finance & blockchain.</sub>
