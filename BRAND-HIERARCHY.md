# Goldspire Ventures — brand hierarchy

**Status:** Canonical (founder decisions locked June 2026)  
**Legal entity:** Goldspire Ventures Ltd · United Kingdom

---

## Structure (Option A)

Goldspire Ventures Ltd is the **parent holding company**. All portfolio products and the services division operate under this umbrella.

```text
Goldspire Ventures Ltd  (goldspireventures.com)
│
├── Products (consumer / B2B SaaS)
│   ├── Livia          livia-hq.com          [live]
│   ├── Veil           join-veil.goldspireventures.com  [live]
│   ├── Mulah          [building]
│   ├── S.I.M.I.       [building]
│   ├── Triforge       Groundline · Vouchline · Stillpath  [building]
│   ├── Valrolly       → future Livia events vertical  [building]
│   ├── TrustBase      [building]
│   ├── MOVE / EZFlow  [building]
│   └── Japa           [building]
│
└── Divisions
    └── Goldspire Studio   goldspire.dev   [live]
        Product design & engineering for external clients.
        Operates as a division of Goldspire Ventures Ltd.
```

---

## Domains

| Surface | Domain | Owner |
|---------|--------|-------|
| Corporate / portfolio | `goldspireventures.com` | Ventures Ltd |
| Studio marketing | `goldspire.dev` | Studio division |
| Studio ops (internal) | `goldspire.studio` | Studio division |
| Livia product | `livia-hq.com` | Livia |
| Veil portal | `join-veil.goldspireventures.com` | Veil |
| Veil API | `veil-api.goldspireventures.com` | Veil |

---

## Email

| Address | Use |
|---------|-----|
| `support@goldspireventures.com` | Corporate, portfolio, product support default |
| `security@goldspireventures.com` | Veil security reports |
| `privacy@goldspireventures.com` | Privacy requests (products) |
| `hello@goldspire.dev` | Studio sales & project enquiries |
| `ops@goldspire.studio` | Internal studio operations |

Studio client contracts and footers should read: **Goldspire Studio, a division of Goldspire Ventures Ltd.**

---

## GitHub organisation

**Active org:** [github.com/goldspireventures](https://github.com/goldspireventures)

All portfolio repositories live under this org. See `REPO-REGISTRY.yaml` for the full map.

---

## Code registries (keep in sync)

| Registry | Location | Purpose |
|----------|----------|---------|
| **Public portfolio** | `goldspire-corporate/src/data/portfolio.ts` | Marketing site company pages |
| **Repo map** | `docs/REPO-REGISTRY.yaml` | Local path ↔ GitHub repo ↔ product |
| **Studio brand** | `launch-stack/packages/config/src/brand.ts` | Studio apps & packages |
| **Studio marketing** | `launch-stack/packages/commercial/src/marketing-site-narrative.ts` | goldspire.dev copy + legal |
| **Per-product legal** | e.g. `livia/.../company.ts`, `veil/.../product.js` | Product footers |

---

## Valrolly → Livia

Valrolly remains a portfolio company while events infrastructure matures. The intended end state is absorption into **Livia's events vertical** — not a separate long-term brand. Track convergence in both repos before public messaging commits to either path.

---

## Triforge

Triforge (Groundline, Vouchline, Stillpath) is a **Ventures portfolio company**, not a separate holding brand. Product marketing may use the Triforge trust mark; legal and corporate surfaces roll up to Goldspire Ventures Ltd.
