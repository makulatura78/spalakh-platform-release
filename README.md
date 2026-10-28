# Spalakh Platform

**Безкоштовна програма для стримерів на Windows: чат-бот, озвучення, донати, алерти, оверлеї для OBS і автоматизація.**
Twitch, а також чати Kick, YouTube і TikTok. Українською та англійською.

[Завантажити](https://github.com/makulatura78/spalakh-platform-release/releases/latest) ·
[Сайт](https://bot-valeriy.com) ·
[Discord](https://discord.gg/KZKGwSbF4W) ·
[Усі релізи](https://github.com/makulatura78/spalakh-platform-release/releases) ·
[English](#english)

---

## Що це

Spalakh (раніше Bot Valeriy) — програма для стримерів. Усе працює на твоєму комп'ютері: дії, змінні, оверлеї й налаштування зберігаються локально. Це програма, а не хмарний сервіс.

- **Автоматизація.** Дії з кроків (чат, озвучення, OBS, Twitch, змінні, світло, VTube Studio, Voicemod, WebSocket) з умовами, повторами й перемикачами. Запускаються тригерами (стрім, чат, події каналу, прогнози, модерація, файли, вебхуки, VTube Studio), за розкладом, коли запускається гра, гарячою клавішею, командою, нагородою, з мобільної панелі на телефоні або через локальний API (наприклад, зі Stream Deck). Кнопка ▶ перевіряє тригер на зразковій події. Модулі на JavaScript, Lua чи Python. Частковий імпорт зі Streamer.bot.
- **Чат і модерація.** Twitch, Kick, YouTube і TikTok в одному місці. Власні команди з тегами, кулдауни й аліаси, таймери, заборонені слова, фільтри чату, журнал модерації, цитати, постійні глядачі, розіграші.
- **Озвучення.** Українські голоси працюють на твоєму ПК без інтернету (StyleTTS2, Supertonic). Для інших голосів можна підключити ElevenLabs, OpenAI, Gemini, Grok чи Edge зі своїм ключем. Голос для кожного глядача, черга озвучення, модерація.
- **Алерти й оверлеї.** Фолов, підписка, подарунки, рейд, бітси, викуп балів, донат: для кожної події свій текст, звук і голос. Редактор сцен для OBS (Browser Source), теми оверлеїв одним файлом, «Зараз грає», мета, таймер, колесо, титри, музика від глядачів.
- **Стрім-сетап.** OBS, VTube Studio, світло Elgato Key Light і Philips Hue, Voicemod — з дій і з вкладок ручного керування.
- **Донати.** Donatello і donatik: алерт, озвучення, подяка в чаті.
- **Дві мови й теми.** Інтерфейс і відповіді бота українською чи англійською, окремо для кожного. Темна й світла тема.

## Встановлення

1. Відкрий [останній реліз](https://github.com/makulatura78/spalakh-platform-release/releases/latest), завантаж `Spalakh-stable-Setup.exe` і запусти.
2. «Підключення» → «Акаунти» → «Увійти через Twitch». Там же Kick, YouTube і TikTok.
3. На сторінці «TTS» обери голос, в «Озвучці й голосах» — кому можна озвучувати.
4. Натисни «Запустити».

Є також портативна збірка `Spalakh-stable-Portable.zip`: розпакуй у будь-яку теку й запусти `Spalakh.exe` з неї.

Поки не вийшов перший стабільний Spalakh, стабільний інсталятор ще називається `BotValeriyUiV2-win-Setup.exe`: він поставить Bot Valeriy, а та з першим оновленням перейде на Spalakh сама.

**Вимоги:** Windows 10 або 11, 64-бітна. Окремо встановлювати .NET не потрібно.

## Оновлення

Програма оновлюється сама: при запуску перевіряє нову версію й пропонує встановити її ([Velopack](https://velopack.io)).

- **Стабільний канал.** Звичайні релізи (позначені як Latest). Типовий вибір.
- **Бета.** Попередні версії (Pre-release) з новими можливостями, які ще перевіряються на стрімах. Увімкни «Отримувати бета-версії» в «Налаштуваннях»; зняв галочку — програма повернеться на стабільну версію.

**З Bot Valeriy на Spalakh.** Якщо в тебе стоїть стара Bot Valeriy, нічого робити не треба: після оновлення вона сама поставить Spalakh, перенесе налаштування, дії, сцени й голоси і видалиться. Далі запускай Spalakh. Портативну копію Bot Valeriy заміни новою вручну.

## Файли в релізі

| Файл | Що це |
|---|---|
| `Spalakh-stable-Setup.exe` | Інсталятор стабільної версії |
| `Spalakh-stable-Portable.zip` | Портативна збірка стабільної версії |
| `Spalakh-preview-Setup.exe`, `Spalakh-preview-Portable.zip` | Те саме для бети |
| `BotValeriyUiV2-*` | Старий пакет Bot Valeriy: через нього старі встановлення переходять на Spalakh. Завантажувати не потрібно |
| `*.nupkg`, `RELEASES*`, `releases.*.json` | Службові файли для автоматичного оновлення |

## Де зберігаються дані

Налаштування, дії, змінні й оверлеї лежать у профілі користувача (`%LocalAppData%\Spalakh`) і не залишають комп'ютер. Після переходу з Bot Valeriy стара тека `%LocalAppData%\BotValeriy` лишається як резервна копія. Секрети (токени, ключі) шифруються засобами Windows.

## Допомога й зворотний зв'язок

- Питання, ідеї й помилки: [Discord](https://discord.gg/KZKGwSbF4W).
- Підтримати проєкт: [Donatello](https://donatello.to/zaddiros).
- Вихідний код зберігається в закритому репозиторії; цей репозиторій містить лише релізи.

---

## English

**A free streaming app for Windows: a chat bot, text-to-speech, donations, alerts, OBS overlays and automation.**
Twitch, plus Kick, YouTube and TikTok chat. In Ukrainian and English.

[Download](https://github.com/makulatura78/spalakh-platform-release/releases/latest) ·
[Website](https://bot-valeriy.com/en) ·
[Discord](https://discord.gg/KZKGwSbF4W) ·
[All releases](https://github.com/makulatura78/spalakh-platform-release/releases)

### What it is

Spalakh (formerly Bot Valeriy) is an app for streamers. Everything runs on your computer: actions, variables, overlays and settings are stored locally. It is an app, not a cloud service.

- **Automation.** Actions built from steps (chat, speech, OBS, Twitch, variables, lights, VTube Studio, Voicemod, WebSocket) with conditions, repeats and switches. Start them with triggers (stream, chat, channel events, predictions, moderation, files, webhooks, VTube Studio), a schedule, a game starting, a hotkey, a command, a reward, the mobile panel on your phone, or the local API (for example from Stream Deck). The ▶ button tests a trigger on a sample event. Modules in JavaScript, Lua or Python. Partial import from Streamer.bot.
- **Chat and moderation.** Twitch, Kick, YouTube and TikTok in one place. Custom commands with tags, cooldowns and aliases, timers, banned words, chat filters, a moderation log, quotes, regular viewers, giveaways.
- **Text-to-speech.** Ukrainian voices run on your PC with no internet (StyleTTS2, Supertonic). For other voices you can connect ElevenLabs, OpenAI, Gemini, Grok or Edge with your own key. A voice per viewer, a speech queue, moderation.
- **Alerts and overlays.** Follow, sub, gifts, raid, bits, point redemption, donation: each event gets its own text, sound and voice. A scene editor for OBS (Browser Source), overlay themes as one file, Now Playing, goal, timer, wheel, credits, viewer song requests.
- **Stream setup.** OBS, VTube Studio, Elgato Key Light and Philips Hue lights, Voicemod — from actions and from manual control tabs.
- **Donations.** Donatello and donatik: an alert, speech, a thank-you in chat.
- **Two languages and themes.** The interface and the bot's replies can each be Ukrainian or English. Dark and light theme.

### Install

1. Open the [latest release](https://github.com/makulatura78/spalakh-platform-release/releases/latest), download `Spalakh-stable-Setup.exe` and run it.
2. Connections → Accounts → Sign in with Twitch. Kick, YouTube and TikTok are there too.
3. Pick a voice on the TTS page, and who may use speech on Speech & voices.
4. Press Start.

A portable build `Spalakh-stable-Portable.zip` is also available: unzip it anywhere and run `Spalakh.exe` from it.

Until the first stable Spalakh is out, the stable installer is still called `BotValeriyUiV2-win-Setup.exe`: it installs Bot Valeriy, which moves to Spalakh by itself with its first update.

**Requirements:** Windows 10 or 11, 64-bit. You do not need to install .NET separately.

### Updates

The app updates itself: on start it checks for a new version and offers to install it ([Velopack](https://velopack.io)).

- **Stable.** Regular releases (marked Latest). The default.
- **Beta.** Pre-releases with new features still being tried on streams. Turn on "Receive beta versions" in Settings; turning it off returns you to the stable version.

**From Bot Valeriy to Spalakh.** If you have the old Bot Valeriy, there is nothing to do: after an update it installs Spalakh itself, moves your settings, actions, scenes and voices over and removes itself. Start Spalakh from then on. Replace a portable Bot Valeriy copy with the new one by hand.

### Files in a release

| File | What it is |
|---|---|
| `Spalakh-stable-Setup.exe` | Stable installer |
| `Spalakh-stable-Portable.zip` | Stable portable build |
| `Spalakh-preview-Setup.exe`, `Spalakh-preview-Portable.zip` | The same for the beta |
| `BotValeriyUiV2-*` | The old Bot Valeriy package, which moves old installs over to Spalakh. No need to download it |
| `*.nupkg`, `RELEASES*`, `releases.*.json` | Files used by automatic updates |

### Your data

Settings, actions, variables and overlays live in your user profile (`%LocalAppData%\Spalakh`) and never leave your computer. After moving from Bot Valeriy, the old `%LocalAppData%\BotValeriy` folder stays as a backup. Secrets (tokens, keys) are encrypted with Windows.

### Help and feedback

- Questions, ideas and bugs: [Discord](https://discord.gg/KZKGwSbF4W).
- Support the project: [Donatello](https://donatello.to/zaddiros).
- The source code is kept in a private repository; this repository only hosts releases.
