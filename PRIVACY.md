# Privacy & Security — Mopsino Account Manager

**English** · [Українська](#українська) · [Русский](#русский)

## What is stored on your PC and how

Everything is kept in `%APPDATA%\Mopsino Account Manager` on your own computer.

| Data | How it is protected |
|---|---|
| Roblox session cookies (`.ROBLOSECURITY`) | Encrypted with Windows (DPAPI, via Electron `safeStorage`). Only your Windows user on this PC can decrypt them. |
| Roblox login & password (only if you use one-click re-login) | Encrypted the same way. Optional. |
| License key and device ID (HWID) | Encrypted the same way. A license file copied to another PC does not work. |
| Settings, groups, tags, drop history | Plain local files. |

Cookies and passwords are never shown in the interface, never written to logs and never included in backups. Removing an account also deletes its saved Roblox login session.

If Windows encryption is unavailable (very rare), values are only Base64-encoded, so keep your Windows account protected with a password.

## Where the app connects

Mopsino talks only to:

- **Roblox** (`*.roblox.com`, `*.rbxcdn.com`) — logging in, launching games, profiles, avatars, presence. Your cookie is sent only to Roblox.
- **Mopsino license server** — when you activate PRO and re-check it later (on start and every 6 hours). Sent: **only your license key and device ID**. No cookies, no Roblox passwords.
- **Mopsino Discord tracker** — only if you turn on the Discord tracker (PRO). Sent: drop/reward statistics from your scripts (account names, avatars, level, gems, gold, drops). No cookies.
- **Your own Discord webhook** — only if you enter one in the tracker settings.
- **GitHub** — checking for updates and downloading them from this repository.

The local tracker receiver (`http://localhost:3217/mopsino`) listens only on your own PC and refuses requests from web pages.

## What is never collected

- No passwords or cookies are sent anywhere except to Roblox itself.
- No analytics, telemetry, crash reports or usage tracking.
- No ads, no third-party trackers.

## Check that your download is genuine

Every release lists SHA-256 hashes and VirusTotal reports. Installers are built by GitHub Actions and carry a signed build-provenance attestation:

```
gh attestation verify MopsinoAccountManager-Setup-X.Y.Z.exe --repo kildreyn/mopsino-account-manager
```

Download Mopsino only from [Releases](https://github.com/kildreyn/mopsino-account-manager/releases).

---

## Українська

**Що зберігається на ПК.** Усе лежить у `%APPDATA%\Mopsino Account Manager` на твоєму комп'ютері.
- Cookie Roblox, логін і пароль для повторного входу (якщо ввімкнено), ключ ліцензії та ID пристрою **зашифровані засобами Windows (DPAPI)**. Розшифрувати їх може лише твій користувач Windows на цьому ПК. Ліцензія, скопійована на інший ПК, не працює.
- Cookie і паролі ніколи не показуються в інтерфейсі, не пишуться в логи й не потрапляють у бекапи. Видалення акаунта стирає і його сесію Roblox.

**Куди програма ходить у мережу:**
- **Roblox** — вхід, запуск ігор, профілі, аватари, статуси. Cookie надсилається тільки на Roblox.
- **Сервер ліцензій Mopsino** — під час активації PRO і перевірки (при старті та кожні 6 годин). Надсилається **лише ключ ліцензії та ID пристрою**, без cookie і паролів.
- **Discord-трекер Mopsino** — тільки якщо ти його ввімкнеш (PRO): статистика дропів зі скриптів (імена акаунтів, аватари, рівень, гемы, золото, дропи). Без cookie.
- **Твій власний Discord-вебхук** — лише якщо ти його вкажеш.
- **GitHub** — перевірка й завантаження оновлень.

**Що не збирається взагалі:** паролі й cookie нікуди, крім Roblox; жодної аналітики, телеметрії, звітів про збої чи реклами.

**Перевірка завантаження:** у кожному релізі є SHA-256 і звіти VirusTotal, а exe мають підтвердження походження від GitHub (команда вище).

---

## Русский

**Что хранится на ПК.** Всё лежит в `%APPDATA%\Mopsino Account Manager` на твоём компьютере.
- Cookie Roblox, логин и пароль для повторного входа (если включено), ключ лицензии и ID устройства **зашифрованы средствами Windows (DPAPI)**. Расшифровать их может только твой пользователь Windows на этом ПК. Лицензия, скопированная на другой ПК, не работает.
- Cookie и пароли никогда не показываются в интерфейсе, не пишутся в логи и не попадают в бэкапы. Удаление аккаунта стирает и его сессию Roblox.

**Куда программа ходит в сеть:**
- **Roblox** — вход, запуск игр, профили, аватары, статусы. Cookie отправляется только на Roblox.
- **Сервер лицензий Mopsino** — при активации PRO и проверке (при запуске и каждые 6 часов). Отправляется **только ключ лицензии и ID устройства**, без cookie и паролей.
- **Discord-трекер Mopsino** — только если ты его включишь (PRO): статистика дропов из скриптов (имена аккаунтов, аватары, уровень, гемы, золото, дропы). Без cookie.
- **Твой собственный Discord-вебхук** — только если ты его укажешь.
- **GitHub** — проверка и загрузка обновлений.

**Что не собирается вообще:** пароли и cookie никуда, кроме Roblox; никакой аналитики, телеметрии, отчётов о сбоях или рекламы.

**Проверка загрузки:** в каждом релизе есть SHA-256 и отчёты VirusTotal, а exe имеют подтверждение происхождения от GitHub (команда выше).
