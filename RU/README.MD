# WiFi Spammer Tool || RU

![Bash](https://img.shields.io/badge/bash-v5.0%2B-blue) 
![License](https://img.shields.io/badge/license-MIT-green) 
![Platform](https://img.shields.io/badge/platform-Linux-lightgrey)

Скрипт для создания множества фейковых WiFi точек доступа с SSID

## 📝 Описание

Этот инструмент создает множество фейковых WiFi точек доступа для тестирования безопасности беспроводных сетей. 
Особенности:
- SSID популярных российских сетей
- Префиксы роутеров, распространенных в РФ
- Несколько режимов работы
- Автоматическое восстановление сети

## ⚙️ Требования

- Linux
- Беспроводной адаптер с поддержкой мониторного режима
- Root-доступ
- Пакеты: `aircrack-ng`, `iw`

## 📦 Установка

1. Установите зависимости:
```bash
sudo apt update && sudo apt install -y aircrack-ng iw
```

2. Скачайте скрипт:
```bash
git clone https://github.com/ars3nb/wifispam/RU.git
cd RU  # Русская версия
```

3. Дайте права на выполнение:
```bash
chmod +x wifi_spammer.sh
```

## 🚀 Использование

Запустите с root-правами:
```bash
sudo ./wifi_spammer.sh
```

Следуйте инструкциям на экране. Для остановки - Ctrl+C.

## 📂 Файлы конфигурации

- `popular.txt` - популярные SSID в России
- `router.txt` - префиксы роутеров
- `custom.txt` - ваши кастомные SSID

## ⚠️ Важно

Только для образовательных целей и тестирования собственных сетей!

## Особенности русской версии

- Все SSID в `popular.txt` и `router.txt` адаптированы под российских пользователей
