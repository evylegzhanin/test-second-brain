# LLM Wiki Lifecycle

Lifecycle-подход решает проблему "wiki rot": не все утверждения остаются одинаково точными, свежими и полезными.

## Confidence

Каждое важное утверждение желательно оценивать по надежности: сколько источников его поддерживают, насколько они свежие, есть ли противоречия. В минимальной версии достаточно уровней `high`, `medium`, `low`.

## Freshness

`last_verified` показывает, когда страница или утверждение последний раз подтверждались. Для быстро меняющихся тем stale-порог может быть 90 дней; для устойчивых концептов вроде [[Zettelkasten]] он может быть гораздо дольше.

## Supersession

Если новый источник обновляет старое утверждение, старое не надо молча удалять. Его нужно пометить как superseded и связать с новым утверждением. Это сохраняет историю знания.

## Forgetting

Не все факты должны оставаться в активном слое. Устаревшие или давно неиспользуемые наблюдения можно понижать в приоритете, архивировать или помечать как low-confidence.

## Typed relationships

Обычные wikilinks показывают связь, но не тип связи. Расширенный LLM Wiki может хранить отношения:

- `supports` - поддерживает утверждение;
- `contradicts` - противоречит;
- `extends` - расширяет базовую идею;
- `implements` - реализует концепт;
- `used_by` - используется чем-то;
- `supersedes` - заменяет старую версию.

## Конфликт в текущих источниках

Явного содержательного противоречия между источниками пока не найдено. Есть различие в акцентах:

- Karpathy предлагает minimal viable wiki с `raw/`, `wiki/`, schema, `index.md` и `log.md`.
- LLM Wiki v2 и техническая реализация Rangaprabhu добавляют lifecycle, graph, automation и quality controls.

Это не конфликт, а расширение: [[LLM Wiki]] может начинаться минимально и постепенно включать lifecycle-механику.

## Источники

- [raw/LLM Wiki v2 - extending Karpathy's LLM Wiki pattern with lessons from building agentmemory.md](../raw/LLM%20Wiki%20v2%20%E2%80%94%20extending%20Karpathy's%20LLM%20Wiki%20pattern%20with%20lessons%20from%20building%20agentmemory.md)
- [raw/Building my Personal LLM Wiki (Part 2) The Technical Implementation.md](<../raw/Building%20my%20Personal%20LLM%20Wiki%20(Part%202)%20The%20Technical%20Implementation.md>)
- [raw/llm-wiki.md](../raw/llm-wiki.md)

## Связи

- [[LLM Wiki]]
- [[LLM Wiki Workflow]]
- [[Obsidian]]
