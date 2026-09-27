# Free Skills

## Направления

- [Разработка](skills/development/) — пять ролей для работы над программным продуктом: от постановки задачи до финального аудита PR.
- [Motion-видео](skills/motion-video/SKILL.md) — быстрый старт агента: [инструменты и установка](skills/motion-video/SETUP.md), [возможности для пользователя](skills/motion-video/CAPABILITIES.md).

## Разработка

Это копии рабочих Skill-файлов, подготовленные для отдельного использования.

Короткая схема работы ролей и настройка GitHub — в [AGENTS.md](AGENTS.md).

| Роль | Когда подключать | Результат |
| --- | --- | --- |
| [Product Manager](skills/development/product-manager/SKILL.md) | Новая или крупная продуктовая задача | Целостная логика в `docs/product.md` и draft PR |
| [Tech Lead](skills/development/tech-lead/SKILL.md) | Есть продуктовая постановка; нужно определить реализацию | Техническое задание и разбиение на PR |
| [Developer](skills/development/developer/SKILL.md) | Техническое задание утверждено | Код текущего этапа |
| [Code Reviewer](skills/development/code-reviewer/SKILL.md) | Код готов | Проверка и исправление связанных с задачей дефектов |
| [Logic Auditor](skills/development/logic-auditor/SKILL.md) | PR прошёл ревью | Финальная проверка логики, только обязательные замечания |

## Как использовать

1. Скопируйте `skills/development/` в `skills/development/` своего репозитория. Копируйте папки ролей целиком: `self-review.md` и `modes/` относятся к соответствующим Skill.
2. Скопируйте файлы из `.codex/agents/` в `.codex/agents/` своего репозитория. В них указано, какой Skill читает каждая роль.
3. Для Product Manager и Tech Lead используйте `docs/product.md` как общую продуктовую постановку. Если у проекта другой путь, измените его в Skill-файлах перед запуском.
4. Подключите доступ к своему репозиторию GitHub, если хотите, чтобы роли создавали ветки, PR и комментарии. Без этого адаптируйте шаги работы с GitHub под свои инструменты.

При переносе цепочки в свой проект добавьте правила из `AGENTS.md` к уже действующим инструкциям проекта.

Для небольшой задачи с уже описанной продуктовой логикой можно начать с Tech Lead. Для новой или меняющей поведение продукта задачи сначала используйте Product Manager. Дальше цепочка: Tech Lead → Developer → Code Reviewer → Logic Auditor.

Эти Skill задают обязанности и границы ролей. Модели и способ запуска выбирайте в своём окружении.

## Motion-видео

Скопируйте `skills/motion-video/` в проект. Агент читает [SKILL.md](skills/motion-video/SKILL.md), проверяет систему по [SETUP.md](skills/motion-video/SETUP.md), готовит нужный стек и сразу предлагает человеку понятное [меню возможностей](skills/motion-video/CAPABILITIES.md). Для JS/TS-ролика нужны Node.js, FFmpeg/ffprobe и один движок; Python, Blender и внешние каталоги добавляются по задаче. В таблице Skill указано, за что отвечает каждый инструмент.
