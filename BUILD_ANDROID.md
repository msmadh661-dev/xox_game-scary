# بناء نسخة الأندرويد

## الطريقة 1: على جهازك (يحتاج Node 20+ و Android Studio)
    npm install
    npm run build
    npx cap add android
    # في android/app/src/main/AndroidManifest.xml أضف للـ activity:
    #   android:screenOrientation="sensorLandscape"
    npx cap sync android
    npx cap open android      # ثم Build > Build APK(s)

## الطريقة 2: بدون تثبيت أي شيء
ارفع المجلد إلى مستودع GitHub ثم Actions > "Build Android APK" > Run workflow.
بعد دقائق حمّل ملف dark-forest-apk من نتائج التشغيل وثبّته على هاتفك.

## التحكم باللمس
- عصا يسار الشاشة: الحركة
- السحب على يمين الشاشة: النظر حولك
- زر "جري" + أزرار الكشاف/الفلير/العلاج في الواجهة
