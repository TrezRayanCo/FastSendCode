ارسال پیامک کد فعال سازی و یا احراز هویت کاربران یکی از مسائل مهم طراحان سایت و اپلیکیشن ها می باشد. چرا که این پیام ها هم باید به همه ارسال شوند و هم با سرعت بسیار بالا ارسال گردد.
ما برای شما راه حل ساده ای داریم. این امکان کاملا رایگان در اختیار شما قرار می گیرد و شما فقط هزینه پیام ها را پرداخت می کنید ، این نکته را توجه داشته باشید که این پیامک ها به شماره های بلک لیست و یا شماره های مسدود هم ارسال می شوند لازم به ذکر است که وظیفه تولید کد نیز بر عهده سامانه می باشد و شما فقط شماره موبایل کاربرتان را اعلام می کنید.بنابراین شما دیگر دغدغه ای برای ارسال پیامک کد فعال سازی برای احراز هویت کاربر نخواهید داشت.
ارسال پیامک کد فعال سازی یا احراز هویت پیامکی خودکار از طریق URL
ارسال پیامک از طریق متد Post :
 
آدرس : http://smspanel.Trez.ir/AutoSendCode.ashx
پارامتر ها :
نام کاربری :	UserName	مثلا : test123
رمز عبور :	Password	مثلا : 123456 / رمز سامانه پیامک
گیرنده کد فعال سازی :	Mobile	مثلا : 09116665601
متن انتهای پیامک	Footer	 RayganSMS : مثلا
 
نمونه کد سی شارپ برای استفاده از متد پست :
 
RemotePost myremotepost = new RemotePost();
myremotepost.Url = "http://smspanel.Trez.ir/AutoSendCode.ashx";
myremotepost.Add("Username", "test123");
myremotepost.Add("Password", "123456");
myremotepost.Add("Mobile", "09116665601");
myremotepost.Add("Footer", "RayganSMS"); // این بخش اختیاری می باشد
myremotepost.Post();
 کلاس RemotePost را از این جا دانلود کنید  
http://smspanel.trez.ir/Download/RemotePost.rar
•	سامانه پیامک بصورت خود کار کد فعال سازی را تولید می کند و شما می توانید با استفاده از بخشی که در ادامه شرح داده خواهد شد صحت کد فعال سازی که کاربر شما در سایت و یا نرم افزار شما وارد نموده است را بررسی نمایید.
ارسال پیامک از طریق متد GET :
 
آدرس : http://smspanel.Trez.ir/AutoSendCode.ashx
پارامتر ها :
نام کاربری:	UserName	مثلا : test123
رمز عبور :	Password	مثلا : 123456 / رمز سامانه پیامک
گیرنده کد فعال سازی :	Mobile	مثلا : 09116665601
متن انتهای پیامک :	Footer	RayganSMS : مثلا
 
نمونه کامل سامانه :
http://smspanel.Trez.ir/AutoSendCode.ashx?Username=test123&Password=****&Mobile=09116665601&Footer=RayganSMS
بررسی صحت کد فعال سازی یا احراز هویت پیامکی از طریق URL
بررسی از طریق متد Post :
 
آدرس : http://smspanel.Trez.ir/CheckSendCode.ashx
پارامتر ها :
نام کاربری:	UserName	مثلا : test123
رمز عبور :	Password	مثلا : 123456 / رمز سامانه پیامک
گیرنده کد فعال سازی :	Mobile	مثلا : 09116665601
کد فعال سازی :	Code	123456 : مثلا
نمونه کد سی شارپ برای استفاده از متد پست :
 
RemotePost myremotepost = new RemotePost();
myremotepost.Url = "http://smspanel.Trez.ir/CheckSendCode.ashx";
myremotepost.Add("Username", "test123");
myremotepost.Add("Password", "123456");
myremotepost.Add("Mobile", "09116665601");
myremotepost.Add("Code", "123456");
myremotepost.Post();
 کلاس RemotePost را از این جا دانلود کنید  
