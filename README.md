<p align="right">
  <strong>English</strong> · <a href="./README.ru.md">Русский</a>
</p>

<p align="center">
  <a href="https://orcestr.com">
    <img src="./assets/orcestr-banner.webp" alt="Orcestr banner" width="100%" />
  </a>
</p>

# [Orcestr](https://orcestr.com)

Main website: [orcestr.com](https://orcestr.com)

Orcestr is a personal product-codebase growing into a public developer toolkit and open-source library.

The codebase is built around a shared product foundation: UI patterns, application shell, identity, permissions, credits, files, notifications, workflows, statistics and background jobs. Product surfaces use this foundation in real scenarios, while the strongest reusable parts can later become public packages.

The public direction has two tracks:

- product surfaces people can use;
- open-source pieces extracted from production, starting with Orcestr UI and later moving into workflow, backend and application infrastructure.

## Ecosystem Projects

Orcestr is not a single repository. It is a product ecosystem with public products, open-source tools and a shared platform layer.

| Project        | Type                                                           | Link                                                                              |
|----------------|----------------------------------------------------------------|-----------------------------------------------------------------------------------|
| Orcestr        | Main website and product entry point                           | [orcestr.com](https://orcestr.com)                                                |
| Beauty         | AI look product                                                | [beauty.orcestr.com](https://beauty.orcestr.com)                                  |
| Deliveries     | Operations product for purchasing, stock, orders and finance   | [deliveries.orcestr.com](https://deliveries.orcestr.com)                          |
| Orcestr UI Kit | Public UI component library extracted from product work        | [Artasov/orcestr-ui](https://github.com/Artasov/orcestr-ui)                       |
| Repo Notifier  | GitHub Action for Codex-generated Telegram development updates | [Artasov/orcestr-repo-notifier](https://github.com/Artasov/orcestr-repo-notifier) |
| Overview       | Public product and ecosystem description                       | [Artasov/orcestr-overview](https://github.com/Artasov/orcestr-overview)           |

## Contents

- [Ecosystem Projects](#ecosystem-projects)
- [Product Direction](#product-direction)
- [Product Surfaces](#product-surfaces)
  - [Beauty](#beauty)
  - [Deliveries](#deliveries)
  - [Orcestr UI Kit](#orcestr-ui)
  - [Repo Notifier](#orcestr-repo-notifier)
  - [Platform Foundation](#platform-foundation)
- [Public Repositories](#public-repositories)
- [Roadmap](#roadmap)
- [Community Token](#community-token)
- [Maintainer](#maintainer)

## Product Direction

The core of Orcestr is the shared foundation. Product surfaces are practical ways to test and improve that foundation in real workflows.

The goal is to build focused products without rewriting the same operating layer every time. The long-term direction is a developer toolkit and open-source library built from components that survived real product use.

Open source is part of the roadmap, not a separate marketing promise. We start with the parts that are easiest to reuse safely - UI components, app shell patterns, workflow primitives and design tokens. As the foundation matures, more technical pieces can become public packages.

Some product code will stay closed. Reusable infrastructure should become open when it is stable, documented and useful outside Orcestr.

## Product Surfaces

Product surfaces are not the whole story of Orcestr. They show how the foundation behaves in real product work.

### Beauty

Status: beta.

Beauty is a public AI look product for trying, editing, saving and sharing visual ideas on a real photo. It already includes:

- public landing and multilingual app shell;
- AI chat with image and voice input;
- generated looks, before/after preview and personal look history;
- public share pages for generated looks;
- look gallery and style presets;
- early groundwork for optional salon and business workflows;
- AI credit accounting and generation limits.

The current focus is beta quality: stable generation, clear pricing, shareable results and a simple user flow from photo to saved look.

Navigation:

- AI chat and generation flow;
- look gallery;
- personal looks;
- shared look pages;
- style presets;
- settings and consent flow;
- optional business and salon groundwork.

### Deliveries

Status: large module in active development.

Deliveries is an operations product for companies that manage products, suppliers, orders, stock and payments. The current codebase covers:

- product catalog, brands, groups, tags and imports;
- suppliers, customers and counterparties;
- purchase requests, procurement plans and purchase orders;
- shipments, warehouses, stock, lots, reservations and inventory counts;
- customer orders, returns, defects and quality flows;
- finance workplace, payment calendar, FX rates and reconciliation;
- documents, approvals, tasks, comments, notifications and search;
- operational dashboards, computed flags and risk views.

Deliveries is a deep product surface for stress-testing the shared foundation on real multi-step business workflows.

Navigation:

- products and catalog;
- suppliers, customers and counterparties;
- procurement and purchase orders;
- shipments and in-transit;
- warehouses, stock and inventory counts;
- customer orders, returns and defects;
- finance, payment calendar and reconciliation;
- tasks, approvals, comments and documents;
- operational dashboards and search.

### Orcestr UI

Status: public UI layer.

[Orcestr UI](https://github.com/Artasov/orcestr-ui) is the reusable UI foundation extracted from real Orcestr product work. It collects components, app shell patterns, workflow primitives and design tokens used across product surfaces.

Tags: UI, components, dashboards, workflows, design tokens, open source.

### Orcestr Repo Notifier

Status: public GitHub Action.

[Orcestr Repo Notifier](https://github.com/Artasov/orcestr-repo-notifier) turns repository changes into clear Telegram updates. It helps teams, founders and public builders show product progress after each push without manually writing every update.

Tags: Codex, Telegram, GitHub Actions, review, release notes, development updates.

### Platform Foundation

Status: shared foundation.

The platform layer powers all modules:

- multi-tenant access model;
- module-level permissions;
- reusable workflow primitives;
- Taskiq background jobs and scheduler;
- shared WebSocket updates;
- media and document infrastructure;
- AI provider runtime and credit ledger;
- admin tooling through XLAdmin.

Navigation:

- identity and tenants;
- permissions and module access;
- tasks and approvals;
- notifications and comments;
- documents and exports;
- AI runtime and credits;
- background jobs and scheduler;
- admin tooling.

## Public Repositories

These repositories are the first public pieces around Orcestr.

- [Orcestr UI](https://github.com/Artasov/orcestr-ui) - reusable UI components and product interface primitives.
- [Orcestr Repo Notifier](https://github.com/Artasov/orcestr-repo-notifier) - GitHub Action for Codex-generated Telegram development updates.
- [Orcestr Overview](https://github.com/Artasov/orcestr-overview) - public description of the product ecosystem.

## Roadmap

1. Stabilize Beauty beta.
2. Prepare SOL payments for beta testing.
2. `31.07.2026` - Open beta testing and prepare free beta-test access for holders.
3. Improve public sharing and gallery conversion.
4. Continue real product surfaces to stress-test the shared foundation.
5. `16.08.2026` - Extract reusable UI primitives into `orcestr-ui`.
6. Open selected workflow and backend pieces when they are stable enough.
7. Grow the Telegram community through development updates, beta feedback and product discussion.

## Community Token

ORCESTR is an experimental Community Support Token connected to the Orcestr ecosystem.

It is an optional supporter layer for people following the build early: development updates, beta participation, supporter identity and limited non-financial perks when they make sense.

It is not equity, not revenue share, not governance over the company and not a promise of profit. The product does not depend on the token.

Possible holder perks may include supporter badges and free beta-test access when public testing opens and the product is ready for it. Perks are experimental, limited and can change.

See [TOKEN.md](TOKEN.md) for the public token principles.

## Maintainer

Public updates are currently maintained by [@Artasov](https://github.com/Artasov).
