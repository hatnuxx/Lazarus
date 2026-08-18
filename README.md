# Lazarus | لازاروس

A lightweight, privacy-first tool for adding fragment, fingerprint, and cipher parameters to VLESS/Trojan proxy links.

> All processing happens locally in your browser — no data is ever sent to any server.

---

## Features

- **Fragment Parameters** — Automatically inject `fm` (fragment mask) and `cs` (cipher suites) into your configs
- **Fingerprint** — Set TLS fingerprint (`fp`) for all links
- **Server Override** — Replace server address across all links at once
- **Multi-link Support** — Process multiple links simultaneously
- **Bilingual** — Full Persian (FA) and English (EN) support
- **Dark / Light Theme** — Toggle between themes, preference saved locally
- **Zero Dependencies** — Single HTML file, no build step, no framework

## Supported Protocols

| Protocol | Status |
|----------|--------|
| VLESS    | ✅ Full support |
| Trojan   | ✅ Full support |

## Client Requirements

| Platform | Client | Minimum Version |
|----------|--------|-----------------|
| Windows  | v2rayN | 7.24.7+ |
| Android  | v2rayNG / PattNG | 2.3.4+ |

> This tool only works with configs that have **TLS** enabled (`security=tls` or `security=reality`).

## Usage

1. Open `index.html` in your browser
2. Paste your `vless://` or `trojan://` links (one per line)
3. Adjust fingerprint, cipher suites, or fragment settings if needed
4. Click **Convert**
5. Copy the enhanced links from the output

## Project Structure

```
Lazarus/
├── index.html    # Main application (single-file)
├── README.md     # This file
├── LICENSE       # MIT License
└── .gitignore    # Git ignore rules
```

## License

[MIT](LICENSE)

---

# لازاروس

ابزاری سبک و حریم‌خواه برای افزودن پارامترهای فرگمنت، اثر انگشت و مجموعه رمزها به لینک‌های پروکسی VLESS/Trojan.

> تمام پردازش‌ها در مرورگر شما انجام می‌شود — هیچ داده‌ای به هیچ سروری ارسال نمی‌گردد.

---

## امکانات

- **پارامترهای فرگمنت** — تزریق خودکار `fm` (ماسک فرگمنت) و `cs` (مجموعه رمزها) به کانفیگ‌ها
- **اثر انگشت** — تنظیم اثر انگشت TLS (`fp`) برای همه لینک‌ها
- **جایگزینی سرور** — تغییر آدرس سرور در همه لینک‌ها به صورت همزمان
- **پشتیبانی از چند لینک** — پردازش همزمان چند لینک
- **دو زبانه** — پشتیبانی کامل از فارسی و انگلیسی
- **حالت تاریک / روشن** — تغییر پوسته با ذخیره ترجیحات در مرورگر
- **بدون وابستگی** — یک فایل HTML، بدون نیاز به بیلد یا فریمورک

## پروتکل‌های پشتیبانی شده

| پروتکل | وضعیت |
|--------|-------|
| VLESS  | ✅ پشتیبانی کامل |
| Trojan | ✅ پشتیبانی کامل |

## نسخه مورد نیاز کلاینت

| پلتفرم | کلاینت | حداقل نسخه |
|---------|--------|-----------|
| ویندوز  | v2rayN | 7.24.7+ |
| اندروید | v2rayNG / PattNG | 2.3.4+ |

> این ابزار فقط روی کانفیگ‌هایی کار می‌کند که **TLS** فعال داشته باشند (`security=tls` یا `security=reality`).

## نحوه استفاده

1. فایل `index.html` را در مرورگر خود باز کنید
2. لینک‌های `vless://` یا `trojan://` را بچسبانید (هر خط یک لینک)
3. در صورت نیاز، اثر انگشت، مجموعه رمزها یا تنظیمات فرگمنت را تغییر دهید
4. روی **تبدیل کردن** کلیک کنید
5. لینک‌های بهبود یافته را از خروجی کپی کنید

## ساختار پروژه

```
Lazarus/
├── index.html    # برنامه اصلی (تک فایل)
├── README.md     # این فایل
├── LICENSE       # مجوز MIT
└── .gitignore    # قوانین نادیده گرفتن گیت
```

## مجوز

[MIT](LICENSE)