http://smspanel.trez.ir/Download/RemotePost.rar
•	سامانه پیامک بصورت خود کار کد فعال سازی را تولید می کند و شما می توانید با استفاده از بخشی که در ادامه شرح داده خواهد شد صحت کد فعال سازی که کاربر شما در سایت و یا نرم افزار شما وارد نموده است را بررسی نمایید.
ارسال پیامک از طریق متد GET :
 
آدرس : http://smspanel.Trez.ir/CheckSendCode.ashx
پارامتر ها :
نام کاربری:	UserName	مثلا : test123
رمز عبور :	Password	مثلا : 123456 / رمز سامانه پیامک
گیرنده کد فعال سازی :	Mobile	مثلا : 09116665601
کد فعال سازی :	Code	123456 : مثلا
نمونه کامل سامانه :
http://smspanel.Trez.ir/CheckSendCode.ashx?Username=test123&Password=****&Mobile=09116665601&Code=123456
ارسال پیامک کد فعال سازی یا احراز هویت پیامکی با کد فعال سازی دلخواه از طریق URL
ارسال پیامک از طریق متد Post :
 
آدرس : http://smspanel.Trez.ir/SendMessageWithCode.ashx
پارامتر ها :
نام کاربری :	UserName	مثلا : test123
رمز عبور :	Password	مثلا : 123456 / رمز سامانه پیامک
گیرنده کد فعال سازی :	Mobile	مثلا : 09116665601
متن پیامک	Message	 با سلام ، کد فعال سازی : 123456 : مثلا
 
نمونه کد سی شارپ برای استفاده از متد پست :
 
RemotePost myremotepost = new RemotePost();
myremotepost.Url = "http://smspanel.Trez.ir/SendMessageWithCode.ashx";
myremotepost.Add("Username", "test123");
myremotepost.Add("Password", "123456");
myremotepost.Add("Mobile", "09116665601");
myremotepost.Add("Message", "Your Code Is : 123456"); // این بخش اختیاری می باشد
myremotepost.Post();
 کلاس RemotePost را از این جا دانلود کنید  
http://smspanel.trez.ir/Download/RemotePost.rar
•	سامانه پیامک بصورت خود کار کد فعال سازی را تولید می کند و شما می توانید با استفاده از بخشی که در ادامه شرح داده خواهد شد صحت کد فعال سازی که کاربر شما در سایت و یا نرم افزار شما وارد نموده است را بررسی نمایید.
ارسال پیامک از طریق متد GET :
 
آدرس : http://smspanel.Trez.ir/SendMessageWithCode.ashx
پارامتر ها :
نام کاربری:	UserName	مثلا : test123
رمز عبور :	Password	مثلا : 123456 / رمز سامانه پیامک
گیرنده کد فعال سازی :	Mobile	مثلا : 09116665601
متن پیام :	Message	با سلام ، کد فعال سازی : 123456: مثلا
 
نمونه کامل سامانه :
http://smspanel.Trez.ir/SendMessageWithCode.ashx?Username=test123&Password=****&Mobile=09116665601&Message=Your Code is : 123456
در صورتی که مقدار True را دریافت نمایید بدین معنی است که کد فعال سازی درست  می باشد و در غیر اینصورت کد غلط است
 
برای استفاده کافیست آدرس بالا را در قسمت آدرس بار سامانه کپی کنید و پارامتر های مربوط به خود را ثبت و اجرا نمایید.
نکات مهم :
•	در صورتی که پس از ارسال با کد 8 مواجه شده اید. این به این معنی می باشد که امکان استفاده از وب سرویس و url برای شما فعال نمی باشد.برای فعال کردن این امکان بصورت رایگان در قسمت پشتیبانی با تیکت درخواست فعال سازی را ثبت نمایید و یا با شرکت تماس بگیرید.
•	در صورتی که از ارسال با عددی بزرگتر از 2000 مواجه شده اید به این معنی می باشد که پیامک شما بدون نقض ارسال گردید. و در غیر این صورت با خطا مواجه شده اید.
•	در هر صورتی که با خطا مواجه شده اید و یا برای استفاده از این امکان دچار مشکل شده اید با ما در تماس باشید

