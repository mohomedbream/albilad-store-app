# تطبيق البلاد - أندرويد (Capacitor)

التطبيق يعرض موقع https://www.albiladksa.com داخل التطبيق (الرابط في capacitor.config.json)، وتظهر صفحة www/index.html عند انقطاع الإنترنت.

## الطريقة 1: بناء APK على جهازك
المتطلبات: Node.js 18+ و Android Studio (يشمل JDK 17).
1. npm install
2. npx cap add android
3. npx cap sync android
4. npx cap open android  ثم من Android Studio: Build > Build APK(s)

## الطريقة 2: بناء APK سحابيًا بدون Android Studio
1. ارفع المجلد كاملًا إلى مستودع GitHub جديد.
2. افتح تبويب Actions وانتظر انتهاء Build APK.
3. نزّل الملف store-apk من أسفل صفحة التشغيل.

## التعديل
- المنتجات والأسعار تُدار من موقعك مباشرة، ولا تحتاج تحديث التطبيق عند تغييرها.
- بعد أي تعديل: npx cap sync android ثم أعد البناء.
- اسم التطبيق والمعرّف: capacitor.config.json (غيّر appId قبل النشر على Google Play).
