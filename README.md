<div align="center">

<img src="logo.svg" alt="Lazarus Logo" width="200" />

# Lazarus | لازاروس

A lightweight, privacy-first tool for enhancing VLESS & Trojan proxy configs with fragment, fingerprint, and cipher suite parameters.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![GitHub stars](https://img.shields.io/github/stars/hatnuxx/Lazarus?style=flat&logo=github)](https://github.com/hatnuxx/Lazarus/stargazers)
[![GitHub Pages](https://img.shields.io/badge/%F0%9F%8C%90%20Live%20Demo-GitHub%20Pages-blue?style=for-the-badge)](https://hatnuxx.github.io/Lazarus/)

> All processing happens entirely in your browser — **no data is ever sent to any server.**

</div>

---

## Live Demo

**[Launch Lazarus](https://hatnuxx.github.io/Lazarus/)** — no installation required. Just open and use.

---

## Features

| Feature | Description |
|---------|-------------|
| **Fragment Parameters** | Automatically inject `fm` (fragment mask) and `cs` (cipher suites) into your configs |
| **TLS Fingerprint** | Set TLS fingerprint (`fp`) to `unsafe`, `chrome`, `firefox`, `safari`, `random`, or `none` |
| **Server Override** | Replace the server address across all input links at once |
| **Multi-link Support** | Process multiple `vless://` or `trojan://` links simultaneously |
| **Bilingual UI** | Full Persian (FA, RTL) and English (EN, LTR) with one-click toggle |
| **Dark / Light Theme** | Toggle between themes, preference saved in `localStorage` |
| **Zero Dependencies** | Single HTML file — no build step, no framework, no external libs |

## How It Works

Lazarus parses your existing VLESS/Trojan proxy links and injects additional parameters that help bypass network restrictions:

| Parameter | Key | Purpose |
|-----------|-----|---------|
| Fragment Mask | `fm` | Splits TLS ClientHello into smaller fragments to evade DPI inspection |
| Cipher Suites | `cs` | Overrides the list of cipher suites offered during the TLS handshake |
| Fingerprint | `fp` | Modifies the TLS fingerprint to match common browsers (Chrome, Firefox, etc.) |

> **Note:** These parameters are only applied when `security=tls` or `security=reality` is present in the config.

## Supported Protocols

| Protocol | Status |
|----------|--------|
| VLESS | Supported |
| Trojan | Supported |

## Client Requirements

| Platform | Client | Minimum Version |
|----------|--------|-----------------|
| Windows | v2rayN | 7.24.7+ |
| Android | v2rayNG / PattNG | 2.3.4+ |

## Quick Start

### Option A — Use the hosted version (Recommended)

Open **[hatnuxx.github.io/Lazarus](https://hatnuxx.github.io/Lazarus/)** in your browser.

### Option B — Run locally

```bash
git clone https://github.com/hatnuxx/Lazarus.git
cd Lazarus
# Open index.html in any modern browser
open index.html    # macOS
xdg-open index.html  # Linux
start index.html   # Windows
```

### Steps

1. Paste your `vless://` or `trojan://` links into the input area (one per line)
2. Adjust **fingerprint**, **cipher suites**, or **fragment settings** if needed
3. Optionally set a **server override** to replace the server address across all links
4. Click **Convert**
5. Copy the enhanced links from the output section

## Project Structure

```
Lazarus/
├── index.html    # Main application (single-file, ~1700 lines)
├── logo.svg      # Project logo
├── README.md     # This file
├── LICENSE       # MIT License
└── .gitignore    # Git ignore rules
```

## Tech Stack

- **HTML5** — Semantic markup, single-file structure
- **CSS3** — Custom properties for theming, transitions, responsive design, RTL support
- **Vanilla JavaScript** — ES5-compatible, IIFE pattern, zero external dependencies
- **Web APIs** — `URL`/`URLSearchParams`, `navigator.clipboard`, `localStorage`

## License

[MIT License](LICENSE) — Copyright (c) 2026 Lazarus Contributors

---

<details>
<summary><strong>فارسی (Persian)</strong></summary>

<br>

<div dir="rtl">

# لازاروس

ابزاری سبک و حریم‌خواه برای بهبود کانفیگ‌های پروکسی VLESS و Trojan با تزریق پارامترهای فرگمنت، اثر انگشت و مجموعه رمزها.

> تمام پردازش‌ها در مرورگر شما انجام می‌شود — **هیچ داده‌ای به هیچ سروری ارسال نمی‌گردد.**

### [باز کردن لازاروس](https://hatnuxx.github.io/Lazarus/) — بدون نیاز به نصب

### امکانات

- **پارامترهای فرگمنت** — تزریق خودکار `fm` (ماسک فرگمنت) و `cs` (مجموعه رمزها) به کانفیگ‌ها
- **اثر انگشت TLS** — تنظیم `fp` به مقادیر `unsafe`، `chrome`، `firefox`، `safari`، `random` یا `none`
- **جایگزینی سرور** — تغییر آدرس سرور در همه لینک‌ها به صورت همزمان
- **پشتیبانی از چند لینک** — پردازش همزمان چند لینک
- **دو زبانه** — پشتیبانی کامل از فارسی و انگلیسی
- **حالت تاریک / روشن** — تغییر پوسته با ذخیره ترجیحات در مرورگر
- **بدون وابستگی** — یک فایل HTML، بدون نیاز به بیلد یا فریمورک

### پروتکل‌های پشتیبانی شده

| پروتکل | وضعیت |
|--------|-------|
| VLESS | پشتیبانی کامل |
| Trojan | پشتیبانی کامل |

### نسخه مورد نیاز کلاینت

| پلتفرم | کلاینت | حداقل نسخه |
|---------|--------|-----------|
| ویندوز | v2rayN | 7.24.7+ |
| اندروید | v2rayNG / PattNG | 2.3.4+ |

> این ابزار فقط روی کانفیگ‌هایی کار می‌کند که **TLS** فعال داشته باشند (`security=tls` یا `security=reality`).

### نحوه استفاده

1. فایل `index.html` را در مرورگر خود باز کنید (یا از [نسخه آنلاین](https://hatnuxx.github.io/Lazarus/) استفاده کنید)
2. لینک‌های `vless://` یا `trojan://` را بچسبانید (هر خط یک لینک)
3. در صورت نیاز، اثر انگشت، مجموعه رمزها یا تنظیمات فرگمنت را تغییر دهید
4. روی **تبدیل کردن** کلیک کنید
5. لینک‌های بهبود یافته را از خروجی کپی کنید

### مجوز

[مجوز MIT](LICENSE)

</div>

</details>
