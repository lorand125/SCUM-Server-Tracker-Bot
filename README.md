# SCUM Server Tracker Bot

Бот для отслеживания онлайн игроков на сервере SCUM через анализ логов.

## 🌟 Особенности
- Отслеживание онлайн игроков в реальном времени
- REST API для интеграции с сайтами
- История за 24 часа и топ игроков
- Автоматическое определение перезапуска сервера
- Поддержка Windows и Linux

## 🚀 Быстрый старт

### Вариант 1: Docker (рекомендуется)
```bash
git clone https://github.com/lorand125/scum-server-tracker.git
cd scum-server-tracker
cp config.example.json config.json
# Отредактируйте config.json
docker-compose up -d
```

### Вариант 2: Установка вручную
```bash
git clone https://github.com/lorand125/scum-server-tracker.git
cd scum-server-tracker
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
cp config.example.json config.json
# Отредактируйте config.json
python scum_bot/bot.py
```
