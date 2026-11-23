
# Журнал изменений

Здесь записаны все заметные изменения проекта [AI-Demo](https://github.com/Starbugstone/AI-Demo).

## [1.1.0] - 2025-10-27
### Добавлено
- Новая песочница: клон Flappy Bird «Neon Pipelines» ([PR #4](https://github.com/Starbugstone/AI-Demo/pull/4)).
- Новая песочница: match-three игра «Cascade Candy Clash» с системой бонусов ([PR #5](https://github.com/Starbugstone/AI-Demo/pull/5)).
- Новая песочница: классический «Сапёр» (Minesweeper) ([PR #1](https://github.com/Starbugstone/AI-Demo/pull/1)).
- Визуальные подсказки (hinting) и улучшенные аркадные эффекты в match-three.
- Цепные взрывы бомб и взаимодействие бонусов (cross bonus, rainbow explosion) в «Cascade Candy Clash».

### Изменено
- Песочницы теперь корректно масштабируются в полноэкранном режиме (responsive fullscreen) ([PR #3](https://github.com/Starbugstone/AI-Demo/pull/3)).
- Улучшена графика, анимации и звуковое сопровождение в аркадных проектах.

### Исправлено
- Исправлена ошибка в проекте Aurora, где `RequestAnimationFrame` вызывался без привязки к объекту `window`.
- Исправлено масштабирование предпросмотра при переходе в полноэкранный режим.
- Исправлена логика сетки и drag-and-drop в match-three.
- Удалены неиспользуемые зависимости npm и скорректированы версии пакетов для стабильной сборки в Azure.

## [1.0.0] - 2025-10-23
### Добавлено
- Инициализация репозитория с базовыми демо-проектами и оболочкой галереи.
- Настроен CI-воркфлоу для автоматического развёртывания через Azure Static Web Apps.
