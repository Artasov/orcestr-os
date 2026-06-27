<p align="right">
  <img src="./assets/orcestr-logo.png" alt="Логотип Orcestr" width="42" height="42" align="left" />
  <a href="./README.md">English</a> · <strong>Русский</strong>
</p>

# Orcestr

Orcestr - личная продуктовая кодовая база, которая развивается в публичный developer toolkit и open-source библиотеку.

Кодовая база строится вокруг общей продуктовой основы: UI patterns, application shell, identity, permissions, credits,
files, notifications, workflows, статистика и фоновые задачи. Product surfaces используют эту основу в реальных
сценариях, а самые сильные переиспользуемые части со временем могут становиться публичными пакетами.

Публичное направление состоит из двух частей:

- product surfaces, которыми можно пользоваться;
- open-source части, выделенные из production, начиная с Orcestr UI и дальше переходя к workflow, backend и application
  infrastructure.

## Содержание

- [Продуктовое направление](#продуктовое-направление)
- [Product surfaces](#product-surfaces)
    - [Beauty](#beauty)
    - [Deliveries](#deliveries)
    - [Platform foundation](#platform-foundation)
    - [Open Source: Orcestr UI](#open-source-orcestr-ui)
- [Roadmap](#roadmap)
- [Community token](#community-token)
- [Maintainer](#maintainer)

## Продуктовое направление

Ядро Orcestr - общая основа. Product surfaces нужны, чтобы проверять и улучшать эту основу в реальных workflows.

Цель - делать сфокусированные продукты и не переписывать каждый раз один и тот же операционный слой. Долгосрочное
направление - developer toolkit и open-source библиотека из компонентов, которые прошли реальное продуктовое
использование.

Open source - часть roadmap, а не отдельное маркетинговое обещание. Начинаем с того, что безопаснее и полезнее всего
переиспользовать: UI components, app shell patterns, workflow primitives и design tokens. По мере зрелости основы больше
технических частей можно будет открывать как публичные пакеты.

Часть продуктового кода останется закрытой. Переиспользуемая инфраструктура должна становиться открытой, когда она
стабильна, понятна и полезна вне Orcestr.

## Product surfaces

Product surfaces - не вся история Orcestr. Они показывают, как общая основа ведет себя в реальной продуктовой работе.

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

### Open Source: Orcestr UI

Планируемая публичная developer-работа начинается с UI:

- библиотека компонентов `orcestr-ui`;
- app shell patterns для операционных dashboard;
- modal, table, filter и workflow primitives;
- design tokens из production-модулей;
- примеры из product surfaces, если их можно безопасно открыть.

UI-библиотека должна быть полезна сама по себе. Это первый шаг к более широкому open-source слою, собранному из реальной
продуктовой работы.

## Roadmap

1. Стабилизировать Beauty beta.
2. Добавить надежный credit purchase flow и подготовить бесплатный beta-test для holders.
3. Улучшить публичный sharing и conversion из галереи.
4. Продолжать реальные product surfaces для проверки общей основы.
5. Выделить переиспользуемые UI-примитивы в `orcestr-ui`.
6. Открывать выбранные workflow и backend части, когда они достаточно стабильны.
7. Строить небольшое community вокруг продукта, а не вокруг хайпа.

## Community Token

Подробности о токене будут добавлены позже.

ORCESTR планируется как экспериментальный Community Support Token для экосистемы Orcestr.

Это не equity, не revenue share, не управление компанией и не обещание прибыли. Продукт не зависит от токена.

Возможные holder perks могут включать supporter badges и бесплатный beta-test доступ, когда мы откроем публичное тестирование и продукт будет готов. Perks экспериментальные, ограниченные и могут меняться.

См. [TOKEN.ru.md](TOKEN.ru.md) для публичных принципов токена.

## Maintainer

Публичные обновления сейчас ведет [@Artasov](https://github.com/Artasov).
