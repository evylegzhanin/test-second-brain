# LLM-Wiki Index

Карта обработанной базы знаний. Начинать поиск по vault стоит отсюда, затем переходить в тематические страницы и при необходимости в `raw/`.

## Центральные темы

- [[LLM Wiki]] - паттерн, где LLM поддерживает persistent markdown-wiki поверх неизменяемых источников.
- [[LLM Wiki Workflow]] - операции ingest, query, lint и crystallization.
- [[LLM Wiki Lifecycle]] - confidence, freshness, supersession, forgetting и typed relationships.
- [[Obsidian]] - локальная markdown-среда для связанной базы знаний.
- [[Zettelkasten]] - атомарные заметки, связи и переработка fleeting notes в permanent notes.
- [[Second Brain]] - внешний мозг для захвата, организации и переиспользования знаний.
- [[PARA]] - Projects, Areas, Resources, Archives как практичная система организации.
- [[Obsidian Web Clipper]] - инструмент захвата web-источников в vault.

## Источники

- [[Source Notes]] - краткие саммари всех ingested `raw/`-источников и замечания по качеству.

## Полезные маршруты

- Для настройки этого vault: [[LLM Wiki]] -> [[LLM Wiki Workflow]] -> [[LLM Wiki Lifecycle]].
- Для практики ведения заметок: [[Obsidian]] -> [[Zettelkasten]] -> [[Second Brain]].
- Для захвата новых материалов: [[Obsidian Web Clipper]] -> [[LLM Wiki Workflow]].

## Schema агента

Правила для LLM-агента, который поддерживает vault, лежат в `AGENTS.md` в корне репозитория. Это единственный source of truth для базового поведения: ingest, query, lint, обработка изменений в `raw/`, lifecycle и конфликты источников.

## Открытые вопросы

- Будем ли вводить lifecycle-поля в frontmatter каждой wiki-страницы: `confidence`, `last_verified`, `sources`, `relationships`?
