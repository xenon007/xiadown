<div align="center">
  <img src="./frontend/public/appicon.png" width="112" alt="Иконка XiaDown" />
  <h1>XiaDown</h1>
  <p><strong>Менеджер медиатеки с поддержкой загрузки видео</strong></p>
  <p>
    <img src="https://img.shields.io/github/v/tag/arnoldhao/xiadown?label=version" alt="Последняя версия" />
    <img src="https://img.shields.io/badge/license-Apache--2.0-blue" alt="Лицензия" />
    <img src="https://img.shields.io/badge/platform-Windows%20%7C%20macOS-lightgrey" alt="Поддерживаемые платформы" />
    <img src="https://img.shields.io/badge/stack-Go%20%E2%80%A2%20Wails%20%E2%80%A2%20React-green" alt="Технологии" />
  </p>
  <p>
    <a href="https://xiadown.app/">Сайт</a> ·
    <a href="https://xiadown.app/docs/">Документация</a> ·
    <a href="https://github.com/arnoldhao/xiadown/releases">Релизы</a> ·
    <a href="https://github.com/arnoldhao/xiadown/issues">Сообщить об ошибке</a> ·
    <a href="https://ko-fi.com/arnoldhao">Поддержать проект</a>
  </p>
  <p>
    <a href="./README.md">简体中文</a> ·
    <a href="./README_zh-Hant.md">繁體中文</a> ·
    <a href="./README_en.md">English</a> ·
    <a href="./README_ja-JP.md">日本語</a> ·
    <a href="./README_ko-KR.md">한국어</a> ·
    <a href="./README_es-419.md">Español (LatAm)</a> ·
    <a href="./README_pt-BR.md">Português (BR)</a> ·
    <a href="./README_id-ID.md">Bahasa Indonesia</a> ·
    <a href="./README_vi-VN.md">Tiếng Việt</a> ·
    <strong>Русский</strong>
  </p>
</div>

<p align="center">
  <a href="https://xiadown.app/docs/library/">
    <img src="./images/library.webp" alt="Медиатека XiaDown" width="92%" />
  </a>
  <br />
  <strong>Медиатека</strong>
</p>

## Обзор

XiaDown — менеджер медиатеки, который в первую очередь работает с локальными данными. Он поддерживает загрузку видео и обнаружение медиафайлов на веб-страницах. Также приложение служит клиентом YouTube, YouTube Music и RSS. Медиафайлы можно скачивать одним нажатием прямо во время просмотра.

## Основные возможности

- 🗂️ **[Медиатека](https://xiadown.app/docs/library/)** — загрузка видео, перекодирование и управление медиафайлами.
- 🔎 **[Поиск медиа (Sniff)](https://xiadown.app/docs/sniff/)** — обнаружение и скачивание медиафайлов с веб-страниц.
- 🎵 **[Музыка](https://xiadown.app/docs/music/)** — просмотр и скачивание музыки из YouTube Music, воспроизведение локальной музыки.
- ▶️ **[YouTube](https://xiadown.app/docs/youtube/)** — поиск, просмотр и скачивание видео.
- 📡 **[RSS](https://xiadown.app/docs/rss/)** — подписка на ленты, чтение публикаций и скачивание медиафайлов.

## Мобильная версия

📱 Приложение для iPhone и iPad находится в разработке.

## Интерфейс приложения

<table>
  <tr>
    <td align="center" width="50%"><a href="https://xiadown.app/docs/sniff/"><img src="./images/sniff-desk.webp" alt="Поиск медиа XiaDown" width="100%" /></a><br /><strong>Поиск медиа</strong></td>
    <td align="center" width="50%"><a href="https://xiadown.app/docs/rss/"><img src="./images/rss.webp" alt="RSS XiaDown" width="100%" /></a><br /><strong>RSS</strong></td>
  </tr>
  <tr>
    <td align="center" width="50%"><a href="https://xiadown.app/docs/music/"><img src="./images/youtube-music.webp" alt="Музыка XiaDown" width="100%" /></a><br /><strong>Музыка</strong></td>
    <td align="center" width="50%"><a href="https://xiadown.app/docs/youtube/"><img src="./images/youtube-live.webp" alt="YouTube в XiaDown" width="100%" /></a><br /><strong>YouTube</strong></td>
  </tr>
</table>

## Установка

### Homebrew

Установите приложение для macOS с помощью Homebrew cask:

```bash
brew install --cask arnoldhao/tap/xiadown
```

### Скачать пакет

| Платформа | Архитектура | Пакет | Ссылка |
| --- | --- | --- | --- |
| macOS | Apple Silicon | DMG | [Скачать](https://updates.dreamapp.cc/xiadown/downloads/xiadown-macos-arm64-latest.dmg) |
| macOS | Intel | DMG | [Скачать](https://updates.dreamapp.cc/xiadown/downloads/xiadown-macos-x64-latest.dmg) |
| Windows | x64 | Установщик | [Скачать](https://updates.dreamapp.cc/xiadown/downloads/xiadown-windows-x64-latest-installer.exe) |
| Windows | x64 | Портативная версия | [Скачать](https://updates.dreamapp.cc/xiadown/downloads/xiadown-windows-x64-latest.zip) |

> Для macOS требуется macOS 14 (Sonoma) или новее. Для Windows — Windows 10 или новее.

При первом запуске XiaDown поможет настроить язык, оформление, сеть и необходимые компоненты. Подробности см. в разделе [«Установка и первый запуск»](https://xiadown.app/docs/start/install/).

## Локальная разработка

Для разработки необходимы Go 1.25.12, Node.js 24, Bun 1.3.5 и Wails 3 alpha2.117:

```bash
go install github.com/wailsapp/wails/v3/cmd/wails3@v3.0.0-alpha2.117
wails3 task dev
```

Другие задачи сборки и проверки перечислены в [Taskfile.yml](./Taskfile.yml).

## Отказ от ответственности

- XiaDown предназначен исключительно для управления медиафайлами и сохранения материалов, к которым у вас есть законный доступ и право использования.
- Вы самостоятельно отвечаете за соблюдение местного законодательства, разрешений правообладателей и условий использования соответствующих платформ при скачивании, сохранении, преобразовании и использовании контента.
- Не используйте XiaDown для обработки контента, нарушающего авторские права, распространяемого без разрешения, доступного только за плату, приватного или иным образом незаконного.
- Вы принимаете на себя ответственность за любые проблемы, связанные с авторскими правами, правилами платформ, аккаунтами, сетевым доступом и другими последствиями использования XiaDown.

## Благодарности

XiaDown использует проекты с открытым исходным кодом, включая [Go](https://go.dev/), [Wails](https://v3alpha.wails.io/), [React](https://react.dev/), [yt-dlp](https://github.com/yt-dlp/yt-dlp), [FFmpeg](https://ffmpeg.org/) и [SQLite](https://www.sqlite.org/). Сведения о зависимостях и лицензиях см. в [THIRD_PARTY_NOTICES.txt](./frontend/public/THIRD_PARTY_NOTICES.txt).

## Участие в разработке

- В настоящее время проект не принимает pull request. Для сообщений об ошибках и предложений используйте [GitHub Issues](https://github.com/arnoldhao/xiadown/issues).
- Репозиторий распространяется по лицензии `Apache-2.0`. См. [LICENSE](./LICENSE).

## Контакты

- Сайт: <https://xiadown.app/>
- Документация: <https://xiadown.app/docs/>
- Электронная почта: <xunruhao@gmail.com>

---

*Перевёл: [Xenon007](https://github.com/xenon007).*
