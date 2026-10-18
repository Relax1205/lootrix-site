# Сайт Lootrix (публичная часть)

Всё в этой папке можно показывать всем: страница игры и политика конфиденциальности.
Ссылка на политику нужна в Google Play Console (Policy → App content → Privacy policy) и есть в игре
(Профиль → «Конфиденциальность», адрес задан в `FEEDBACK.privacy` в `prototype/js/extras.js`).

## Как опубликовать

Основной репозиторий закрытый, а GitHub Pages для закрытых репозиториев платный.
Поэтому сайт живёт в отдельном публичном репозитории `lootrix-site`:

1. На GitHub: New repository → имя `lootrix-site`, Public, без README.
2. Один раз: `git remote add site https://github.com/Relax1205/lootrix-site.git`
3. Отправить папку: `npm run site` (это `git subtree push --prefix site site main`).
4. В `lootrix-site` на GitHub: Settings → Pages → Branch `main`, папка `/ (root)` → Save.

Через минуту сайт будет по адресу https://relax1205.github.io/lootrix-site/ ,
политика — https://relax1205.github.io/lootrix-site/privacy.html .

## Что поправить, когда появится

- Почта: lootrix1096@gmail.com (элементы `class="mail"` в `index.html` и `privacy.html`).
- Ссылка на Google Play: кнопка `btn off` в `index.html`.
- Если реклама или аналитика будут другими (не Яндекс Медиация, не Firebase) — поправить разделы политики.
