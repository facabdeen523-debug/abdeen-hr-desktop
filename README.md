# مصنع عابدين - برنامج شئون الموظفين (Desktop)

**الوصف:** تطبيق سطح مكتب مبني بـ Electron + React + TypeScript + SQLite. الواجهة بالعربية (RTL).

## كيفية التشغيل محليًا (تطوّر)
1. تثبيت الحزم:
   ```
   npm install
   ```
2. تهيئة قاعدة البيانات التجريبية:
   ```
   node electron-db/db-init.js
   ```
3. تشغيل Vite:
   ```
   npm run dev
   ```
4. تشغيل Electron (في نافذة طرفية ثانية):
   ```
   npm run start:electron
   ```

## بناء ملف exe (Windows)
1. تأكد أنك على نظام Windows أو تستخدم CI على GitHub Actions (workflow موجود).
2. قم بالبناء:
   ```
   npm run build:web
   npm run build:win
   ```
سيتم إنشاء ملفات التثبيت أو المجلد القابل للتشغيل في `dist_electron`.

## ملاحظة
- لا يمكنني توليد ملف .exe داخل هذه الجلسة مباشرة، لكن أضفت ملف GitHub Actions سيمكنك من إنشاء exe تلقائيًا على GitHub وربط الـArtifacts.
