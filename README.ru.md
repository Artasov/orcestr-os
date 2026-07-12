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
| Orcestr Auth              | lib     | ![Beta](https://img.shields.io/badge/-Beta-3b82f6)                                                           | [Artasov/orcestr-auth](https://github.com/Artasov/orcestr-auth)                           | Переиспользуемая основа авторизации для Python/FastAPI backend, браузерных клиентов, React Query, готовых форм на `@orcestr/ui` и защитных helpers для Next.js. Она покрывает сессии, восстановление, опциональные GitHub, Google и Яндекс OAuth, CSRF-защиту и WebSocket tickets, а пользователи, permissions, брендинг и tenant logic остаются в приложении. |
| Orcestr Commerce          | lib     | ![Beta](https://img.shields.io/badge/-Beta-3b82f6)                                                           | `orcestr-commerce`                                                                        | Composable commerce core для записей каталога, checkout orders, order items и payment systems: SQLAlchemy models, явная сборка через CommerceModule и FastAPI router assembly. Репозиторий пока не публичный.                                           |
| Orcestr UI                | lib     | ![Dev](https://img.shields.io/badge/-Dev-f59e0b) ![Beta](https://img.shields.io/badge/-Beta-3b82f6)          | [Artasov/orcestr-ui](https://github.com/Artasov/orcestr-ui)                               | Переиспользуемая UI-основа, выделенная из реальной продуктовой разработки Orcestr: components, app shell patterns, workflow primitives и design tokens, которые используются в product surfaces.                                                     |
| Orcestr Icons             | lib     | ![Planned](https://img.shields.io/badge/-Planned-8b5cf6)                                                     | Запланировано                                                                             | Пакет с разными видами иконок и наборами иконок. Он работает как дополнение к основному Orcestr UI kit: расширяет визуальный язык продукта, но не раздувает базовую UI-библиотеку.                                                                   |
| Orcestr Repo Notifier     | tool    | ![Released](https://img.shields.io/badge/-Released-2ea44f)                                                   | [Artasov/orcestr-repo-notifier](https://github.com/Artasov/orcestr-repo-notifier)         | Превращает изменения в репозитории в понятные Telegram-обновления, чтобы команды, founders и public builders показывали прогресс продукта после каждого push без ручного написания постов.                                                           |
| Orcestr Media Transcriber | tool    | ![Dev](https://img.shields.io/badge/-Dev-f59e0b) ![Pre-beta](https://img.shields.io/badge/-Pre--beta-64748b) | [Artasov/orcestr-media-transcriber](https://github.com/Artasov/orcestr-media-transcriber) | Репозиторий для транскрибации аудио и видео: практическая основа для переиспользуемых транскриптов, поиска по медиа и будущих сценариев медиа-помощников.                                                                                            |
| Orcestr Media Assistant   | tool    | ![Planned](https://img.shields.io/badge/-Planned-8b5cf6)                                                     | Запланировано                                                                             | Большой ассистент для вашего медиа-пространства. Первый модуль - Telegram-модуль автоматической беседы в чате; дальше он может связывать транскрипты, медиатеку и workflows для контента.                                                            |
| Beauty                    | product | ![Beta](https://img.shields.io/badge/-Beta-3b82f6)                                                           | [beauty.orcestr.com](https://beauty.orcestr.com)                                          | Публичный AI-продукт для примерки, редактирования, сохранения и sharing визуальных идей на реальном фото: AI-чат, сгенерированные образы, история, галерея, presets и учет AI credits.                                                               |
| Deliveries                | product | ![Dev](https://img.shields.io/badge/-Dev-f59e0b) ![Pre-beta](https://img.shields.io/badge/-Pre--beta-64748b) | [deliveries.orcestr.com](https://deliveries.orcestr.com)                                  | Операционный продукт для компаний, которые управляют товарами, поставщиками, заказами, складами и оплатами; глубокий surface для проверки общей основы на реальных бизнес-процессах.                                                                 |

## Содержание

- [Проекты экосистемы](#проекты-экосистемы)
- [Roadmap](#roadmap)
- [Community token](#community-token)
- [Maintainer](#maintainer)

Часть продуктового кода останется закрытой. Переиспользуемая инфраструктура должна становиться открытой, когда она
стабильна, понятна и полезна вне Orcestr.

## Roadmap

1. Стабилизировать Beauty beta.
2. Подготовиться к оплате через SOL для бета тестирования.
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
