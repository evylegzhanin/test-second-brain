# LLM Wiki Workflow

Основные операции LLM Wiki: ingest, query, lint и crystallization. Они превращают vault из папки с заметками в поддерживаемую систему знаний.

## Ingest

Ingest нового источника:

1. Прочитать файл из `raw/`.
2. Сделать краткое саммари.
3. Выделить ключевые идеи, термины и сущности.
4. Создать или обновить страницы в `wiki/`.
5. Добавить `[[wikilinks]]` и ссылки на raw/source URL.
6. Обновить [[index]].
7. Добавить запись в [[log]].

В расширенной версии ingest также включает confidence, freshness, typed relationships и health-check после обработки.

## Query

При вопросе сначала читается [[index]], затем релевантные страницы `wiki/`. Только если wiki недостаточно, агент обращается к `raw/`. Если ответ содержит новый устойчивый вывод, его стоит сохранить как отдельную страницу или раздел.

## Lint

Периодический lint должен искать:

- битые `[[wikilinks]]`;
- дублирующиеся страницы;
- устаревшие утверждения;
- противоречия между источниками;
- страницы без входящих ссылок;
- важные упоминания без отдельной страницы.

## Crystallization

Crystallization - это сохранение результата исследования или ответа как wiki-страницы. В отличие от обычного ответа в чате, такой вывод становится частью базы и может усиливать существующие страницы.

## Практический ритм

- Daily capture: новые web-источники попадают в `raw/` через [[Obsidian Web Clipper]].
- Ingest по одному источнику или небольшими пачками.
- Query по wiki с цитированием источников.
- Monthly lint: проверить здоровье базы и обновить stale-страницы.

## Источники

- [raw/llm-wiki.md](../raw/llm-wiki.md)
- [raw/LLM Wiki v2 - extending Karpathy's LLM Wiki pattern with lessons from building agentmemory.md](../raw/LLM%20Wiki%20v2%20%E2%80%94%20extending%20Karpathy's%20LLM%20Wiki%20pattern%20with%20lessons%20from%20building%20agentmemory.md)
- [raw/Building my Personal LLM Wiki (Part 2) The Technical Implementation.md](<../raw/Building%20my%20Personal%20LLM%20Wiki%20(Part%202)%20The%20Technical%20Implementation.md>)

## Связи

- [[LLM Wiki]]
- [[LLM Wiki Lifecycle]]
- [[Source Notes]]
