# منظومة المصور ياسر الطائي لحماية المحتوى وإدارة البلاغات

هذه نسخة أولية جاهزة للنشر على GitHub Pages.

## الملفات
- `index.html`: الموقع كامل بملف واحد.

## ما الذي يعمل؟
- واجهة عربية RTL.
- اختيار المنصة ونوع الانتهاك.
- توليد بلاغ عربي + إنجليزي.
- زر للمسار الرسمي لمركز المساعدة.
- تسجيل دخول Google عبر OAuth.
- إرسال Gmail عبر Gmail API بصلاحية `gmail.send` فقط.

## مهم قبل أن يعمل إرسال Gmail
تحتاج إنشاء Google Cloud Project وOAuth Client ID خاص بالموقع، ثم:
1. فعّل Gmail API في مشروع Google Cloud.
2. أنشئ OAuth 2.0 Client ID من نوع Web application.
3. أضف رابط GitHub Pages ضمن Authorized JavaScript origins.
4. افتح الموقع، ضع Client ID في الخانة، واحفظه.
5. اضغط "تسجيل الدخول عبر Google" ووافق على صلاحية الإرسال.

الأداة لا تعرف كلمة مرور Google ولا تحفظها.

## النشر على GitHub Pages
1. ارفع `index.html` إلى جذر المستودع.
2. من Settings > Pages اختر Deploy from a branch.
3. اختر branch: `main` والمجلد `/ (root)`.
4. احفظ وانتظر حتى يظهر رابط GitHub Pages.

## تنبيه
هذه الأداة تنظّم البلاغات والمراسلات، ولا تملك صلاحية حذف محتوى مباشرة من خوادم منصات التواصل.
