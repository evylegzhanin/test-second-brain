# Obsidian

Obsidian - локальная markdown-среда для связанных заметок. В контексте этой базы он выступает как IDE для [[LLM Wiki]]: пользователь читает и навигирует по wiki, а LLM поддерживает структуру.

## Почему подходит для LLM Wiki

- Markdown-файлы легко читать, diff-ить, версионировать и редактировать агентом.
- `[[wikilinks]]` создают явную сеть между страницами.
- Graph view помогает увидеть хабы, изолированные страницы и плотность связей.
- Local-first подход делает `raw/` и `wiki/` контролируемыми пользователем.

## Практики

Для ручного ведения заметок источники советуют начинать минимально: меньше папок, меньше плагинов, больше связей и переработки своими словами. Для LLM Wiki это превращается в правило: raw-источники не переписываются, а обработанный смысл живет в wiki-страницах.

## Полезные функции

- [[Obsidian Web Clipper]] для сохранения web-страниц в `raw/`.
- Templates и Dataview могут помочь, если появится frontmatter с `confidence`, `last_verified`, `sources` и `relationships`.
- Git полезен для истории изменений wiki.

## Источники

- [raw/Build a Second Brain Using Obsidian - A Practical Guide for Engineers.md](../raw/Build%20a%20Second%20Brain%20Using%20Obsidian%20%E2%80%93%20A%20Practical%20Guide%20for%20Engineers.md)
- [raw/Zettelkasten и Obsidian - лучшие друзья вашей памяти и креативности.md](../raw/Zettelkasten%20%D0%B8%20Obsidian%20%E2%80%94%20%D0%BB%D1%83%D1%87%D1%88%D0%B8%D0%B5%20%D0%B4%D1%80%D1%83%D0%B7%D1%8C%D1%8F%20%D0%B2%D0%B0%D1%88%D0%B5%D0%B9%20%D0%BF%D0%B0%D0%BC%D1%8F%D1%82%D0%B8%20%D0%B8%20%D0%BA%D1%80%D0%B5%D0%B0%D1%82%D0%B8%D0%B2%D0%BD%D0%BE%D1%81%D1%82%D0%B8.md)
- [raw/Getting Started with Zettelkasten in Obsidian.md](../raw/Getting%20Started%20with%20Zettelkasten%20in%20Obsidian.md)

## Связи

- [[LLM Wiki]]
- [[Zettelkasten]]
- [[Second Brain]]
- [[Obsidian Web Clipper]]
