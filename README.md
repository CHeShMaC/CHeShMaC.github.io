<div align="center">
  <a href="#english">English</a> | <a href="#persian">فارسی</a>
</div>

---

<h2 id="persian">فارسی</h2>
<div dir="rtl">

# 👁️ چشمک | رمزنگاری مدرن با ایموجی

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Language](https://img.shields.io/badge/language-JavaScript-yellow.svg)
![Status](https://img.shields.io/badge/status-Stable-brightgreen.svg)

**چشمک** یک ابزار تحت وب سبک و متن‌باز است که متن‌های شما را به رشته‌ای از ایموجی‌ها تبدیل می‌کند. این ابزار با استفاده از الگوریتم‌های فشرده‌سازی مدرن مرورگر و رمزنگاری چند‌حرفی، پیام‌های شما را ایمن و فشرده کرده و آن‌ها را به شکلی جذاب و پنهان در معرض دید قرار می‌دهد.

🔗 **نمایش زنده:** [https://cheshmac.github.io/CHeShMaC.github.io/](https://cheshmac.github.io/CHeShMaC.github.io/)

---

## ✨ ویژگی‌های کلیدی

* **رمزنگاری ایموجی:** تبدیل متن خام به رشته‌ای از ایموجی‌ها بر اساس کلید رمز شخصی.
* **فشرده‌سازی هوشمند:** استفاده از API `CompressionStream` برای کاهش حجم متن قبل از رمزنگاری.
* **امنیت سمت کاربر:** تمام پردازش‌ها داخل مرورگر شما انجام می‌شود و هیچ داده‌ای به سرور ارسال نمی‌گردد.
* **رابط کاربری دوزبانه:** پشتیبانی کامل از زبان فارسی (RTL) و انگلیسی.
* **تم‌های رنگی:** دارای حالت تاریک (پیش‌فرض) و حالت روشن.
* **ریسپانسیو:** بهینه شده برای موبایل و دسکتاپ.

## 🛠️ مکانیزم عملکرد

چشمک تنها یک جایگزینی ساده نیست، بلکه فرایندی چندمرحله‌ای را طی می‌کند:

1.  **پردازش ورودی:** متن به بایت‌های UTF-8 تبدیل می‌شود.
2.  **فشرده‌سازی:** جریان بایت‌ها با الگوریتم `deflate-raw` فشرده می‌شود تا حجم پیام کاهش یابد.
3.  **رمزنگاری:** یک رمزنگاری به سبک Vigenère اعمال می‌شود. هر بایت داده با بایت متناظر از **کلید** شما ترکیب می‌شود (Modulo 256).
4.  **نگاشت ایموجی:** مقادیر بایت‌های رمزگذاری شده (0-255) به یک دیکشنری اختصاصی از 256 ایموجی نگاشت می‌شوند.

## 🚀 راهنمای استفاده

1.  **وارد کردن کلید:** یک رمز عبور امن (حداقل ۵ کاراکتر) وارد کنید یا دکمه "تصادفی" را بزنید.
2.  **نوشتن متن:** پیام خود را در کادر "متن ساده" بنویسید.
3.  **تبدیل:** دکمه آبی رنگ تبدیل را فشار دهید.
4.  **اشتراک‌گذاری:** رشته ایموجی تولید شده را کپی کرده و در تلگرام، واتس‌اپ یا پیامک ارسال کنید.
5.  **رمزگشایی:** گیرنده باید چشمک را باز کرده، **همان کلید** را وارد کند، ایموجی‌ها را جایگذاری کرده و تبدیل را بزند تا پیام اصلی نمایان شود.

## 💻 تکنولوژی‌های استفاده شده

* **HTML5**
* **CSS3** (متغیرهای CSS برای تم)
* **Vanilla JavaScript** (ES6+, CompressionStream API)
* بدون استفاده از کتابخانه‌های سنگین خارجی.

---

طراحی شده با ❤️ توسط [CHeShMaC](https://github.com/CHeShMaC)

</div>

---

<h2 id="english">English</h2>

# 👁️ چشمک | Modern Emoji Cryptography

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Language](https://img.shields.io/badge/language-JavaScript-yellow.svg)
![Status](https://img.shields.io/badge/status-Stable-brightgreen.svg)

**Cheshmak** (meaning "Wink" in Persian) is a lightweight, open-source web tool that transforms your text into a string of Emojis. It uses modern browser-native compression and a polyalphabetic cipher to ensure your messages are both compressed and secure, hiding sensitive data in plain sight.

🔗 **Live Demo:** [https://cheshmac.github.io/CHeShMaC.github.io/](https://cheshmac.github.io/CHeShMaC.github.io/)

---

## ✨ Key Features

* **Emoji Encryption:** Converts raw text into a compressed string of emojis based on a user-defined key.
* **Smart Compression:** Uses the `CompressionStream` API (Deflate-raw) to shrink text before encryption, allowing for longer messages.
* **Client-Side Security:** All processing happens in your browser. No data is sent to any server.
* **Bilingual UI:** Fully supports English (LTR) and Persian (RTL).
* **Themeable:** Includes a beautiful Dark Mode (default) and Light Mode.
* **Responsive:** Optimized for mobile and desktop devices.

## 🛠️ How It Works

Cheshmak is not just a simple substitution cipher. It employs a multi-step process:

1.  **Input Processing:** The text is converted to UTF-8 bytes.
2.  **Compression:** The byte stream is compressed using the `deflate-raw` algorithm to reduce payload size.
3.  **Encryption:** A Vigenère-style cipher is applied. Each byte of the data is shifted by the corresponding byte of your **Key** (Modulo 256).
4.  **Emoji Mapping:** The resulting encrypted byte values (0-255) are mapped to a specific dictionary of 256 unique Emojis.

## 🚀 Usage

1.  **Enter a Key:** Type a secure password (minimum 5 characters) or click "Random" to generate one.
2.  **Input Text:** Type your message in the "Plain Text" box.
3.  **Convert:** Click the blue conversion button.
4.  **Share:** Copy the resulting Emoji string and send it via Telegram, WhatsApp, or SMS.
5.  **Decrypt:** The recipient opens Cheshmak, enters the **same key**, pastes the Emojis, and clicks convert to reveal the message.

## 💻 Tech Stack

* **HTML5**
* **CSS3** (CSS Variables for theming)
* **Vanilla JavaScript** (ES6+, CompressionStream API)
* No external frameworks or heavy dependencies.

---

Made with ❤️ by [CHeShMaC](https://github.com/CHeShMaC)
