<div align="center" markdown="1">

<img src="icon.svg" alt="Mirage" width="128" height="128" />

# Mirage

### Защищённый децентрализованный мессенджер
**E2E-шифрование • Обход DPI • P2P Mesh**

[![Latest Release](https://img.shields.io/github/v/release/Prorok1015/Mirage-Releases?label=latest&style=flat-square)](../../releases/latest)
[![Platforms](https://img.shields.io/badge/platforms-Windows%20%7C%20macOS-blue?style=flat-square)](#-скачать)
[![Status](https://img.shields.io/badge/status-alpha-orange?style=flat-square)](#)

[Скачать](#-скачать) • [Установка](#-установка) • [Проверка целостности](#-проверка-целостности) • [Сообщить о проблеме](#-сообщить-о-проблеме)

</div>

---

> 📦 Этот репозиторий содержит **только готовые сборки** Mirage для конечных пользователей.

---

## ✨ Что такое Mirage

Mirage — это P2P-мессенджер, построенный вокруг приватности по умолчанию.

| | |
|---|---|
| 🔐 | **Сообщения видите только вы и собеседник.** Сквозное шифрование на Ed25519 + X25519 + ChaCha20-Poly1305. Серверы не имеют доступа к вашим сообщениям. |
| 🪪 | **Никаких номеров и email.** Учётная запись — это криптографическая пара ключей, созданная на вашем устройстве. |
| 🛡️ | **Обфусцированный трафик.** QUIC поверх UDP с TLS 1.3 — спроектирован так, чтобы быть неотличимым от обычного веб-трафика. |
| 🌐 | **Mesh-архитектура.** Когда прямое P2P-соединение невозможно, сообщения проходят через релейные узлы в зашифрованном виде. |

> ⚠️ **Alpha-релиз.** Mirage находится на ранней стадии. Используйте его для тестирования и знакомства, **но не как основной мессенджер**.

---

## 📥 Скачать

<p align="center" markdown="1">
  <a href="https://github.com/Prorok1015/Mirage-Releases/releases/latest/download/Mirage-Setup-Windows.exe">
    <img src="https://img.shields.io/badge/Скачать_для-Windows-0078D6?style=for-the-badge&logoColor=white" alt="Скачать для Windows" />
  </a>
  &nbsp;
  <a href="https://github.com/Prorok1015/Mirage-Releases/releases/latest/download/Mirage-macOS-arm64.dmg">
    <img src="https://img.shields.io/badge/Скачать_для-macOS_(Apple_Silicon)-000000?style=for-the-badge&logo=apple&logoColor=white" alt="Скачать для macOS Apple Silicon" />
  </a>
  &nbsp;
  <a href="https://github.com/Prorok1015/Mirage-Releases/releases/latest/download/Mirage-macOS-x64.dmg">
    <img src="https://img.shields.io/badge/Скачать_для-macOS_(Intel)-555555?style=for-the-badge&logo=apple&logoColor=white" alt="Скачать для macOS Intel" />
  </a>
</p>

<p align="center" markdown="1">
  <sub>
    Все версии и release notes — на странице
    <a href="https://github.com/Prorok1015/Mirage-Releases/releases/latest"><b>последнего релиза</b></a>.
  </sub>
</p>

> 💡 Файлы `latest.yml` и `latest-mac.yml` рядом с релизом нужны встроенному авто-апдейтеру — вручную их качать не требуется.

---

## 🛠 Установка

<details markdown="1">
<summary><b>🪟 Windows</b></summary>

1. Запустите `Mirage-Setup-X.Y.Z.exe`.
2. Если SmartScreen покажет предупреждение об «unknown publisher» — нажмите **«Подробнее»** → **«Выполнить в любом случае»**.
3. Следуйте инструкциям установщика.

</details>

<details markdown="1">
<summary><b>🍎 macOS</b></summary>

1. Откройте `.dmg` и перетащите Mirage в папку **Applications**.
2. При первом запуске macOS может сказать, что приложение от неизвестного разработчика. Откройте **Системные настройки** → **Безопасность и конфиденциальность** и нажмите **«Открыть в любом случае»**.

</details>

### 🔄 Автоматические обновления

После установки Mirage сам проверяет наличие новых версий через этот репозиторий и предлагает обновиться. Достаточно нажать на уведомление.

Управлять поведением апдейтера можно в **Настройках → Обновления**.

---

## 🔍 Проверка целостности

К каждому релизу прилагается файл **`SHA256SUMS.txt`** с контрольными суммами. Проверьте загруженный файл перед установкой.

**Windows (PowerShell):**
```powershell
Get-FileHash Mirage-Setup-X.Y.Z.exe -Algorithm SHA256
```

**macOS / Linux:**
```bash
shasum -a 256 Mirage-X.Y.Z-arm64.dmg
```

Полученное значение должно совпадать со строкой из `SHA256SUMS.txt`.

---

## 🐞 Сообщить о проблеме

| Тип | Куда писать |
|---|---|
| 🐛 **Баги, предложения, вопросы** | Откройте issue в этом репозитории |
| 💥 **Краш-репорты** | Включаются опцией **«Отчёты об ошибках»**. Клиент сам отправит минидампы — без содержимого сообщений. |

---

## 📜 Лицензия

© Mirage Project. Все права защищены. Условия использования будут опубликованы вместе с beta-релизом.

---

<div align="center" markdown="1">

**Сделано с заботой о приватности**

</div>
