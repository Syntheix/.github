<div align="center">
  <h1>Syntheix Cloud</h1>
  <h3>Thailand's sovereign developer cloud · คลาวด์ของไทย</h3>
  <p>
    <a href="https://syntheix.cloud">syntheix.cloud</a> ·
    <a href="https://syntheix.cloud/docs/quickstart">Quickstart</a> ·
    <a href="https://syntheix.cloud/changelog">Changelog</a> ·
    <a href="https://syntheix.cloud/status">Status</a>
  </p>
</div>

---

> **Build on Thailand-domiciled cloud infrastructure.** PDPA-aligned, baht-denominated billing, the same primitives you already know from AWS — with TH latency and a real human at the other end of the line.

## What ships today (alpha)

| Surface | Live at | Source |
|---|---|---|
| 🌐 Marketing + docs | [syntheix.cloud](https://syntheix.cloud) | [Syntheix/www](https://github.com/Syntheix/www) |
| 🔐 Identity (SSO via Keycloak) | [auth.syntheix.cloud](https://auth.syntheix.cloud) | (Keycloak realm) |
| ⚙ Control-plane API (Bun + Hono + Drizzle) | [api.syntheix.cloud](https://api.syntheix.cloud) | [Syntheix/api](https://github.com/Syntheix/api) |
| 🖥 Admin console (Next.js 16) | [console.syntheix.cloud](https://console.syntheix.cloud) | [Syntheix/console](https://github.com/Syntheix/console) |
| 📦 Object Storage (S3-compatible) | [s3.syntheix.cloud](https://s3.syntheix.cloud) | (MinIO + control-plane routes) |
| 🛠 `syx` CLI (Go, multi-platform) | one binary, every service | [Syntheix/cli](https://github.com/Syntheix/cli) |
| 📊 Live agent observability | localhost:4242 (dev tool) | [Syntheix/board](https://github.com/Syntheix/board) |

## Engineering principles

1. **Thai sovereignty by default.** Every byte of customer data lives on hardware in Thailand. PDPA isn't a checkbox — it's the architecture.
2. **Same primitives, different gravity.** S3-compatible buckets, Postgres, VMs (Q3), K8s (Q4) — APIs you already know, hosted next door.
3. **Boring stack, fast iteration.** Bun + Hono + Drizzle + Postgres + Keycloak + Cloudflare Tunnel + MinIO. No exotic infra; production-grade plumbing.
4. **Heterogeneous fleet from day one.** Every container image is multi-arch (linux/amd64 + linux/arm64). The substrate runs on a rack server today and is built to absorb PCs, ARM SBCs, and Apple Silicon Macs as workers.
5. **Build in public.** Every release lands in [the changelog](https://syntheix.cloud/changelog) the day it ships. No press releases, no bait, no fake uptime numbers.

## Roadmap

- **Q2 2026** (now) — Foundation: control plane, IAM, Object Storage, console, CLI ✅ · Stripe + e-Tax billing 🚧 · Terraform provider 🚧 · alpha launch with 5 friendly customers 🚧
- **Q3 2026** — Compute (VMs · libvirt + cloud-init) · OVN networking · Managed Postgres · DNS-as-a-service · public beta · 30 customers · ฿80k MRR
- **Q4 2026** — Managed Kubernetes · observability (Mimir + Loki + Tempo) · BaaS Postgres · Saraburi DR site · GA · 80 customers · ฿320k MRR
- **Q1 2027** — ISO 27001 · PDPA compliance pack · ก.ล.ต. cyber resilience · first ฿1M+ enterprise contract
- **Q2 2027** — Functions · Edge CDN · SNS/SQS-equivalent · 300+ customers · ฿2.5M MRR · breakeven

[Full roadmap →](https://syntheix.cloud/#roadmap)

## Contributing

We're a small team (one engineer) right now, but we welcome PRs to any of the open repos. The CLI ([Syntheix/cli](https://github.com/Syntheix/cli)) is the lowest-friction entry point — small UX tweaks ship fast.

## Contact

- General inquiries · [hi@syntheix.cloud](mailto:hi@syntheix.cloud)
- Security disclosures · [security@syntheix.cloud](mailto:security@syntheix.cloud) (PGP at `/.well-known/pgp.asc`)
- Waitlist for alpha access · [syntheix.cloud](https://syntheix.cloud) (footer form)

<sub>Built in 🇹🇭 · Apache 2.0 where applicable · See individual repos for licensing details</sub>
