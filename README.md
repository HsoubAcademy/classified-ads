

 موقع إعلانات مبوبة
-------------------------------


1- git clone git@gitlab.com:mabras/classifiedads.git

2- أضف ملف .env

3- نفذ الأمر composer install

4- أنشئ الجداول مع تعبئة البيانات بواسطة الأمر
 php artisan migrate --seed



 لتجربة عملية إرسال الايميل
-------------------------------
قم بضبط الإعدادات في ملف env حسب التعريف الذي تختاره.

في حال اخترت التجربة على https://mailtrap.io لمحاكاة إرسال البريد نفذ ما يلي:

1- سجل في الموقع المذكور

2- بعد التسجيل ادخل على الرابط https://mailtrap.io/inboxes/
   ثم انتقل إلى Demo inbox

3- انسخ اسم المستخدم و الباسوورد إلى ملف env ، لتصبح الإعدادات كالتالي:

QUEUE_DRIVER=database

MAIL_DRIVER=smtp

MAIL_HOST=smtp.mailtrap.io

MAIL_PORT=2525

MAIL_USERNAME=اسم المستخدم
MAIL_PASSWORD= الباسوورد

MAIL_ENCRYPTION=tls


