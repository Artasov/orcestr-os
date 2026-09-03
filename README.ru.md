<p align="right">
  <a href="./README.md">English</a> · <strong>Русский</strong>
</p>

<p align="center">
  <a href="https://orcestr.com">
    <img src="./assets/orcestr-banner.webp" alt="Баннер Orcestr" width="100%" />
  </a>
</p>

# [Orcestr](https://orcestr.com) Is Open-Source

[![Лицензия контента: CC BY 4.0](https://img.shields.io/badge/Content-CC_BY_4.0-lightgrey.svg)](./LICENSE)

Основной сайт: [orcestr.com](https://orcestr.com)

Orcestr - экосистема где есть open-source библиотеки, developer toolkit, прикладные инструкменты и реальные продукты.

Публичное направление состоит из трех частей:

- Open-source **lib**s.
- Open-source **tool**s.
- Web **product**s.

## Проекты экосистемы

| Проект                    | Тип     | Статус                                                                                                       | Ссылка                                                                                    | Описание                                                                                                                                                                                                                                             |
|---------------------------|---------|--------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Orcestr Core              | lib     | ![Beta](https://img.shields.io/badge/-Beta-3b82f6)                                                           | [Artasov/orcestr-core](https://github.com/Artasov/orcestr-core)                           | Общие, независимые от бизнес-домена контракты и runtime-адаптеры для единообразной обработки API-ошибок, контекста запросов, уведомлений и безопасной навигации в TypeScript, React, Next.js, Python и FastAPI. Публикуется как три npm-пакета и один пакет на PyPI. |
| Orcestr Auth              | lib     | ![Beta](https://img.shields.io/badge/-Beta-3b82f6)                                                           | [Artasov/orcestr-auth](https://github.com/Artasov/orcestr-auth)                           | Переиспользуемая основа авторизации для Python/FastAPI backend, браузерных клиентов, React Query, готовых форм на `@orcestr/ui` и защитных helpers для Next.js. Она покрывает сессии, восстановление, опциональные GitHub, Google и Яндекс OAuth, CSRF-защиту и WebSocket tickets, а пользователи, permissions, брендинг и tenant logic остаются в приложении. |
| Orcestr Commerce          | lib     | ![Beta](https://img.shields.io/badge/-Beta-3b82f6)                                                           | [CommerceXL](https://github.com/Artasov/commercexl) · [Solana](https://github.com/Artasov/orcestr-commerce-solana) | Композиционный commerce- и payment-стек: каталоги и заказы с серверными ценами, контракты провайдеров и однократное исполнение заказа, стандартизированный React checkout UI и некастодиальная оплата native SOL и Token-2022 с finalized-проверкой в блокчейне. |
| Orcestr UI                | lib     | ![Dev](https://img.shields.io/badge/-Dev-f59e0b) ![Beta](https://img.shields.io/badge/-Beta-3b82f6)          | [Artasov/orcestr-ui](https://github.com/Artasov/orcestr-ui)                               | Переиспользуемая UI-основа, выделенная из реальной продуктовой разработки Orcestr: components, app shell patterns, workflow primitives и design tokens, которые используются в product surfaces.                                                     |
| Orcestr Icons             | lib     | ![Planned](https://img.shields.io/badge/-Planned-8b5cf6)                                                     | Запланировано                                                                             | Пакет с разными видами иконок и наборами иконок. Он работает как дополнение к основному Orcestr UI kit: расширяет визуальный язык продукта, но не раздувает базовую UI-библиотеку.                                                                   |
| Orcestr Repo Notifier     | tool    | ![Released](https://img.shields.io/badge/-Released-2ea44f)                                                   | [Artasov/orcestr-repo-notifier](https://github.com/Artasov/orcestr-repo-notifier)         | Превращает изменения в репозитории в понятные Telegram-обновления, чтобы команды, founders и public builders показывали прогресс продукта после каждого push без ручного написания постов.                                                           |
| Orcestr Media Transcriber | tool    | ![Dev](https://img.shields.io/badge/-Dev-f59e0b) ![Pre-beta](https://img.shields.io/badge/-Pre--beta-64748b) | [Artasov/orcestr-media-transcriber](https://github.com/Artasov/orcestr-media-transcriber) | Репозиторий для транскрибации аудио и видео: практическая основа для переиспользуемых транскриптов, поиска по медиа и будущих сценариев медиа-помощников.                                                                                            |
| Orcestr Media Assistant   | tool    | ![Planned](https://img.shields.io/badge/-Planned-8b5cf6)                                                     | Запланировано                                                                             | Большой ассистент для вашего медиа-пространства. Первый модуль - Telegram-модуль автоматической беседы в чате; дальше он может связывать транскрипты, медиатеку и workflows для контента.                                                            |
| Beauty                    | product | ![Beta](https://img.shields.io/badge/-Beta-3b82f6)                                                           | [beauty.orcestr.com](https://beauty.orcestr.com)                                          | Публичный AI-продукт для примерки, редактирования, сохранения и sharing визуальных идей на реальном фото: AI-чат, сгенерированные образы, история, галерея, presets и учет AI credits. Платные тарифы доступны через общий Commerce checkout с оплатой native SOL или ORCESTR. |
| Deliveries                | product | ![Dev](https://img.shields.io/badge/-Dev-f59e0b) ![Pre-beta](https://img.shields.io/badge/-Pre--beta-64748b) | [deliveries.orcestr.com](https://deliveries.orcestr.com)                                  | Операционный продукт для компаний, которые управляют товарами, поставщиками, заказами, складами и оплатами; глубокий surface для проверки общей основы на реальных бизнес-процессах.                                                                 |

## Содержание

- [Проекты экосистемы](#проекты-экосистемы)
- [Общий Core](#общий-core)
- [Commerce-стек](#commerce-стек)
- [Roadmap](#roadmap)
- [Community token](#community-token)
- [Maintainer](#maintainer)

## Общий Core

[Orcestr Core](https://github.com/Artasov/orcestr-core) — кросс-платформенная основа для поведения, которое должно быть
одинаковым во всех приложениях Orcestr, но не относится к конкретному бизнес-домену или визуальной дизайн-системе. Пакеты
используют единый строгий контракт API-ошибок, а интеграции с фреймворками остаются на внешних слоях:

- [`@orcestr/core`](https://www.npmjs.com/package/@orcestr/core) содержит независимые от фреймворков API transport,
  разбор ошибок, пути полей, каталоги ошибок и примитивы безопасной внутренней навигации;
- [`@orcestr/core-react`](https://www.npmjs.com/package/@orcestr/core-react) связывает представление ошибок и уведомления
  с React и TanStack Query, но не отрисовывает собственный UI;
- [`@orcestr/core-next`](https://www.npmjs.com/package/@orcestr/core-next) содержит небольшой Next.js-слой для запросов,
  origins и redirects;
- [`orcestr-core`](https://pypi.org/project/orcestr-core/) содержит Python-модели ошибок, контекст запроса и опциональные
  FastAPI handlers, интеграцию с OpenAPI и middleware для request ID.

Core отвечает за общие контракты и механику передачи данных. Продуктовые и авторизационные пакеты по-прежнему владеют
бизнес-кодами ошибок, переводами и правилами, а визуальные компоненты и design tokens остаются в Orcestr UI. Такое
направление зависимостей сохраняет общую основу переиспользуемой и не превращает её в монолитный application framework.

## Commerce-стек

Orcestr Commerce разделяет коммерческие данные, платежных провайдеров и интерфейс. Приложение может добавлять способы
оплаты без дублирования логики заказов и без создания отдельного checkout для каждого провайдера. Опубликованный стек:

| Пакет | Registry | Ответственность |
| --- | --- | --- |
| `commercexl` | [PyPI](https://pypi.org/project/commercexl/) | Основа на FastAPI, Pydantic и SQLAlchemy для продуктов и цен в БД, заказов, платежных попыток, контрактов провайдеров, состояний проверки, outbox-событий и однократного исполнения продукта. |
| `@orcestr/commerce-ui` | [npm](https://www.npmjs.com/package/@orcestr/commerce-ui) | Нейтральная к провайдеру React-оболочка checkout и стандартизированный выбор способа оплаты на `@orcestr/ui`. |
| `orcestr-commerce-solana` | [PyPI](https://pypi.org/project/orcestr-commerce-solana/) | Backend-провайдер Solana, transaction-request endpoints, reconciliation и строгая finalized-проверка через стандартный Solana JSON-RPC. |
| `@orcestr/commerce-solana-core` | [npm](https://www.npmjs.com/package/@orcestr/commerce-solana-core) | Независимые от фреймворка контракты Solana-платежей, точные суммы, API client и проверка транзакции. |
| `@orcestr/commerce-solana-react` | [npm](https://www.npmjs.com/package/@orcestr/commerce-solana-react) | React Query hooks, интеграция Wallet Standard и адаптеры общих realtime-событий. |
| `@orcestr/commerce-solana-ui` | [npm](https://www.npmjs.com/package/@orcestr/commerce-solana-ui) | QR-код, deep link для кошелька, ожидание, подтверждение и восстановление внутри стандартизированного checkout. |

Продукты и редактируемые цены остаются в базе приложения. CommerceXL фиксирует выбранную цену в заказе, пользователь
выбирает провайдера в едином checkout, а Solana-дополнение создаёт запрос для кошелька. Backend декодирует и проверяет
точный finalized-перевод, после чего CommerceXL помечает платеж оплаченным и исполняет продукт ровно один раз.

Solana-провайдер поддерживает native SOL и явно разрешённые fungible-активы Token-2022, включая ORCESTR. Legacy SPL Token
Program намеренно не поддерживается. Для корректной проверки не нужны платный RPC-тариф, webhook, индексатор, hosted
checkout или приватный ключ на сервере. Аутентификация и CSRF остаются ответственностью host-приложения и могут быть
подключены через Orcestr Auth. [Beauty](https://beauty.orcestr.com) — первая production-интеграция этого стека с оплатой
через SOL и ORCESTR.

Часть продуктового кода останется закрытой. Переиспользуемая инфраструктура должна становиться открытой, когда она
стабильна, понятна и полезна вне Orcestr.

## Roadmap

1. Стабилизировать Beauty beta.
2. Расширить выпущенный checkout через SOL и Token-2022 за пределы первой интеграции Beauty.
3. `31.07.2026` - Открыть beta test и подготовить бесплатный beta-test для holders.
4. Улучшить публичный sharing и conversion из галереи.
5. Продолжать реальные product surfaces для проверки общей основы.
6. `16.08.2026` - Выделить переиспользуемые UI-примитивы в `orcestr-ui`.
7. Ввести `orcestr-media-transcriber` в экосистему как основу для аудио/видео транскриптов и поиска по медиа.
8. Стабилизировать beta Orcestr Auth и public API пакетов для Python, browser, React, forms и Next.js.
9. Сформировать Orcestr Icons как дополнительный пакет иконок для основного UI kit.
10. Спланировать Orcestr Media Assistant вокруг media spaces, начав с Telegram-модуля автоматической беседы.
11. Открывать выбранные workflow и backend части, когда они достаточно стабильны.
12. Развивать Telegram community через обновления разработки, beta feedback и обсуждение продукта.
13. Превращать повторяющуюся продуктовую инфраструктуру в стабильные публичные пакеты с понятной документацией, примерами и версионированными релизами.
14. Вырастить Orcestr в цельный toolkit для создания SaaS и commerce-продуктов: UI, auth, commerce, media, workflows и операционные backends.

## Community Token

ORCESTR - экспериментальный Community Support Token, связанный с экосистемой Orcestr.

Это optional supporter layer для тех, кто рано следит за разработкой: development updates, beta participation, supporter identity и ограниченные нефинансовые perks, когда они уместны.

Это не equity, не revenue share, не управление компанией и не обещание прибыли. Продукт не зависит от токена.

Возможные holder perks могут включать supporter badges и бесплатный beta-test доступ, когда мы откроем публичное тестирование и продукт будет готов. Perks экспериментальные, ограниченные и могут меняться.

См. [TOKEN.ru.md](TOKEN.ru.md) для публичных принципов токена.

## Maintainer   

Публичные обновления сейчас ведет [@Artasov](https://github.com/Artasov).

## Лицензия и указание авторства

Если в файле не указано иное, тексты и документация распространяются по
[CC BY 4.0](./LICENSE): коммерческое использование разрешено при указании авторства и внесенных
изменений. Рекомендуемая форма указана в [NOTICE](./NOTICE). Название Orcestr, логотипы, баннер,
символы токена и другие элементы бренда исключены из CC BY 4.0; см.
[TRADEMARKS.md](./TRADEMARKS.md).
