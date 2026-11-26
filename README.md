# حسابداری کوچک معین

پروژه Android WebView با شناسه `ir.hesabdarkoochak.moein`، حداقل Android 5.0 (API 21) و target/compile SDK 34.

## انتشار با GitHub Actions
1. این آرشیو را استخراج و تمام محتویات پوشه پروژه را به یک repository جدید GitHub آپلود کنید.
2. با push کردن فایل‌ها یا از تب **Actions** و گزینه **Run workflow**، گردش کار **Android build** اجرا می‌شود.
3. پس از پایان موفق، گردش کار را باز کنید و از بخش **Artifacts** فایل `hesabdarkoochak-debug-apk` را دریافت کنید. APK داخل آن `app-debug.apk` است.

Workflow به Java 17 و Gradle 8.6 متکی است و APK آزمایشی debug تولید می‌کند. برای انتشار عمومی Google Play باید نسخه release امضا‌شده با کلید خودتان بسازید.

## ساخت محلی
نیازمند JDK 17، Android SDK و Gradle 8.6 است. اجرا: `gradle assembleDebug`.

برنامه محتوای `app/src/main/assets/index.html` را داخل WebView بارگذاری می‌کند. داده‌ها در localStorage مرورگر ذخیره می‌شوند. منطق شمارنده آزمایشی ۳۰ تراکنش در HTML مبدا موجود است. خرید مایکت یا پل بومی پرداخت تنظیم نشده، چون شناسه محصول و SDK/اعتبارنامه فروشنده ارائه نشده است.
