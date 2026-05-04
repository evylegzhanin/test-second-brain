# Source Notes

Краткие заметки по ingested источникам из `raw/`. Файлы `raw/` не изменялись.

## LLM Wiki sources

### llm-wiki

- Raw: [raw/llm-wiki.md](../raw/llm-wiki.md)
- URL: https://gist.github.com/karpathy/442a6bf555914893e9891c11519de94f
- Summary: оригинальный паттерн [[LLM Wiki]]: LLM поддерживает persistent markdown-wiki поверх immutable raw sources. Основные операции - ingest, query, lint; ключевые файлы - [[index]] и [[log]].
- Key terms: [[LLM Wiki]], raw sources, wiki, schema, ingest, query, lint, crystallization.

### LLM Wiki v2

- Raw: [raw/LLM Wiki v2 - extending Karpathy's LLM Wiki pattern with lessons from building agentmemory.md](../raw/LLM%20Wiki%20v2%20%E2%80%94%20extending%20Karpathy's%20LLM%20Wiki%20pattern%20with%20lessons%20from%20building%20agentmemory.md)
- URL: https://gist.github.com/rohitg00/2067ab416f7bbe447c1977edaaa681e2
- Summary: расширяет оригинальный паттерн lifecycle-подходом, typed knowledge graph, hybrid search, automation, quality controls и collaboration. Главный тезис: wiki должна не только накапливать, но и управлять свежестью, уверенностью и конфликтами.
- Key terms: [[LLM Wiki Lifecycle]], confidence, supersession, forgetting, typed relationships, hybrid search, self-healing.

### Building my Personal LLM Wiki - Part 1

- Raw: [raw/Building my Personal LLM Wiki (Part 1) The Motivation.md](<../raw/Building%20my%20Personal%20LLM%20Wiki%20(Part%201)%20The%20Motivation.md>)
- URL: https://www.rangaprabhu.com/blog/building-my-llm-wiki
- Summary: личная мотивация для LLM Wiki: не строить всеобъемлющий second brain, а создать небольшую библиотеку, где идеи связываются и переиспользуются. Главная боль - не хранение, а обслуживание базы знаний.
- Key terms: [[Second Brain]], [[LLM Wiki]], personal library, maintenance, compounding knowledge.

### Building my Personal LLM Wiki - Part 2

- Raw: [raw/Building my Personal LLM Wiki (Part 2) The Technical Implementation.md](<../raw/Building%20my%20Personal%20LLM%20Wiki%20(Part%202)%20The%20Technical%20Implementation.md>)
- URL: https://www.rangaprabhu.com/blog/building-my-personal-llm-wiki-part-2-the-implementation
- Summary: техническая реализация personal LLM Wiki на Claude Code, [[Obsidian]] и Python. Описывает raw sources, wiki pages, schema, automation scripts, confidence scores, freshness tracking и typed relationships.
- Key terms: [[LLM Wiki Workflow]], [[LLM Wiki Lifecycle]], automation, lint-wiki.py, export-graph.py.

## Obsidian, Zettelkasten, Second Brain sources

### Getting Started with Zettelkasten in Obsidian

- Raw: [raw/Getting Started with Zettelkasten in Obsidian.md](../raw/Getting%20Started%20with%20Zettelkasten%20in%20Obsidian.md)
- URL: https://obsidian.rocks/getting-started-with-zettelkasten-in-obsidian/
- Summary: практический подход к [[Zettelkasten]] в [[Obsidian]]: fleeting notes нужно регулярно перерабатывать в permanent notes, которые понятны без контекста, написаны своими словами и связаны с другими заметками.
- Key terms: [[Zettelkasten]], fleeting notes, permanent notes, atomic notes, MOC.

### Zettelkasten и Obsidian - лучшие друзья вашей памяти и креативности

- Raw: [raw/Zettelkasten и Obsidian - лучшие друзья вашей памяти и креативности.md](../raw/Zettelkasten%20%D0%B8%20Obsidian%20%E2%80%94%20%D0%BB%D1%83%D1%87%D1%88%D0%B8%D0%B5%20%D0%B4%D1%80%D1%83%D0%B7%D1%8C%D1%8F%20%D0%B2%D0%B0%D1%88%D0%B5%D0%B9%20%D0%BF%D0%B0%D0%BC%D1%8F%D1%82%D0%B8%20%D0%B8%20%D0%BA%D1%80%D0%B5%D0%B0%D1%82%D0%B8%D0%B2%D0%BD%D0%BE%D1%81%D1%82%D0%B8.md)
- URL: https://habr.com/ru/articles/548154/
- Summary: русскоязычный минималистичный старт в [[Obsidian]] и [[Zettelkasten]]: не начинать со сложных папок, формулировать идеи своими словами, использовать `[[wikilinks]]` как главный инструмент и стремиться к атомарности.
- Key terms: [[Obsidian]], [[Zettelkasten]], атомарность, обратные ссылки, минимализм.

### Zettelkasten и Obsidian: ваш помощник в структурировании знаний

- Raw: [raw/Zettelkasten и Obsidian ваш помощник в структурировании знаний.md](../raw/Zettelkasten%20%D0%B8%20Obsidian%20%D0%B2%D0%B0%D1%88%20%D0%BF%D0%BE%D0%BC%D0%BE%D1%89%D0%BD%D0%B8%D0%BA%20%D0%B2%20%D1%81%D1%82%D1%80%D1%83%D0%BA%D1%82%D1%83%D1%80%D0%B8%D1%80%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D0%B8%20%D0%B7%D0%BD%D0%B0%D0%BD%D0%B8%D0%B9.md)
- URL: https://habr.com/ru/articles/854230/
- Summary: источник неполный: после frontmatter содержит только слово `Zettelkasten`. Использовать осторожно; содержательных утверждений для wiki почти нет.
- Key terms: [[Zettelkasten]]

### Introduction to Obsidian Web Clipper

- Raw: [raw/Introduction to Obsidian Web Clipper.md](../raw/Introduction%20to%20Obsidian%20Web%20Clipper.md)
- URL: https://obsidian.md/help/web-clipper
- Summary: справка по [[Obsidian Web Clipper]]: расширение сохраняет web-контент и highlights в vault, поддерживает templates, variables, filters, logic и локальное хранение.
- Key terms: [[Obsidian Web Clipper]], clipper, highlighter, reader, templates.

### Build a Second Brain Using Obsidian

- Raw: [raw/Build a Second Brain Using Obsidian - A Practical Guide for Engineers.md](../raw/Build%20a%20Second%20Brain%20Using%20Obsidian%20%E2%80%93%20A%20Practical%20Guide%20for%20Engineers.md)
- URL: https://ps11.hashnode.dev/engineers-guide-to-building-a-second-brain-in-obsidian-practical-tips
- Summary: практическое введение в [[Second Brain]] на [[Obsidian]] для инженеров. Делает акцент на markdown, локальности, linking, graph view, plugins, привычке ежедневного использования и [[PARA]].
- Key terms: [[Second Brain]], [[Obsidian]], [[PARA]], Dataview, QuickAdd, templates, graph view.

## Замеченные проблемы качества

- Один raw-файл про Zettelkasten неполный и требует повторного clipping или другого источника.
- Источники по LLM Wiki v2 предлагают более сложную систему, чем минимальный Karpathy-паттерн; это отмечено как расширение, не противоречие.

## Связи

- [[LLM Wiki]]
- [[LLM Wiki Workflow]]
- [[LLM Wiki Lifecycle]]
- [[Obsidian]]
- [[Zettelkasten]]
- [[Second Brain]]
- [[Obsidian Web Clipper]]
