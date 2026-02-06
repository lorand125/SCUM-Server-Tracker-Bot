# 🎮 SCUM Server Tracker Bot

[![Python Version](https://img.shields.io/badge/python-3.9+-blue.svg)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Docker](https://img.shields.io/badge/docker-available-blue.svg)](https://www.docker.com/)

Бот для отслеживания онлайн игроков на сервере SCUM через анализ логов в реальном времени.

![SCUM Tracker Demo](https://via.placeholder.com/800x400.png?text=SCUM+Tracker+Demo)

## ✨ Возможности

- ✅ **Отслеживание онлайн игроков** в реальном времени
- ✅ **REST API** для интеграции с сайтами и панелями управления
- ✅ **История онлайна** за 24 часа с графиками
- ✅ **Топ игроков** по времени в игре
- ✅ **Автоопределение перезапуска** сервера
- ✅ **Поддержка Windows, Linux, Docker**
- ✅ **CIFS/SMB монтирование** для удаленных логов
- ✅ **Автосохранение** данных каждые 5 минут

## 🚀 Быстрый старт

### Способ 1: Docker (рекомендуется)

```bash
# Клонируем репозиторий
git clone https://github.com/yourusername/scum-server-tracker.git
cd scum-server-tracker

# Настраиваем конфигурацию
cp config.example.json config.json
nano config.json  # отредактируйте путь к логам

# Запускаем через Docker Compose
docker-compose up -d

# Проверяем работу
curl http://localhost:5001/api/health
```
### Способ 2: Прямая установка (Python)
```bash
# Клонируем репозиторий
git clone https://github.com/yourusername/scum-server-tracker.git
cd scum-server-tracker

# Создаем виртуальное окружение
python3 -m venv venv
source venv/bin/activate  # или venv\Scripts\activate на Windows

# Устанавливаем зависимости
pip install -r requirements.txt

# Настраиваем конфигурацию
cp config.example.json config.json
# Отредактируйте config.json, указав путь к логам SCUM

# Запускаем бота
python run.py
```
