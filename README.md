# Standard Input Output
في لغة برمجة Dart ، يمكنك أخذ المدخلات من المستخدم من خلال مايسمى console or Terminal

كيف يتم اخذ ادخالات المستخدم ؟

  لأخذ مدخلات من المستخدم، تحتاج إلى استيراد مكتبة  تسمى dart: io من مكتبات Dart. ثم استخدام دالة  stdin.readLineSync() وهذه الداله هي إحدى الطرق المستخدمة لأخذ المدخلات من المستخدم

مثال :


    import 'dart:io';
    void main()
    {
        print("Enter your name?");
        // Reading name of the Student
        String? name = stdin.readLineSync();
        // Printing the name
        print("Hello, $name! \nWelcome to Tuwaiq Academy!!");
    }

نلاحظ تم استخدام دالة stdin.readLineSync() بعد = ليتم اسناد قيمتها داخل المتغير name.
يتم الاستفاده من اسناد قيمة الداله داخل متغير ليتم التعامل مع القيمه داخل الكود عن طريق هذا المتغير 
المخرجات :
سوف يتم الطلب من المستخدم ادخال الاسم 

    Enter your name?



    Enter your name?
    Fahad

بعد كتابة الاسم سوف يتم اظهار الرساله الموجوده داخل print مع طباعة الاسم الذي تم ادخاله 

    Hello, Fahad! 
    Welcome to Tuwaiq Academy!!

ليصبح المخرجات في النهايه بهذا الشكل :


    Enter your name?
    Fahad
    Hello, Fahad! 
    Welcome to Tuwaiq Academy!!


ادخال الارقام :

اي مدخل يتم ادخاله من قبل المستخدم يعتبر String. لتعامل مع الارقام المدخله من المستخدم يجب تحويله من String  الى رقم بستخدام دالة pares  

مثال :

    // Importing dart:io file
    import 'dart:io';
     
    void main()
    {
        // Asking for favourite number
        print("Enter your number:");
     
       // Scanning number
        int? n = int.parse(stdin.readLineSync()!);
       // Here ? and ! are for null safety
     
        // Printing that number
        print("Your number is $n");
    }


- نلاحظ في المثال الاعلى تم تعريف متغير n من نوع int  
- ثم تم كتابة int بعد = بعدها دالة pares  ليتم تحويل اي قيمه  الى int يتم تضمينها داخل اقواس () الخاصه فيه parse 
    - لاستخدام دالة parse يتم كتابة النوع المراد تحويل القيمه لها ثم كتابة .parse 
- بعد تحويل القيمه من String الى int تم اسناد القيمه داخل المتغير n 

المخرجات :

    Enter your number:

في البدايه سوف يتم طلب منك ادخال رقمك 


    Enter your number:
    0550200335

بعد كتابة المستخدم الرقم سوف يتم اظهار له رساله تحتوي على الرقم المدخل 


    Enter your number:
    0550200335
    Your number is 550200335


مسودة
