# LLM Wiki

LLM Wiki - это паттерн личной базы знаний, где LLM не просто отвечает по raw-документам, а постепенно компилирует из них persistent wiki: саммари, концепты, сущности, синтезы и связи.

## Ключевая идея

В обычном RAG LLM заново извлекает релевантные куски при каждом вопросе. В LLM Wiki знание сначала перерабатывается в устойчивый промежуточный слой - `wiki/`, а затем переиспользуется. Это делает базу compounding artifact: новые источники усиливают, уточняют или оспаривают уже существующие страницы.

## Архитектура

- `raw/` - неизменяемые источники истины: статьи, клипы, pdf, транскрипты, ссылки.
- `wiki/` - LLM-maintained markdown-страницы: summaries, concept pages, entity pages, comparisons, synthesis.
- Schema - правила работы агента: как ingest-ить, когда создавать страницы, как вести ссылки, как фиксировать конфликты.

В этой базе текущие правила заданы пользователем в чате; их стоит позже вынести в отдельную страницу или проектный rule.

## Роль человека и LLM

Человек выбирает источники, задает направление и проверяет смысл. LLM выполняет обслуживание: читает источники, выделяет идеи, обновляет связи, ведет `index.md`, пишет `log.md`, отмечает противоречия и предлагает новые страницы.

## Чем отличается от Second Brain

[[Second Brain]] часто описывает широкий личный контур захвата и организации информации. LLM Wiki уже: он делает акцент на поддерживаемом слое знаний между источниками и ответами. Поэтому LLM Wiki можно считать рабочим режимом для [[Obsidian]]-vault, особенно когда источники регулярно пополняются.

## Источники

- [raw/llm-wiki.md](../raw/llm-wiki.md) - оригинальный паттерн Karpathy.
- [raw/LLM Wiki v2 - extending Karpathy's LLM Wiki pattern with lessons from building agentmemory.md](../raw/LLM%20Wiki%20v2%20%E2%80%94%20extending%20Karpathy's%20LLM%20Wiki%20pattern%20with%20lessons%20from%20building%20agentmemory.md) - расширение с lifecycle, graph и automation.
- [raw/Building my Personal LLM Wiki (Part 1) The Motivation.md](<../raw/Building%20my%20Personal%20LLM%20Wiki%20(Part%201)%20The%20Motivation.md>) - мотивация личной реализации.
- [raw/Building my Personal LLM Wiki (Part 2) The Technical Implementation.md](<../raw/Building%20my%20Personal%20LLM%20Wiki%20(Part%202)%20The%20Technical%20Implementation.md>) - техническая реализация.

## Связи

- [[LLM Wiki Workflow]]
- [[LLM Wiki Lifecycle]]
- [[Obsidian]]
- [[Second Brain]]
