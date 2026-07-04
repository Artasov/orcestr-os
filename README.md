<p align="right">
  <strong>English</strong> · <a href="./README.ru.md">Русский</a>
</p>

<p align="center">
  <a href="https://orcestr.com">
    <img src="./assets/orcestr-banner.webp" alt="Orcestr banner" width="100%" />
  </a>
</p>

# [Orcestr](https://orcestr.com) is open-source

Main website: [orcestr.com](https://orcestr.com)

Orcestr is an ecosystem with open-source libraries, a developer toolkit, applied tools and real products.

The public direction has three parts:

- Open-source **lib**s.
- Open-source **tool**s.
- Web **product**s.

## Ecosystem Projects

| Project | Type | Status | Link |
| --- | --- | --- | --- |
| Orcestr Auth | Shared authentication layer for React, Next.js and FastAPI services | ![Planned](https://img.shields.io/badge/-Planned-8b5cf6) | Planned: `orcestr-auth`, `orcestr-fastapi-auth`, `orcestr-next-auth` |
| Orcestr UI | Public UI library extracted from product development | ![Dev](https://img.shields.io/badge/-Dev-f59e0b) | [Artasov/orcestr-ui](https://github.com/Artasov/orcestr-ui) |
| Orcestr Icons | Package of different icon styles as an add-on to Orcestr UI | ![Planned](https://img.shields.io/badge/-Planned-8b5cf6) | Planned |
| Orcestr Repo Notifier | GitHub Action for Codex-generated Telegram development updates | ![Released](https://img.shields.io/badge/-Released-2ea44f) | [Artasov/orcestr-repo-notifier](https://github.com/Artasov/orcestr-repo-notifier) |
| Orcestr Media Transcriber | Repository for media transcription | ![Dev](https://img.shields.io/badge/-Dev-f59e0b) | [Artasov/orcestr-media-transcriber](https://github.com/Artasov/orcestr-media-transcriber) |
| Orcestr Media Assistant | Telegram-first assistant for your media space | ![Planned](https://img.shields.io/badge/-Planned-8b5cf6) | Planned |
| Beauty | AI product for look selection | ![Beta](https://img.shields.io/badge/-Beta-3b82f6) | [beauty.orcestr.com](https://beauty.orcestr.com) |
| Deliveries | Operations product for purchasing, stock, orders and finance | ![Dev](https://img.shields.io/badge/-Dev-f59e0b) | [deliveries.orcestr.com](https://deliveries.orcestr.com) |

## Contents

- [Ecosystem Projects](#ecosystem-projects)
- [Product Direction](#product-direction)
- [Products](#products)
    - [Orcestr Auth](#orcestr-auth)
    - [Orcestr UI](#orcestr-ui)
    - [Orcestr Icons](#orcestr-icons)
    - [Orcestr Repo Notifier](#orcestr-repo-notifier)
    - [Orcestr Media Transcriber](#orcestr-media-transcriber)
    - [Orcestr Media Assistant](#orcestr-media-assistant)
    - [Beauty](#beauty)
    - [Deliveries](#deliveries)
    - [Platform foundation](#platform-foundation)
- [Public Repositories](#public-repositories)
- [Roadmap](#roadmap)
- [Community token](#community-token)
- [Maintainer](#maintainer)

Some product code will stay closed. Reusable infrastructure should become open when it is stable, understandable and useful outside Orcestr.

## Products

### Orcestr Auth

Status: planned.

Orcestr Auth is planned as a shared authentication layer in three repositories: `orcestr-auth`, `orcestr-fastapi-auth` and `orcestr-next-auth`. It should work with React and Next.js on the frontend, FastAPI + SQLAlchemy on the backend, and cover both regular authentication and OAuth flows. The goal is to reuse identity, sessions and product authentication scenarios across all Orcestr surfaces.

Tags: authentication, React, Next.js, FastAPI, SQLAlchemy, OAuth, identity, planned.

### Orcestr UI

Status: public UI layer.

[Orcestr UI](https://github.com/Artasov/orcestr-ui) is a reusable UI foundation extracted from real Orcestr product development. It collects components, app shell patterns, workflow primitives and design tokens used in product surfaces.

Tags: UI, components, dashboards, workflows, design tokens, open source.

### Orcestr Icons

Status: planned.

Orcestr Icons is a planned package with different icon styles and icon sets. It should work as an add-on to the main Orcestr UI kit: expanding the product visual language without bloating the base UI library.

Tags: icons, icon sets, UI kit, design system, planned.

### Orcestr Repo Notifier

Status: public GitHub Action.

[Orcestr Repo Notifier](https://github.com/Artasov/orcestr-repo-notifier) turns repository changes into clear Telegram updates. It helps teams, founders and public builders show product progress after each push without manually writing posts.

Tags: Codex, Telegram, GitHub Actions, review, release notes, development updates.

### Orcestr Media Transcriber

Status: repository in early active development.

[Orcestr Media Transcriber](https://github.com/Artasov/orcestr-media-transcriber) is a repository for transcribing audio and video. It is needed as a practical foundation for reusable transcripts, media search and future media assistant scenarios.

Tags: media, transcription, AI, audio, video, workflows.

### Orcestr Media Assistant

Status: planned.

Orcestr Media Assistant is a planned large assistant for your media space. The first module should be a Telegram module for automatic chat conversations: it can tell new people about a project, answer common questions or simply support a useful dialogue. Later it can connect transcripts, a media library and content workflows.

Tags: media assistant, Telegram, chat automation, AI, transcription, planned.

### Beauty

Status: beta.

Beauty is a public AI product for trying on, editing, saving and sharing visual ideas on a real photo. It already includes:

- public landing page and multilingual app shell;
- AI chat with image and voice input;
- generated looks, before/after preview and look history;
- public pages for shared looks;
- look gallery and style presets;
- early foundation for optional salon and business workflows;
- AI credit accounting and generation limits.

The current focus is beta quality: stable generation, clear prices, beautiful shared results and a simple path from photo to saved look.

Navigation:

- AI chat and generation flow;
- look gallery;
- my looks;
- shared look pages;
- style presets;
- settings and consent flow;
- optional business and salon groundwork.

### Deliveries

Status: large module in active development.

Deliveries is an operations product for companies that manage products, suppliers, orders, warehouses and payments. The current codebase covers:

- product catalog, brands, groups, tags and imports;
- suppliers, customers and counterparties;
- purchase requests, procurement plans and purchase orders;
- shipments, warehouses, stock, lots, reservations and inventory counts;
- customer orders, returns, defects and quality flows;
- finance workplace, payment calendar, FX rates and reconciliation;
- documents, approvals, tasks, comments, notifications and search;
- operational dashboards, computed flags and risk views.

Deliveries is a deep product surface for testing the shared foundation on real multi-step business processes.

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

### Platform foundation

Status: shared foundation.

The platform layer supports all modules:

- multi-tenant access model;
- module-level permissions;
- reusable workflow primitives;
- Taskiq background jobs and scheduler;
- shared WebSocket updates;
- media/document infrastructure;
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

## Roadmap

1. Stabilize Beauty beta.
2. Prepare SOL payments for beta testing.
3. `31.07.2026` - Open beta test and prepare free beta-test access for holders.
4. Improve public sharing and gallery conversion.
5. Continue real product surfaces to test the shared foundation.
6. `16.08.2026` - Extract reusable UI primitives into `orcestr-ui`.
7. Bring `orcestr-media-transcriber` into the ecosystem as a foundation for audio/video transcripts and media search.
8. Plan Orcestr Auth as `orcestr-auth`, `orcestr-fastapi-auth` and `orcestr-next-auth` for React, Next.js and FastAPI + SQLAlchemy services.
9. Shape Orcestr Icons as an additional icon package for the main UI kit.
10. Plan Orcestr Media Assistant around media spaces, starting with a Telegram automatic conversation module.
11. Open selected workflow and backend pieces when they are stable enough.
12. Grow the Telegram community through development updates, beta feedback and product discussion.

## Community Token

ORCESTR is an experimental Community Support Token connected to the Orcestr ecosystem.

It is an optional supporter layer for people following the development early: development updates, beta participation, supporter identity and limited non-financial perks when they make sense.

It is not equity, not revenue share, not company governance and not a promise of profit. The product does not depend on the token.

Possible holder perks may include supporter badges and free beta-test access when we open public testing and the product is ready. Perks are experimental, limited and can change.

See [TOKEN.md](TOKEN.md) for the public token principles.

## Maintainer

Public updates are currently maintained by [@Artasov](https://github.com/Artasov).
