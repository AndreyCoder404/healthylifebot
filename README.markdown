# HealthyLifeBot

![CI/CD](https://github.com/AndreyCoder404/healthylifebot/actions/workflows/ci.yml/badge.svg)
![License](https://img.shields.io/badge/license-MIT-blue.svg)
![GitHub Issues](https://img.shields.io/github/issues/AndreyCoder404/healthylifebot)

HealthyLifeBot — это Telegram-приложение, которое помогает пользователям вести здоровый образ жизни и развиваться через персонализированные рекомендации. Проект объединяет питание, тренировки и саморазвитие в одном месте, используя нейросети для адаптации под каждого пользователя.

## 📜 Описание проекта

### Суть проекта
HealthyLifeBot предоставляет три ключевые функции:
1. **Здоровое питание**:
   - Персонализированные рецепты с расчётом БЖУ, калорий и способов приготовления.
   - Калькулятор затрат: сравнение стоимости домашней еды, кафе и замороженной пищи.
   - Рекомендации по витаминам и добавкам (с учётом региона, возраста, пола).
2. **Физическая активность**:
   - Программы тренировок (набор массы, сушка, рельеф) с видеоуроками.
   - Рекомендации по дням и группам мышц (с учётом уровня подготовки).
3. **Саморазвитие**:
   - Библиотека подкастов и книг (философия, стоицизм, буддизм).
   - Возможность загрузки пользовательских материалов (PDF, MP3).
   - Персонализированные рекомендации.

### Идея и перспектива
HealthyLifeBot — это единое решение для тех, кто хочет заботиться о своём здоровье и развитии. Перспектива проекта:
- Расширение до полноценного приложения с интеграцией в другие платформы (iOS, Android).
- Монетизация через подписку на премиум-функции (например, персональный коучинг).
- Создание сообщества вокруг здорового образа жизни.

### Польза
- **Для пользователей**: Экономия времени и денег (калькулятор затрат), персонализированные рекомендации, доступ к полезным ресурсам.
- **Для разработчиков**: Возможность развивать навыки в работе с Telegram, нейросетями, API и микросервисной архитектурой.

## 🛠 Технологии и навыки

Проект использует современный технологический стек:
- **Языки программирования**: Python (Telegram-бот), Go (REST API), JavaScript (мини-приложение).
- **Фреймворки**: Flask (сервер), React (Telegram Web App).
- **Базы данных**: SQLite (MVP), PostgreSQL (масштабирование).
- **API и сервисы**:
  - Telegram Bot API и Web App API.
  - OpenAI API (персонализация).
  - Edamam API (рецепты и БЖУ).
  - YouTube API (видеоуроки).
  - AWS S3 (хранение файлов).
- **Инструменты DevOps**: Docker, Docker Compose, GitHub Actions (CI/CD), Kubernetes (в будущем).
- **Дополнительно**: REST API, HTTP, JSON, YAML, Swagger (документация API).

## 🚀 Установка и запуск

### Требования
- Python 3.9+
- Go 1.18+
- Docker
- Telegram-аккаунт

### Пошаговая инструкция
1. **Клонируйте репозиторий**:
   ```bash
   git clone https://github.com/AndreyCoder404/healthylifebot.git
   cd healthylifebot
   ```
2. **Установите зависимости**:
   - Для Python:
     ```bash
     pip install -r requirements.txt
     ```
   - Для Go (для мини-проектов):
     ```bash
     go mod download
     ```
3. **Настройте окружение**:
   - Создайте файл `.env`:
     ```env
     TELEGRAM_TOKEN=your_bot_token
     OPENAI_API_KEY=your_openai_key
     ```
   - Получите `TELEGRAM_TOKEN` через [BotFather](https://t.me/BotFather).
4. **Запустите с помощью Docker**:
   ```bash
   docker-compose up --build
   ```
5. **Проверьте работу**:
   - Откройте Telegram, найдите вашего бота и отправьте команду `/start`.

## 📂 Структура проекта

Проект состоит из нескольких мини-проектов, каждый из которых находится в отдельном репозитории:
- [recipe-db](https://github.com/AndreyCoder404/recipe-db): База рецептов (Go, PostgreSQL, REST API).
- [recipe-bot](https://github.com/AndreyCoder404/recipe-bot): Telegram-бот для рецептов (Python).
- [workout-db](https://github.com/AndreyCoder404/workout-db): База тренировок (Go, PostgreSQL).
- [workout-bot](https://github.com/AndreyCoder404/workout-bot): Telegram-бот для тренировок (Python).
- [podcast-lib](https://github.com/AndreyCoder404/podcast-lib): Библиотека подкастов (Go, PostgreSQL).
- [podcast-bot](https://github.com/AndreyCoder404/podcast-bot): Telegram-бот для подкастов (Python).

Основной репозиторий (`healthylifebot`) объединяет все компоненты.

## 🤝 Приглашение к разработке

HealthyLifeBot — это open-source проект, и я приглашаю разработчиков присоединиться! Мы будем рады вашему вкладу, если у вас есть навыки в:
- Python, Go, JavaScript (React).
- Работа с Telegram Bot API, REST API, нейросетями.
- DevOps (Docker, Kubernetes, CI/CD).

### Как внести вклад
1. Форкните репозиторий.
2. Создайте ветку для вашей фичи (`git checkout -b feature/your-feature`).
3. Сделайте коммит (`git commit -m "Add your feature"`).
4. Отправьте изменения (`git push origin feature/your-feature`).
5. Создайте Pull Request.

Подробности в [CONTRIBUTING.md](CONTRIBUTING.md).

## 📜 Правообладание и лицензия

© 2025 AndreyCoder404. Все права защищены.

Проект распространяется под лицензией MIT. Вы можете использовать код, но обязаны указывать авторство. Коммерческое использование без письменного разрешения автора запрещено. Подробности в [LICENSE](LICENSE).

## 📬 Контакты

- GitHub: [AndreyCoder404](https://github.com/AndreyCoder404)
- Telegram: @AndreyCoder404

Присоединяйтесь к HealthyLifeBot и давайте сделаем мир здоровее и счастливее вместе! 🚀