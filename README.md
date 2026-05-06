<div align="center">

# 🎮 Hearts of Iron IV · DLC Unlocker for macOS

<img src="https://img.shields.io/badge/Platform-macOS-9cf?style=for-the-badge&logo=apple" alt="macOS">
<img src="https://img.shields.io/badge/CreamAPI-v5.3.0.0-ff69b4?style=for-the-badge" alt="CreamAPI">
<img src="https://img.shields.io/badge/Game-Hearts_of_Iron_IV-red?style=for-the-badge&logo=steam" alt="Hearts of Iron IV">

<br>
<br>

[![Русский](https://img.shields.io/badge/Русский-README-blue?style=flat-square)](README.md)
[![English](https://img.shields.io/badge/English-README_EN.md-blue?style=flat-square)](README_EN.md)

</div>

---

# 🇷🇺 Русская версия

## 🌟 Описание

> **Легальный разблокировщик DLC** для Steam-версии **Hearts of Iron IV** на macOS.  
> Работает через **CreamAPI v5.3.0.0** — не меняет файлы игры, только подменяет библиотеку Steam.

Этот инструмент позволяет разблокировать **все DLC** в лицензионной копии Hearts of Iron IV, приобретённой в Steam.  
Он подменяет оригинальную библиотеку `libsteam_api.dylib` на модифицированную версию CreamAPI, которая сообщает игре, что все DLC якобы уже куплены.

> ⚠️ **Важно:** Сам контент DLC (файлы `.dlc` и ассеты) должен физически находиться в папке игры. Этот инструмент только «включает» доступ к ним.

---

## 🔧 Как это работает

1. CreamAPI перехватывает вызовы Steam API
2. Игра «думает», что все DLC лицензионно приобретены
3. Вы запускаете HOI4 и получаете полный доступ к DLC

---

## 🙏 Благодарности

- **[deadmau5](https://cs.rin.ru/forum/viewtopic.php?f=29&t=70576)** — создатель **CreamAPI**
- **[KyLaEga](https://github.com/KyLaEga/EU4-DLC-Unlocker-macOS/tree/master)** — за предоставление файлов и основы для macOS

---

## 🚀 Инструкция по установке

### 1️⃣ Скачайте файлы
Склонируйте репозиторий или скачайте вручную:
- `cream_api.ini`
- `libsteam_api.dylib`

### 2️⃣ Переименуйте оригинальную библиотеку
Перейдите в папку с игрой (обычно `~/Library/Application Support/Steam/steamapps/common/Hearts of Iron IV/`).  
Найдите `libsteam_api.dylib` и переименуйте его в:

```bash
libsteam_api_o.dylib
```

### 3️⃣ Скопируйте новые файлы
Поместите скачанные `cream_api.ini` и `libsteam_api.dylib` в ту же папку.

### 4️⃣ Запустите игру
Через Steam или напрямую. Если macOS попросит разрешение — откройте **«Конфиденциальность и безопасность»** и разрешите запуск библиотеки.

> 🧠 **Совет:** При первом запуске может появиться предупреждение Gatekeeper — нажмите «Открыть всё равно» или разрешите в настройках.

---

## ✅ Требования

| Компонент                | Условие                                      |
|-------------------------|----------------------------------------------|
| macOS                   | 10.13 (High Sierra) или новее               |
| Hearts of Iron IV       | Лицензионная копия в Steam                   |
| DLC-контент             | Физические файлы DLC (должны быть в папке игры) |

---

## 💻 Поддерживаемые платформы

| Платформа            | Архитектура       | Статус                        |
|----------------------|-------------------|-------------------------------|
| macOS 10.13+         | Intel (x86_64)    | ✅ Полная поддержка           |
| macOS 11+            | Apple Silicon (M1/M2/M3/M4) | ✅ Полная поддержка (через Rosetta 2) |

> На Apple Silicon игра работает через Rosetta 2 — разблокировщик совместим.

---

## ❓ Частые вопросы

**Нужно ли отключать антивирус или SIP?**  
Нет, CreamAPI не требует отключения системной защиты.

**Бан в Steam?**  
Инструмент не взаимодействует с аккаунтом напрямую, но используйте на свой страх и риск.

**DLC не разблокируются?**  
Убедитесь, что файлы DLC лежат в `game/dlc/` или аналогичной папке.

---

## 📄 Лицензия

Проект распространяется в образовательных целях. Все права на CreamAPI принадлежат **deadmau5**.  
Hearts of Iron IV — торговая марка **Paradox Interactive**.

---
