# بناء APK لتطبيق عرض سعر سميك

## الطريقة 1: بدون تثبيت أي شيء (GitHub Actions)
1. أنشئ حساباً مجانياً على github.com ثم مستودعاً جديداً (New repository).
2. ارفع كل محتويات هذا المجلد (بما فيها المجلد المخفي .github).
3. افتح تبويب Actions ← Build APK ← Run workflow.
4. بعد 4-6 دقائق افتح التشغيل الناجح ونزّل الملف من Artifacts: samek-quote-apk.
5. فك الضغط وثبّت app-debug.apk على الهاتف (فعّل "التثبيت من مصادر غير معروفة").

## الطريقة 2: على الكمبيوتر (يلزم Node 18+ و Android Studio)
npm install
npx cap add android
npx cap sync android
npx cap open android   # ثم Build > Build APK
