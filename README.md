# NetPulse

**Network quality monitor for Windows 10/11.** NetPulse pings several hosts continuously, draws a live
latency chart, detects outages, packet loss and lag spikes, and tells you *where* the problem is:
your router, your provider or DNS.

**[⬇ Download the latest version](https://github.com/zemidala/NetPulse-releases/releases/latest)** — a single `NetPulse.exe`, no installation and no .NET required.

English and Russian interface · Русский интерфейс — [see below](#русский)

![Fluent layout](screenshots/fluent.png)

## Features

- **Live latency chart** of several targets at once (Google DNS, Cloudflare, Yandex DNS and your router by default; add your own).
- **Outage detection**: N lost pings in a row start an outage, M replies end it; each outage is logged with its duration.
- **Connection quality** from the ITU-T E-model: R-factor and MOS, plus jitter, P95 and loss.
- **Where is the problem?** The “PC → router → provider → internet → DNS” path highlights the failing link.
- **DNS check** with a direct query to your DNS server, bypassing the Windows cache.
- **Three layouts** switchable on the fly: *Fluent* (Windows 11 style), *Focus* (large figures and an availability map), *Pulse* (gaming style with one bar per ping).
- **In-game overlay**: a small always-on-top window with your current ping.
- **Tray icon** colored by network state, notifications on outages and recovery, start with Windows.
- **Event log** in CSV, export of all measurements to Excel.
- Light and dark themes, update check.

| Focus | Pulse |
|---|---|
| ![Focus layout](screenshots/focus.png) | ![Pulse layout](screenshots/pulse.png) |

## Install

1. Download `NetPulse.exe` from [Releases](https://github.com/zemidala/NetPulse-releases/releases/latest).
2. Run it. The app is not code-signed yet, so Windows SmartScreen may warn you: click **More info → Run anyway**.
3. Settings are stored in `%APPDATA%\NetPulse`. To uninstall, delete the exe and that folder.

## Feedback

- 🐞 Found a bug or want a feature? [Open an issue](https://github.com/zemidala/NetPulse-releases/issues/new/choose).
- 💬 Questions, ideas, your setups — [Discussions](https://github.com/zemidala/NetPulse-releases/discussions).

English or Russian — both are fine.

---

## Русский

**Монитор качества сети для Windows 10/11.** NetPulse непрерывно пингует несколько узлов, рисует живой
график задержки, находит обрывы, потери пакетов и скачки пинга и показывает, *где* проблема:
в роутере, у провайдера или в DNS.

**[⬇ Скачать последнюю версию](https://github.com/zemidala/NetPulse-releases/releases/latest)** — один файл `NetPulse.exe`, без установки, .NET не нужен.
Язык интерфейса переключается в **Settings → Appearance → Language → Русский**.

Возможности:

- живой график задержки нескольких целей сразу;
- обнаружение обрывов с длительностью и числом потерянных пакетов;
- оценка качества связи по E-model (R-фактор, MOS), джиттер, P95, потери;
- цепочка «ПК → роутер → провайдер → интернет → DNS» с подсветкой проблемного звена;
- проверка DNS прямым запросом в обход кэша Windows;
- три шаблона экрана: Fluent, Focus и игровой Pulse;
- оверлей поверх игр, значок в трее, уведомления, автозапуск;
- журнал событий в CSV и экспорт замеров в Excel.

Установка: скачайте `NetPulse.exe` и запустите. Программа пока не подписана цифровой подписью, поэтому
Windows SmartScreen может показать предупреждение: нажмите **Подробнее → Выполнить в любом случае**.

Нашли ошибку — [создайте issue](https://github.com/zemidala/NetPulse-releases/issues/new/choose); вопросы и идеи — в [Discussions](https://github.com/zemidala/NetPulse-releases/discussions).
