<div dir=rtl>

ابزار فارسی برای آندروید
=============
موارد مصرف
-------------
در بسیاری از گوشی های آندروید حروف جدا از هم نوشته می شوند. برای حل این مشکل و به هم چسباندن حروف می توانید از این کلاس استفاده کنید.


نحوه ی استفاده
-------------
استفاده از این کتابخانه بسیار راحت است.
مثال

<pre dir=ltr>
String s = Tools.fa("متن");
TextView t1 = (TextView) findViewById(R.id.textView1);
t1.setText(s);
</pre>

نکته: این اصلاح در نسخه های جدید آندروید ایجاد مشکل می کند. بهتر است در قسمت تنظیمات برنامه ی خود امکان فعال و غیر فعال کردن این اصلاح را قرار دهید. نحوه ی غیر فعال کردن:

<pre dir=ltr>
Tools.enable = false;
</pre>

برای تصحیح فونت هم می تونید از کد زیر استفاده کنید.
فونت مورد نظر را هم در پوشه ی `assets` قرار دهید
<pre dir=ltr>
Typeface tf = Typeface.createFromAsset(getAssets(), "BZar.ttf");
t1.setTypeface(tf);
</pre>
نمونه ی تصویر:
![نمونه](https://github.com/smmoosavi/android-Farsi-Tools/raw/master/img/1.png)
