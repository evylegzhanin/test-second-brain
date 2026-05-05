# Wiki Log

Хронологический журнал изменений LLM-Wiki.

## [2026-05-04] ingest | Initial raw folder bootstrap

- Processed 9 sources from `raw/` without modifying raw files.
- Created initial wiki map: [[index]].
- Created concept pages: [[LLM Wiki]], [[LLM Wiki Workflow]], [[LLM Wiki Lifecycle]], [[Obsidian]], [[Zettelkasten]], [[Second Brain]], [[PARA]], [[Obsidian Web Clipper]].
- Created source overview: [[Source Notes]].
- Noted quality issue: `raw/Zettelkasten и Obsidian ваш помощник в структурировании знаний.md` appears incomplete and contains almost no article body.
- No direct contradiction found; richer lifecycle/automation sources are treated as extensions of the minimal [[LLM Wiki]] pattern.

## [2026-05-04] maintenance | Added maintainer prompts

- Created `prompts/initial-llm-wiki-prompt.md` with the initial LLM-Wiki maintainer prompt.
- Created `prompts/raw-change-workflow-prompt.md` with the workflow for added or removed files in `raw/`.
- Updated `README.md` to document the `prompts/` directory.

## [2026-05-05] maintenance | Consolidated agent rules into AGENTS.md

- Создан `AGENTS.md` в корне репозитория как единый schema-файл с правилами для LLM-агента (соответствует рекомендации паттерна [[LLM Wiki]]).
- Удалены `prompts/initial-llm-wiki-prompt.md` и `prompts/raw-change-workflow-prompt.md`; их содержимое объединено в `AGENTS.md` (baseline + workflow при изменениях в `raw/`).
- Удалена пустая папка `prompts/`.
- Удалён `.cursor/rules/llm-wiki-maintenance.mdc` — Cursor подхватывает `AGENTS.md` нативно, отдельный rule-файл стал дубликатом.
- Обновлён `README.md`: раздел «Промпты» заменён на раздел «Schema для агента» со ссылкой на `AGENTS.md`.
- Обновлён [[index]]: закрыт открытый вопрос про необходимость schema-файла в пользу `AGENTS.md`; добавлена секция «Schema агента».
- Содержательных изменений в `wiki/`-страницах и в `raw/` нет.
