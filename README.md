## Обоснование решения
Для реализации микрофронтендов выбран module federation т.к. изначально не было предъявлено требование о поддержке нескольких фреймворков, что могло бы послужить обоснованием для выбора single-spa.

## Концепт разделения на модули
Считаем что корневой директорией выбран frontend
```
/host               # Хост-приложение
│   ├── /src
│   ├── webpack.config.js
│   └── package.json
├── /profile-module     # Модуль для профиля
│   ├── /src
│   │   ├── Profile.js
│   │   ├── EditProfile.js
│   │   └── styles.css
│   ├── webpack.config.js
│   └── package.json
├── /gallery-module     # Модуль для галереи (загрузка/удаление фото)
│   ├── /src
│   │   ├── Gallery.js
│   │   ├── PhotoCard.js
│   │   └── styles.css
│   ├── webpack.config.js
│   └── package.json
├── /likes-module       # Модуль для лайков
│   ├── /src
│   │   ├── LikeButton.js
│   │   ├── LikesCounter.js
│   │   └── styles.css
│   ├── webpack.config.js
│   └── package.json
```
## Disclaimer
Я не владею JS в должной мере, концепцию модульности понимаю)
