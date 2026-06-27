<p align="right">
  <img src="./assets/orcestr-logo.png" alt="Orcestr logo" width="42" height="42" align="left" />
  <strong>English</strong> · <a href="./README.ru.md">Русский</a>
</p>

# Orcestr

Orcestr is a personal product-codebase growing into a public developer toolkit and open-source library.

The codebase is built around a shared product foundation: UI patterns, application shell, identity, permissions, credits, files, notifications, workflows, statistics and background jobs. Product surfaces use this foundation in real scenarios, while the strongest reusable parts can later become public packages.

The public direction has two tracks:

- product surfaces people can use;
- open-source pieces extracted from production, starting with Orcestr UI and later moving into workflow, backend and application infrastructure.

## Contents

- [Product Direction](#product-direction)
- [Product Surfaces](#product-surfaces)
  - [Beauty](#beauty)
  - [Deliveries](#deliveries)
  - [Platform Foundation](#platform-foundation)
  - [Open Source: Orcestr UI](#open-source-orcestr-ui)
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

### Open Source: Orcestr UI

Planned public developer work starts with UI:

- `orcestr-ui` component library;
- app shell patterns for operational dashboards;
- modal, table, filter and workflow primitives;
- design tokens extracted from production modules;
- examples from product surfaces where they can be safely public.

The UI library should be useful on its own. It is the first step toward a broader open-source layer built from real product work.

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
