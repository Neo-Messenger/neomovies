# 🎬 Neo Movies

<div align="center">
  <img src="public/logo.png" alt="Neo Movies Logo" width="200"/>
  <p><strong>Современный онлайн-кинотеатр с удобным интерфейсом</strong></p>
</div>

## 📋 О проекте

Neo Movies - это современная веб-платформа для просмотра фильмов, построенная с использованием передовых технологий. Проект предлагает удобный интерфейс, быструю навигацию и множество функций для комфортного просмотра фильмов.

### ✨ Основные возможности

- 🎥 Три встроенных видеоплеера на выбор (Alloha, Collaps, Lumex)
- 🔍 Умный поиск по фильмам
- 📱 Адаптивный дизайн для всех устройств
- 🌙 Темная тема
- 👤 Система авторизации и профили пользователей
- ❤️ Возможность добавлять фильмы в избранное
- ⚡ Быстрая загрузка и оптимизированная производительность

## 🛠 Технологии

- **Frontend:**
  - Next.js 13+ (App Router)
  - React 18
  - TypeScript
  - Styled Components
  - NextAuth.js

- **Backend:**
  - Next.js
  - MongoDB
  - Mongoose

- **Дополнительно:**
  - ESLint
  - Prettier
  - Git
  - npm

## Начало работы

1. Клонируйте репозиторий:
```bash
git clone https://gitlab.com/foxixus/neomovies.git
cd neomovies
```

2. Установите зависимости:
```bash
npm install
```

3. Создайте файл `.env` и добавьте следующие переменные:
```env
# База данных MongoDB
MONGODB_URI=your_mongodb_uri

# NextAuth конфигурация
NEXTAUTH_SECRET=your_nextauth_secret
NEXTAUTH_URL=http://localhost:3000

# Google OAuth
GOOGLE_CLIENT_ID=your_google_client_id
GOOGLE_CLIENT_SECRET=your_google_client_secret

# Email конфигурация (для подтверждения регистрации)
GMAIL_USER=your_gmail@gmail.com
GMAIL_APP_PASSWORD=your_app_specific_password

NEXT_PUBLIC_API_URL=https://neomovies-api.vercel.app

# JWT конфигурация
JWT_SECRET=your_jwt_secret

# Lumex Player URL
NEXT_PUBLIC_LUMEX_URL=your_lumex_player_url
```


4. **Запустите проект:**
```bash
# Режим разработки
npm run dev

# Сборка для продакшена
npm run build
npm start
```
Приложение будет доступно по адресу [http://localhost:3000](http://localhost:3000)

## API

Приложение использует отдельный API сервер. API предоставляет следующие возможности:

- Поиск фильмов и сериалов
- Получение детальной информации о фильме/сериале
- Оптимизированная загрузка изображений
- Кэширование запросов

### Google OAuth
1. Перейдите в [Google Cloud Console](https://console.cloud.google.com/)
2. Создайте новый проект
3. Включите Google OAuth API
4. Создайте учетные данные OAuth 2.0
5. Добавьте разрешенные URI перенаправления:
   - http://localhost:3000/api/auth/callback/google
   - https://your-domain.com/api/auth/callback/google

### Gmail App Password
1. Включите двухфакторную аутентификацию в аккаунте Google
2. Перейдите в настройки безопасности
3. Создайте пароль приложения
4. Используйте этот пароль в GMAIL_APP_PASSWORD

## Структура проекта

```
neomovies/
├── src/
│   ├── app/            # App Router pages
│   ├── components/     # React компоненты
│   ├── hooks/          # React хуки
│   ├── lib/           # Утилиты и API
│   ├── models/        # MongoDB модели
│   └── styles/        # Глобальные стили
├── public/            # Статические файлы
└── package.json

```

## 👥 Авторы

- **Frontend Developer** - [Foxix](https://gitlab.com/foxixus)

## 📄 Лицензия

Этот проект распространяется под лицензией Apache-2.0. Подробности в файле [LICENSE](LICENSE).

## 🤝 Участие в проекте

Мы приветствуем любой вклад в развитие проекта! Если у вас есть предложения по улучшению:

1. Форкните репозиторий
2. Создайте ветку для ваших изменений
3. Внесите изменения
4. Отправьте pull request


## Благодарности

- [TMDB](https://www.themoviedb.org/) за предоставление API
- [Vercel](https://vercel.com/) за хостинг API

## 📞 Контакты

Если у вас возникли вопросы или предложения, свяжитесь с нами:
- Email: neo.movies.mail@gmail.com
- Telegram: @foxix_us

---

<div align="center">
  <p>Made with ❤️ by Foxix</p>
</div>
