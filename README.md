# منظومة المصور ياسر الطائي لحماية المحتوى وإدارة البلاغات

هذه الحزمة تحتوي النسخة الكاملة الحالية من الموقع.

## الملفات
- index.html
  الموقع كامل بملف واحد وجاهز للرفع على GitHub Pages.

- README.md
  تعليمات الإعداد والتشغيل.

## اسم النظام
منظومة المصور ياسر الطائي لحماية المحتوى وإدارة البلاغات

## ما الذي يعمل حالياً؟
- واجهة عربية.
- تسجيل الدخول بواسطة Google.
- اختيار منصة التواصل الاجتماعي.
- اختيار نوع الانتهاك.
- إدخال رابط المحتوى أو الحساب.
- توليد بلاغ عربي + إنجليزي.
- نسخ نص البلاغ.
- إرسال Gmail بعد تفعيل Gmail API ومنح صلاحية الإرسال.
- روابط مساعدة رسمية للمنصات.

## Google OAuth
تم وضع Google OAuth Client ID داخل النسخة الحالية.

Client ID:
176131693334-hkc4tpvolpt1dtedd8a8767higqi8348.apps.googleusercontent.com

## المطلوب في Google Cloud
1. افتح نفس Google Cloud Project.
2. اذهب إلى:
   APIs & Services > Library
3. ابحث عن:
   Gmail API
4. اضغط:
   Enable

## إعداد OAuth
نوع التطبيق:
Web application

Authorized JavaScript origins:
https://ymvlog1-boop.github.io

ملاحظة:
إذا تغير حساب GitHub أو رابط الاستضافة مستقبلاً، يجب إضافة الـ Origin الجديد داخل إعدادات OAuth.

## النشر على GitHub Pages
ارفع index.html إلى جذر المستودع.

ثم:
Settings > Pages

واجعل:
Source: Deploy from a branch
Branch: main
Folder: /(root)

بعدها افتح رابط GitHub Pages الخاص بالمستودع.

## مهم
هذه الأداة لا تملك صلاحية حذف المحتوى مباشرة من خوادم TikTok أو Facebook أو Instagram أو غيرها.
هي تنظّم البلاغات وتولّد طلبات رسمية وتساعد على إرسالها عبر حساب Gmail المرتبط.
