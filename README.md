# Valeriy

**Безкоштовний Twitch-бот для Windows: команди, озвучення, донати, алерти, оверлеї для OBS і автоматизація.**
Українською та англійською.

[Завантажити останню версію](https://github.com/makulatura78/bot-valeriy-release/releases/latest/download/BotValeriyUiV2-win-Setup.exe) ·
[Сайт](https://bot-valeriy.com) ·
[Discord](https://discord.gg/KZKGwSbF4W) ·
[Усі релізи](https://github.com/makulatura78/bot-valeriy-release/releases) ·
[English](#english)

---

## Що це

Valeriy — програма для стримерів Twitch. Усе працює на твоєму комп'ютері: дії, змінні, оверлеї й налаштування зберігаються локально. Це програма, а не хмарний сервіс.

- **Автоматизація.** Дії з кроків (чат, озвучення, OBS, Twitch, змінні) з умовами, повторами й перемикачами. Запускаються тригерами (початок і кінець стріму, перше повідомлення, слово в чаті), за розкладом, коли запускається чи закривається гра, гарячою клавішею, командою, нагородою або через локальний API (наприклад, зі Stream Deck). Змінні на всіх і на кожного глядача, групи-вимикачі режимів, готові шаблони, історія запусків. Частковий імпорт зі Streamer.bot.
- **Чат і модерація.** Власні команди з тегами, кулдауни й аліаси, таймери, заборонені слова, фільтри чату, цитати, постійні глядачі, розіграші.
- **Озвучення.** Українські голоси працюють на твоєму ПК без інтернету (StyleTTS2, Supertonic). Для інших голосів можна підключити ElevenLabs, OpenAI, Gemini, Grok чи Edge зі своїм ключем. Голос для кожного глядача, черга озвучення, модерація.
- **Алерти й оверлеї.** Фолов, підписка, подарунки, рейд, бітси, викуп балів, донат: для кожної події свій текст, звук і голос. Редактор сцен для OBS (Browser Source), музика від глядачів із плеєром просто в OBS, окремі джерела звуку для озвучення й музики.
- **Донати.** Donatello (гривня без конвертацій): алерт, озвучення, подяка в чаті.
- **Дві мови.** Інтерфейс і відповіді бота українською чи англійською, мова обирається окремо для кожного.

## Встановлення

1. Завантаж [інсталятор](https://github.com/makulatura78/bot-valeriy-release/releases/latest/download/BotValeriyUiV2-win-Setup.exe) і запусти його.
2. На сторінці «Акаунт Twitch» увійди через Twitch.
3. У «Провайдерах AI і TTS» й «Озвучці й голосах» обери, чим і для кого озвучувати.
4. Натисни «Запустити».

Є також [портативна збірка](https://github.com/makulatura78/bot-valeriy-release/releases/latest/download/BotValeriyUiV2-win-Portable.zip): розпакуй у будь-яку теку й запусти `BotValeriyUiV2.exe` з неї.

**Вимоги:** Windows 10 або 11, 64-бітна. Окремо встановлювати .NET не потрібно.

## Оновлення

Програма оновлюється сама: при запуску вона перевіряє нову версію й пропонує встановити її (використовується [Velopack](https://velopack.io)). Ручне оновлення не потрібне.

Є два канали:

- **Стабільний.** Звичайні релізи (позначені як Latest). Типовий вибір.
- **Бета.** Попередні версії (позначені як Pre-release) з новими можливостями, які ще перевіряються на стрімах. Увімкни «Отримувати бета-версії» в «Налаштуваннях». Якщо вимкнути галочку, програма повернеться на стабільну версію.

## Файли в релізі

| Файл | Що це |
|---|---|
| `BotValeriyUiV2-win-Setup.exe` | Інсталятор стабільної версії |
| `BotValeriyUiV2-win-Portable.zip` | Портативна збірка стабільної версії |
| `BotValeriyUiV2-beta-Setup.exe`, `BotValeriyUiV2-beta-Portable.zip` | Те саме для бета-каналу |
| `*.nupkg`, `RELEASES`, `releases.*.json` | Службові файли для автоматичного оновлення; завантажувати вручну не потрібно |

## Де зберігаються дані

Налаштування, дії, змінні й оверлеї лежать у профілі користувача (`%LocalAppData%\BotValeriy`) і не залишають комп'ютер. Секрети (токени, ключі) шифруються засобами Windows.

## Допомога й зворотний зв'язок

- Питання, ідеї й помилки: [Discord](https://discord.gg/KZKGwSbF4W).
- Підтримати проєкт: [Donatello](https://donatello.to/zaddiros).
- Вихідний код зберігається в закритому репозиторії; цей репозиторій містить лише релізи.

---

## English

**A free Twitch bot for Windows: commands, text-to-speech, donations, alerts, OBS overlays and automation.** In Ukrainian and English.

[Download the latest version](https://github.com/makulatura78/bot-valeriy-release/releases/latest/download/BotValeriyUiV2-win-Setup.exe) ·
[Website](https://bot-valeriy.com/en) ·
[Discord](https://discord.gg/KZKGwSbF4W) ·
[All releases](https://github.com/makulatura78/bot-valeriy-release/releases)

### What it is

Valeriy is a program for Twitch streamers. Everything runs on your computer: actions, variables, overlays and settings are stored locally. It is an app, not a cloud service.

- **Automation.** Actions built from steps (chat, speech, OBS, Twitch, variables) with conditions, repeats and switches. Start them with triggers (stream start and end, a first message, a word in chat), a schedule, a game starting or closing, a hotkey, a command, a reward, or the local API (for example from Stream Deck). Global and per-viewer variables, group switches for modes, ready templates, run history. Partial import from Streamer.bot.
- **Chat and moderation.** Custom commands with tags, cooldowns and aliases, timers, banned words, chat filters, quotes, regular viewers, giveaways.
- **Text-to-speech.** Ukrainian voices run on your PC with no internet (StyleTTS2, Supertonic). For other voices you can connect ElevenLabs, OpenAI, Gemini, Grok or Edge with your own key. A voice per viewer, a speech queue, moderation.
- **Alerts and overlays.** Follow, sub, gifts, raid, bits, point redemption, donation: each event gets its own text, sound and voice. A scene editor for OBS (Browser Source), viewer song requests with a player right in OBS, separate audio sources for speech and music.
- **Donations.** Donatello (hryvnia with no conversion): an alert, speech, a thank-you in chat.
- **Two languages.** The interface and the bot's chat replies can each be Ukrainian or English, set separately.

### Install

1. Download the [installer](https://github.com/makulatura78/bot-valeriy-release/releases/latest/download/BotValeriyUiV2-win-Setup.exe) and run it.
2. Sign in with Twitch on the "Twitch account" page.
3. In "AI & TTS providers" and "Speech & voices" choose what speaks and for whom.
4. Press "Start".

A [portable build](https://github.com/makulatura78/bot-valeriy-release/releases/latest/download/BotValeriyUiV2-win-Portable.zip) is also available: unzip it anywhere and run `BotValeriyUiV2.exe` from it.

**Requirements:** Windows 10 or 11, 64-bit. You do not need to install .NET separately.

### Updates

The app updates itself: on start it checks for a new version and offers to install it (via [Velopack](https://velopack.io)). There are two channels:

- **Stable.** Regular releases (marked Latest). The default.
- **Beta.** Pre-releases (marked Pre-release) with new features still being tried on streams. Turn on "Receive beta versions" in "Settings". Turning it off returns you to the stable version.

### Files in a release

| File | What it is |
|---|---|
| `BotValeriyUiV2-win-Setup.exe` | Stable installer |
| `BotValeriyUiV2-win-Portable.zip` | Stable portable build |
| `BotValeriyUiV2-beta-Setup.exe`, `BotValeriyUiV2-beta-Portable.zip` | The same for the beta channel |
| `*.nupkg`, `RELEASES`, `releases.*.json` | Files used by automatic updates; you do not need to download them |

### Your data

Settings, actions, variables and overlays live in your user profile (`%LocalAppData%\BotValeriy`) and never leave your computer. Secrets (tokens, keys) are encrypted with Windows.

### Help and feedback

- Questions, ideas and bugs: [Discord](https://discord.gg/KZKGwSbF4W).
- Support the project: [Donatello](https://donatello.to/zaddiros).
- The source code is kept in a private repository; this repository only hosts releases.
