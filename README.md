# Opus 5-5

Установщик локального шлюза Nova Code для NVIDIA NIM. Панель: ввод ключа и проверка подключения.

## macOS / Linux

```sh
curl -fsSL "https://raw.githubusercontent.com/kesha666-opt/opus-5-5/main/scripts/install.sh" | sh
```

## Windows PowerShell

```powershell
irm "https://raw.githubusercontent.com/kesha666-opt/opus-5-5/main/scripts/install.ps1" | iex
```

Установщик публичный. Приложение находится в приватном `kesha666-opt/nova-code-bridge`: для установки нужен вход в GitHub и разрешение владельца. GitHub CLI, uv/Python и Claude Code устанавливаются при необходимости.

После установки откроется http://127.0.0.1:8182/admin. Вставьте NVIDIA API key в панель, нажмите «Сохранить и проверить», затем запустите `fcc-claude`.

Существующий FCC, его настройки и порт 8082 не изменяются. Если команды FCC уже заняты, установщик остановится: используйте отдельного пользователя ОС. Настройки этой сборки — `~/.nova-code`.

Название Opus 5-5 обозначает установщик, а не модель Anthropic. Ответы генерирует NVIDIA NIM. Проект независимый, основан на Free Claude Code; см. LICENSE и NOTICE. Реальная генерация требует действительного ключа NVIDIA.
