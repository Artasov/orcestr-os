<p align="right">
  <a href="./README.md">English</a> · <strong>Русский</strong>
</p>

<p align="center">
  <a href="https://orcestr.com">
    <img src="./assets/orcestr-banner.webp" alt="Баннер Orcestr" width="100%" />
  </a>
</p>

# [Orcestr](https://orcestr.com) is open-source

Основной сайт: [orcestr.com](https://orcestr.com)

Orcestr - экосистема где есть open-source библиотеки, developer toolkit, прикладные инструкменты и реальные продукты.

Публичное направление состоит из трех частей:

- Open-source **lib**s.
- Open-source **tool**s.
- Web **product**s.

 ## Проекты экосистемы

| Проект | Тип | Статус | Ссылка |
| --- | --- | --- | --- |
| Orcestr Auth | Общий слой авторизации для React, Next.js и FastAPI-сервисов | ![Planned](https://img.shields.io/badge/-Planned-8b5cf6) | Запланировано: `orcestr-auth`, `orcestr-fastapi-auth`, `orcestr-next-auth` |
| Orcestr UI | Публичная UI-библиотека из продуктовой разработки | ![Dev](https://img.shields.io/badge/-Dev-f59e0b) | [Artasov/orcestr-ui](https://github.com/Artasov/orcestr-ui) |
| Orcestr Icons | Пакет разных видов иконок как дополнение к Orcestr UI | ![Planned](https://img.shields.io/badge/-Planned-8b5cf6) | Запланировано |
| Orcestr Repo Notifier | GitHub Action для Codex-generated Telegram development updates | ![Released](https://img.shields.io/badge/-Released-2ea44f) | [Artasov/orcestr-repo-notifier](https://github.com/Artasov/orcestr-repo-notifier) |
| Orcestr Media Transcriber | Репозиторий для транскрибации медиа | ![Dev](https://img.shields.io/badge/-Dev-f59e0b) | [Artasov/orcestr-media-transcriber](https://github.com/Artasov/orcestr-media-transcriber) |
| Orcestr Media Assistant | Telegram-first ассистент для вашего медиа-пространства | ![Planned](https://img.shields.io/badge/-Planned-8b5cf6) | Запланировано |
| Beauty | AI-продукт для подбора образа | ![Beta](https://img.shields.io/badge/-Beta-3b82f6) | [beauty.orcestr.com](https://beauty.orcestr.com) |
| Deliveries | Операционный продукт для закупок, остатков, заказов и финансов | ![Dev](https://img.shields.io/badge/-Dev-f59e0b) | [deliveries.orcestr.com](https://deliveries.orcestr.com) |

## Содержание

- [Проекты экосистемы](#проекты-экосистемы)
- [Продуктовое направление](#продуктовое-направление)
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
- [Публичные репозитории](#публичные-репозитории)
- [Roadmap](#roadmap)
- [Community token](#community-token)
- [Maintainer](#maintainer)

Часть продуктового кода останется закрытой. Переиспользуемая инфраструктура должна становиться открытой, когда она
стабильна, понятна и полезна вне Orcestr.

## Products

### Orcestr Auth

Статус: запланировано.

Orcestr Auth планируется как общий слой авторизации в трех репозиториях: `orcestr-auth`, `orcestr-fastapi-auth` и `orcestr-next-auth`. Он должен работать с React и Next.js на frontend, FastAPI + SQLAlchemy на backend, а также покрывать обычную авторизацию и OAuth-сценарии. Цель - переиспользовать identity, sessions и продуктовые сценарии авторизации во всех Orcestr surfaces.

Теги: authentication, React, Next.js, FastAPI, SQLAlchemy, OAuth, identity, planned.

### Orcestr UI

Статус: публичный UI-слой.

[Orcestr UI](https://github.com/Artasov/orcestr-ui) - переиспользуемая UI-основа, выделенная из реальной продуктовой разработки Orcestr. Здесь собираются components, app shell patterns, workflow primitives и design tokens, которые используются в product surfaces.

Теги: UI, components, dashboards, workflows, design tokens, open source.

### Orcestr Icons

Статус: запланировано.

Orcestr Icons - запланированный пакет с разными видами иконок и наборами иконок. Он должен работать как дополнение к основному Orcestr UI kit: расширять визуальный язык продукта, но не раздувать базовую UI-библиотеку.

Теги: icons, icon sets, UI kit, design system, planned.

### Orcestr Repo Notifier

Статус: публичный GitHub Action.

[Orcestr Repo Notifier](https://github.com/Artasov/orcestr-repo-notifier) превращает изменения в репозитории в понятные Telegram-обновления. Он помогает командам, founders и public builders показывать прогресс продукта после каждого push без ручного написания постов.

Теги: Codex, Telegram, GitHub Actions, review, release notes, development updates.

### Orcestr Media Transcriber

Статус: репозиторий в ранней активной разработке.

[Orcestr Media Transcriber](https://github.com/Artasov/orcestr-media-transcriber) - репозиторий для транскрибации аудио и видео. Он нужен как практическая основа для переиспользуемых транскриптов, поиска по медиа и будущих сценариев медиа-помощников.

Теги: media, transcription, AI, audio, video, workflows.

### Orcestr Media Assistant

Статус: запланировано.

Orcestr Media Assistant - запланированный большой ассистент для вашего медиа-пространства. Первым модулем должен стать Telegram-модуль автоматической беседы в чате: он сможет рассказывать новым людям о проекте, отвечать на частые вопросы или просто поддерживать полезный диалог. Дальше он может связывать транскрипты, медиатеку и workflows для контента.

Теги: media assistant, Telegram, chat automation, AI, transcription, planned.

### Beauty

Статус: beta.

Beauty - публичный AI-продукт для примерки, редактирования, сохранения и sharing визуальных идей на реальном фото. Уже
есть:

- публичный лендинг и мультиязычная оболочка приложения;
- AI-чат с изображениями и голосовым вводом;
- сгенерированные образы, before/after просмотр и история образов;
- публичные страницы для shared образов;
- галерея образов и style presets;
- ранняя база для optional salon и business workflows;
- учет AI credits и лимиты генерации.

Текущий фокус - beta-качество: стабильная генерация, понятные цены, красивые shared результаты и простой путь от фото к
сохраненному образу.

Навигация:

- AI-чат и generation flow;
- галерея образов;
- мои образы;
- shared look pages;
- style presets;
- settings и consent flow;
- optional business и salon groundwork.

### Deliveries

Статус: большой модуль в активной разработке.

Deliveries - операционный продукт для компаний, которые управляют товарами, поставщиками, заказами, складами и оплатами.
Сейчас кодовая база покрывает:

- каталог товаров, бренды, группы, теги и импорты;
- поставщиков, покупателей и контрагентов;
- заявки на закупку, планы закупок и заказы поставщикам;
- поставки, склады, остатки, партии, резервы и инвентаризации;
- клиентские заказы, возвраты, дефекты и quality flows;
- finance workplace, платежный календарь, FX rates и сверки;
- документы, согласования, задачи, комментарии, уведомления и поиск;
- операционные dashboard, computed flags и risk views.

Deliveries - глубокий product surface для проверки общей основы на реальных многошаговых бизнес-процессах.

Навигация:

- продукты и каталог;
- поставщики, покупатели и контрагенты;
- procurement и purchase orders;
- shipments и in-transit;
- склады, остатки и инвентаризации;
- клиентские заказы, возвраты и дефекты;
- finance, payment calendar и reconciliation;
- задачи, согласования, комментарии и документы;
- operational dashboards и search.

### Platform foundation

Статус: общая основа.

Платформенный слой поддерживает все модули:

- multi-tenant модель доступа;
- права на уровне модулей;
- переиспользуемые workflow-примитивы;
- Taskiq background jobs и scheduler;
- shared WebSocket updates;
- media/document infrastructure;
- AI provider runtime и credit ledger;
- админские инструменты через XLAdmin.

Навигация:

- identity и tenants;
- permissions и module access;
- tasks и approvals;
- notifications и comments;
- documents и exports;
- AI runtime и credits;
- background jobs и scheduler;
- admin tooling.

## Roadmap

1. Стабилизировать Beauty beta.
2. Подготовиться к оплате через SOL для бета тестирования.
3. `31.07.2026` - Открыть beta test и подготовить бесплатный beta-test для holders.
4. Улучшить публичный sharing и conversion из галереи.
5. Продолжать реальные product surfaces для проверки общей основы.
6. `16.08.2026` - Выделить переиспользуемые UI-примитивы в `orcestr-ui`.
7. Ввести `orcestr-media-transcriber` в экосистему как основу для аудио/видео транскриптов и поиска по медиа.
8. Спланировать Orcestr Auth как `orcestr-auth`, `orcestr-fastapi-auth` и `orcestr-next-auth` для React, Next.js и FastAPI + SQLAlchemy сервисов.
9. Сформировать Orcestr Icons как дополнительный пакет иконок для основного UI kit.
10. Спланировать Orcestr Media Assistant вокруг media spaces, начав с Telegram-модуля автоматической беседы.
11. Открывать выбранные workflow и backend части, когда они достаточно стабильны.
12. Развивать Telegram community через обновления разработки, beta feedback и обсуждение продукта.

## Community Token

ORCESTR - экспериментальный Community Support Token, связанный с экосистемой Orcestr.

Это optional supporter layer для тех, кто рано следит за разработкой: development updates, beta participation, supporter identity и ограниченные нефинансовые perks, когда они уместны.

Это не equity, не revenue share, не управление компанией и не обещание прибыли. Продукт не зависит от токена.

Возможные holder perks могут включать supporter badges и бесплатный beta-test доступ, когда мы откроем публичное тестирование и продукт будет готов. Perks экспериментальные, ограниченные и могут меняться.

См. [TOKEN.ru.md](TOKEN.ru.md) для публичных принципов токена.

## Maintainer

Публичные обновления сейчас ведет [@Artasov](https://github.com/Artasov).
