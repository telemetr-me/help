# Правила для ИИ-агентов

- Тексты на русском, для пользователей Telemetr, без канцелярита.
- Адреса страниц не менять: на них ссылаются сайт telemetr.me и поисковики. Если страницу всё же нужно переименовать, добавить переадресацию в `redirects` в `docs.json`.
- Новая страница: файл `<раздел>/<адрес>.mdx` с `title` (и при желании `description`) в шапке, плюс строка в `navigation` в `docs.json`. Если для её адреса была переадресация, удалить её.
- Картинки класть в `images/<раздел>/`, не больше 20 МБ.
- Видео — Kinescope, VK Видео или Rutube через iframe. Kinescope вставлять так:

```mdx
<iframe
  className="w-full aspect-video rounded-xl"
  src="https://kinescope.io/embed/<id>"
  title="Видео"
  allow="autoplay; fullscreen; picture-in-picture; encrypted-media; gyroscope; accelerometer; clipboard-write; screen-wake-lock"
  allowFullScreen
/>
```

- Подсказки — компоненты Mintlify `<Info>`, `<Warning>`, `<Tip>`.
- Перед коммитом: `mint validate` и `mint broken-links`.
