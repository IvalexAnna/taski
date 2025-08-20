# Taski

Приложение для планирования и управления задачами с современным веб-интерфейсом.

## 📋 Описание

Taski - это полнофункциональное веб-приложение для управления задачами, построенное на архитектуре Django + React. Приложение позволяет создавать, редактировать, удалять и отмечать задачи как выполненные.

## 🏗️ Архитектура

Проект состоит из двух основных частей:
- **Backend**: Django REST API с SQLite базой данных
- **Frontend**: React приложение с Bootstrap для стилизации

## 🚀 Технологии

### Backend
- **Django 3.2.3** - веб-фреймворк
- **Django REST Framework 3.12.4** - API фреймворк
- **Django CORS Headers 3.13.0** - поддержка CORS
- **SQLite** - база данных

### Frontend
- **React 18.2.0** - JavaScript библиотека
- **Bootstrap 5.2.3** - CSS фреймворк
- **Reactstrap 9.1.5** - Bootstrap компоненты для React
- **Axios 1.2.1** - HTTP клиент

## 📁 Структура проекта

```
taski/
├── backend/                 # Django backend
│   ├── api/                # API приложение
│   │   ├── models.py       # Модель Task
│   │   ├── views.py        # API views
│   │   ├── serializers.py  # Сериализаторы
│   │   └── migrations/     # Миграции БД
│   ├── backend/            # Основные настройки Django
│   ├── manage.py           # Django management
│   └── requirements.txt    # Python зависимости
├── frontend/               # React frontend
│   ├── src/
│   │   ├── components/     # React компоненты
│   │   │   ├── Task.js     # Компонент задачи
│   │   │   ├── TaskEditModal.js # Модальное окно редактирования
│   │   │   └── TabList.js  # Список вкладок
│   │   └── App.js          # Главный компонент
│   ├── package.json        # Node.js зависимости
│   └── public/             # Статические файлы
└── README.md
```

## ⚙️ Установка и запуск

### Предварительные требования
- Python 3.7+
- Node.js 14+
- npm или yarn

### Backend (Django)

1. Перейдите в папку backend:
```bash
cd backend
```

2. Создайте виртуальное окружение:
```bash
python -m venv venv
```

3. Активируйте виртуальное окружение:
```bash
# Windows
venv\Scripts\activate

# Linux/Mac
source venv/bin/activate
```

4. Установите зависимости:
```bash
pip install -r requirements.txt
```

5. Выполните миграции:
```bash
python manage.py migrate
```

6. Создайте суперпользователя (опционально):
```bash
python manage.py createsuperuser
```

7. Запустите сервер:
```bash
python manage.py runserver
```

Backend будет доступен по адресу: http://127.0.0.1:8000

### Frontend (React)

1. Перейдите в папку frontend:
```bash
cd frontend
```

2. Установите зависимости:
```bash
npm install
```

3. Запустите приложение:
```bash
npm start
```

Frontend будет доступен по адресу: http://localhost:3000

## 🔧 API Endpoints

- `GET /api/tasks/` - получить список всех задач
- `POST /api/tasks/` - создать новую задачу
- `GET /api/tasks/{id}/` - получить задачу по ID
- `PUT /api/tasks/{id}/` - обновить задачу
- `DELETE /api/tasks/{id}/` - удалить задачу

## 📱 Функциональность

- ✅ Создание новых задач
- ✏️ Редактирование существующих задач
- 🗑️ Удаление задач
- ☑️ Отметка задач как выполненных
- 🔄 Переключение между активными и выполненными задачами
- 📱 Адаптивный дизайн для мобильных устройств

## 🎨 Особенности интерфейса

- Современный и чистый дизайн с использованием Bootstrap
- Модальные окна для создания и редактирования задач
- Вкладки для переключения между активными и выполненными задачами
- Адаптивная верстка для различных размеров экрана

## 🧪 Тестирование

### Backend тесты
```bash
cd backend
python manage.py test
```

### Frontend тесты
```bash
cd frontend
npm test
```

## 📦 Сборка для продакшена

### Frontend
```bash
cd frontend
npm run build
```

## 🤝 Вклад в проект

1. Форкните репозиторий
2. Создайте ветку для новой функции
3. Внесите изменения
4. Создайте Pull Request

## 📄 Лицензия

Этот проект распространяется под лицензией, указанной в файле LICENSE.


**Автор:** Ivanova Anna
