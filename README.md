<p align="right">
  <strong>English</strong> · <a href="./README.ru.md">Русский</a>
</p>

<p align="center">
  <a href="https://orcestr.com">
    <img src="./assets/orcestr-banner.webp" alt="Orcestr banner" width="100%" />
  </a>
</p>

# [Orcestr](https://orcestr.com) is open-source

[![Content license: CC BY 4.0](https://img.shields.io/badge/Content-CC_BY_4.0-lightgrey.svg)](./LICENSE)

Main website: [orcestr.com](https://orcestr.com)

Orcestr is an ecosystem with open-source libraries, a developer toolkit, applied tools and real products.

The public direction has three parts:

- Open-source **lib**s.
- Open-source **tool**s.
- Web **product**s.

## Ecosystem Projects

| Project | Type | Status | Link | Description |
| --- | --- | --- | --- | --- |
| Orcestr Core | lib | ![Beta](https://img.shields.io/badge/-Beta-3b82f6) | [Artasov/orcestr-core](https://github.com/Artasov/orcestr-core) | Shared, domain-neutral contracts and runtime adapters for consistent API errors, request context, notifications and safe navigation across TypeScript, React, Next.js, Python and FastAPI applications. Published as three npm packages and one PyPI package. |
| Orcestr Auth | lib | ![Beta](https://img.shields.io/badge/-Beta-3b82f6) | [Artasov/orcestr-auth](https://github.com/Artasov/orcestr-auth) | Reusable authentication foundation for Python/FastAPI backends, browser clients, React Query, ready-made forms on `@orcestr/ui` and Next.js guards. It covers sessions, recovery, optional GitHub, Google and Yandex OAuth, CSRF protection and WebSocket tickets while applications retain their own users, permissions, branding and tenant logic. |
| Orcestr Commerce | lib | ![Beta](https://img.shields.io/badge/-Beta-3b82f6) | [CommerceXL](https://github.com/Artasov/commercexl) · [Solana](https://github.com/Artasov/orcestr-commerce-solana) | Composable commerce and payments stack: server-priced catalogs and orders, provider contracts and exactly-once settlement, a standardized React checkout UI, and non-custodial native SOL and Token-2022 payments with finalized on-chain verification. |
| Orcestr UI | lib | ![Dev](https://img.shields.io/badge/-Dev-f59e0b) ![Beta](https://img.shields.io/badge/-Beta-3b82f6) | [Artasov/orcestr-ui](https://github.com/Artasov/orcestr-ui) | Reusable UI foundation extracted from real Orcestr product development: components, app shell patterns, workflow primitives and design tokens used in product surfaces. |
| Orcestr Icons | lib | ![Planned](https://img.shields.io/badge/-Planned-8b5cf6) | Planned | Package with different icon styles and icon sets. It works as an add-on to the main Orcestr UI kit: expanding the product visual language without bloating the base UI library. |
| Orcestr Repo Notifier | tool | ![Released](https://img.shields.io/badge/-Released-2ea44f) | [Artasov/orcestr-repo-notifier](https://github.com/Artasov/orcestr-repo-notifier) | Turns repository changes into clear Telegram updates so teams, founders and public builders can show product progress after each push without manually writing posts. |
| Orcestr Media Transcriber | tool | ![Dev](https://img.shields.io/badge/-Dev-f59e0b) ![Pre-beta](https://img.shields.io/badge/-Pre--beta-64748b) | [Artasov/orcestr-media-transcriber](https://github.com/Artasov/orcestr-media-transcriber) | Repository for transcribing audio and video: a practical foundation for reusable transcripts, media search and future media assistant scenarios. |
| Orcestr Media Assistant | tool | ![Planned](https://img.shields.io/badge/-Planned-8b5cf6) | Planned | Large assistant for your media space. The first module is a Telegram module for automatic chat conversations; later it can connect transcripts, a media library and content workflows. |
| Beauty | product | ![Beta](https://img.shields.io/badge/-Beta-3b82f6) | [beauty.orcestr.com](https://beauty.orcestr.com) | Public AI product for trying on, editing, saving and sharing visual ideas on a real photo, with AI chat, generated looks, history, gallery, presets and credit accounting. Paid plans can be purchased through the shared Commerce checkout with native SOL or ORCESTR. |
| Deliveries | product | ![Dev](https://img.shields.io/badge/-Dev-f59e0b) ![Pre-beta](https://img.shields.io/badge/-Pre--beta-64748b) | [deliveries.orcestr.com](https://deliveries.orcestr.com) | Operations product for companies that manage products, suppliers, orders, warehouses and payments; a deep surface for testing the shared foundation on real business processes. |

## Contents

- [Ecosystem Projects](#ecosystem-projects)
- [Shared Core](#shared-core)
- [Commerce Stack](#commerce-stack)
- [Roadmap](#roadmap)
- [Community token](#community-token)
- [Maintainer](#maintainer)

## Shared Core

[Orcestr Core](https://github.com/Artasov/orcestr-core) is the cross-runtime foundation for behavior that must remain
consistent between Orcestr applications without belonging to a product domain or a UI design system. Its packages share one
strict API error contract while keeping framework-specific integrations at the edges:

- [`@orcestr/core`](https://www.npmjs.com/package/@orcestr/core) provides framework-independent API transport, error
  parsing, field paths, error catalogs and safe internal navigation primitives;
- [`@orcestr/core-react`](https://www.npmjs.com/package/@orcestr/core-react) connects error presentation and notifications
  to React and TanStack Query without rendering its own UI;
- [`@orcestr/core-next`](https://www.npmjs.com/package/@orcestr/core-next) provides the small Next.js boundary for requests,
  origins and redirects;
- [`orcestr-core`](https://pypi.org/project/orcestr-core/) provides Python error models, request context and optional FastAPI
  handlers, OpenAPI integration and request-ID middleware.

Core owns shared contracts and transport mechanics. Product and authentication packages still own their business error
codes, translations and rules, while visual components and design tokens remain in Orcestr UI. This dependency direction
keeps the common foundation reusable without turning it into a monolithic application framework.

## Commerce Stack

Orcestr Commerce separates commercial state, payment providers and presentation so applications can add payment methods
without duplicating order logic or building a second checkout. The published stack consists of:

| Package | Registry | Responsibility |
| --- | --- | --- |
| `commercexl` | [PyPI](https://pypi.org/project/commercexl/) | FastAPI, Pydantic and SQLAlchemy foundation for database-backed products and prices, orders, payment attempts, provider contracts, verification state, outbox events and exactly-once product fulfillment. |
| `@orcestr/commerce-ui` | [npm](https://www.npmjs.com/package/@orcestr/commerce-ui) | Provider-neutral React checkout shell and standardized payment-method selection built on `@orcestr/ui`. |
| `orcestr-commerce-solana` | [PyPI](https://pypi.org/project/orcestr-commerce-solana/) | Backend Solana provider, transaction-request endpoints, reconciliation and strict finalized verification through standard Solana JSON-RPC. |
| `@orcestr/commerce-solana-core` | [npm](https://www.npmjs.com/package/@orcestr/commerce-solana-core) | Framework-independent Solana payment contracts, exact-amount helpers, API client and transaction validation. |
| `@orcestr/commerce-solana-react` | [npm](https://www.npmjs.com/package/@orcestr/commerce-solana-react) | React Query hooks, Wallet Standard integration and shared realtime-event adapters. |
| `@orcestr/commerce-solana-ui` | [npm](https://www.npmjs.com/package/@orcestr/commerce-solana-ui) | QR code, wallet deep link, waiting, confirmation and recovery views for the standardized checkout. |

The application keeps products and editable prices in its database. CommerceXL freezes the selected price in an order,
the user chooses a provider through one shared checkout, and the Solana add-on produces a wallet request. The backend then
decodes and verifies the exact finalized transfer before CommerceXL marks the payment as paid and applies the product once.

The Solana provider supports native SOL and explicitly allowlisted Token-2022 fungible assets, including ORCESTR. The
legacy SPL Token Program is deliberately unsupported. Payment correctness does not require a paid RPC plan, webhook,
indexer, hosted checkout or server-side private key. Authentication and CSRF remain host-owned and can be supplied by
Orcestr Auth. [Beauty](https://beauty.orcestr.com) is the first live product using this stack for SOL and ORCESTR checkout.

Some product code will stay closed. Reusable infrastructure should become open when it is stable, understandable and useful outside Orcestr.

## Roadmap

1. Stabilize Beauty beta.
2. Expand the released SOL and Token-2022 checkout beyond the first Beauty integration.
3. `31.07.2026` - Open beta test and prepare free beta-test access for holders.
4. Improve public sharing and gallery conversion.
5. Continue real product surfaces to test the shared foundation.
6. `16.08.2026` - Extract reusable UI primitives into `orcestr-ui`.
7. Bring `orcestr-media-transcriber` into the ecosystem as a foundation for audio/video transcripts and media search.
8. Stabilize the Orcestr Auth beta and its public APIs across the Python, browser, React, forms and Next.js packages.
9. Shape Orcestr Icons as an additional icon package for the main UI kit.
10. Plan Orcestr Media Assistant around media spaces, starting with a Telegram automatic conversation module.
11. Open selected workflow and backend pieces when they are stable enough.
12. Grow the Telegram community through development updates, beta feedback and product discussion.
13. Turn repeated product infrastructure into stable public packages with clear documentation, examples and versioned release flows.
14. Grow Orcestr into a coherent toolkit for building SaaS and commerce products: UI, auth, commerce, media, workflows and operational backends.

## Community Token

ORCESTR is an experimental Community Support Token connected to the Orcestr ecosystem.

It is an optional supporter layer for people following the development early: development updates, beta participation, supporter identity and limited non-financial perks when they make sense.

It is not equity, not revenue share, not company governance and not a promise of profit. The product does not depend on the token.

Possible holder perks may include supporter badges and free beta-test access when we open public testing and the product is ready. Perks are experimental, limited and can change.

See [TOKEN.md](TOKEN.md) for the public token principles.

## Maintainer

Public updates are currently maintained by [@Artasov](https://github.com/Artasov).

## License and attribution

Unless a file states otherwise, the prose and documentation are licensed under
[CC BY 4.0](./LICENSE), including commercial reuse with attribution and an indication of changes.
Use the attribution form in [NOTICE](./NOTICE). The Orcestr name, logos, banner, token symbols and
other brand assets are excluded from CC BY 4.0; see [TRADEMARKS.md](./TRADEMARKS.md).
