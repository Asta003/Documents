# Как добавить новый проект в песочницу

## Предусловия

- Node.js версии 18 или новее установлен
- Репозиторий клонирован и зависимости установлены (`npm install`)
- Локальный сервер разработки запускается без ошибок (`npm run dev`)
- Готов HTML/JS-код эксперимента, который нужно опубликовать

## Шаги

1. Создайте папку для нового проекта в каталоге `projects/`.

2. Перейдите в созданную папку.
   
3. Создайте файл `index.html`:
   
4. Откройте `index.html` и добавьте базовую разметку:
   ```
   Shift + 1
   ```

5. Создайте файл `script.js`со следующим содержимым:
   ```
   const root = document.currentScript.getRootNode();
   const heading = root.querySelec ('h1');
   heading.textContent = 'Работает!';
   ```

6. Создайте файл метаданных `project.yaml` c примером содержимого:
   ```
   slug: particle-playground
   name: Particle Playground
   summary: Cinematic particles flow across a dynamic vector field with responsive pointer magnetism.
   agents:
   - Codex GPT-5
   - Visualizer Bot
   status: prototype
   tags:
   - canvas
   - interactive
   - shaders
   entry: index.html
   order: 20
   ```

7. Сохраните все файлы и вернитесь в корень репозитория:
   ```
   cd ../..
   ```

8. Перезапустите сервер:
   ```
   npm run dev
   ```

## Результат

Откройте браузер по выведенному адресу  (Например: http://localhost:5173).

В боковой панели появится новый пункт My Experiment. При клике на него в песочнице отобразится заголовок «Работает!» — это значит, что скрипт выполнился внутри изолированного Shadow DOM.

Если проекта нет в списке — проверьте, что project.yaml лежит строго в папке projects/my-experiment/, а не уровнем выше.

## Что дальше

- [Что такое Shadow DOM-песочница](concept.md) — почему проекты изолированы и как это работает
- [Техническое описание архитектуры](tech-readme.md) — как устроен Vite-плагин и

