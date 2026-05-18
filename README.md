# Rust Neurallog 🎯

**Rust Neurallog** — это продвинутый внешний анализатор боевых логов для игры Rust. Программа позволяет игрокам в режиме реального времени отслеживать свою эффективность, анализировать дистанции выстрелов и детально изучать распределение попаданий по частям тела.

[Русское описание находится ниже](#russian-description)

---

## 🚀 Key Features

*   **Real-time Combat Analysis**: Instantly displays damage dealt, distance to target, and hit areas.
*   **Accuracy Heatmap**: Integrated 2D silhouette visualizes your hit distribution (Head, Chest, Arms, Legs, etc.) based on all-time collected data.
*   **Player Database**: Save and alias encountered players by their SteamID to keep track of friends and foes.
*   **Overlay Mode**: Support for transparent overlay with adjustable opacity and "Click-Through" functionality.
*   **Auto-Update System**: The app automatically checks for the latest version to ensure compatibility and new features.
*   **Privacy & Safety**: Operates as a passive log reader.

## 🛠 How It Works (Technical Note)

Due to Rust's engine constraints, it is impossible to track every shot automatically without game memory injection (which is unsafe). 

**Rust Neurallog** works by:
1.  **Automatic Binding**: The app safely writes a command to your game's `keys.cfg`: `bind [key] consoletoggle;combatlog;consoletoggle`.
2.  **Log Activation**: When you press the hotkey, the game executes `combatlog`, writing recent encounter data to the disk.
3.  **Passive Parsing**: The program monitors the game's log file and displays it in a clean interface.

## 🛡 Security & Fairness

*   **No Memory Injection**: Unlike cheats, this software does not read or write to the game's memory.
*   **Passive Reader**: It only reads text files that the game itself generates.
*   **100% Safe**: Since it follows the same principle as simple log viewers, it is impossible to get banned (EAC/Facepunch). It does not interfere with any game processes.

---

<a name="russian-description"></a>
## 🇷🇺 Описание программы (Russian)

**Rust Neurallog** — это мощный инструмент для анализа боевой статистики в Rust. Он превращает сухие строчки консольных логов в наглядную графическую информацию, помогая вам лучше понимать свои ошибки и прогресс в стрельбе.

## ✨ Основные функции

*   **Анализ боя в реальном времени**: Вывод урона, дистанции и зон попадания сразу после выстрелов.
*   **Карта точности**: Визуализация распределения попаданий на силуэте человека. Учитываются все собранные данные за всё время использования.
*   **База игроков**: Возможность присваивать никнеймы игрокам по SteamID для быстрой идентификации в логах.
*   **Кастомизация**: Настройка прозрачности интерфейса и поддержка горячих клавиш.
*   **Авто-обновление**: Программа сама предложит установить актуальную версию при выходе патча.
*   **Полностью бесплатно**: Весь функционал доступен без подписок и скрытых платежей.

## ⚙️ Техническая часть

Из-за особенностей Rust, отслеживать выстрелы "на лету" без прямого вмешательства в игру невозможно. Наша программа использует легальный метод:
1.  **Создание бинда**: Программа автоматически прописывает команду в конфиг игры (`bind [клавиша] consoletoggle;combatlog;consoletoggle`).
2.  **Запись в лог**: При нажатии клавиши в игре выполняется команда `combatlog`, которая записывает данные боя в файл.
3.  **Отображение**: **Rust Neurallog** мгновенно считывает этот файл и выводит статистику на ваш экран.

## 🔒 Безопасность

*   **Без инъекций**: Программа не внедряется в процессы игры (DLL injection) и не читает память.
*   **Внешнее ПО**: Это просто красивый интерфейс для чтения текстовых файлов, которые игра сама создает на вашем диске.
*   **Бан невозможен**: Использование этого софта эквивалентно чтению консоли или текстового файла лога, что не запрещено правилами. Программа никак не влияет на процесс игры.

---

**Developed with ❤️ for the Rust Community.**
