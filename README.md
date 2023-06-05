# Android-get-and-display-time
Kotlin和XML获取并显示当前时间的程序
在activity_main.xml文件中，使用LinearLayout作为根布局，并在其中放置了一个TextView用于显示当前时间。
在MainActivity.kt文件中，创建了一个继承自AppCompatActivity的MainActivity类。
onCreate()方法是Activity的生命周期方法，在Activity创建时调用。
setContentView(R.layout.activity_main)设置Activity的布局为activity_main.xml。
currentTimeTextView = findViewById(R.id.currentTimeTextView)通过findViewById()方法获取XML布局中currentTimeTextView的引用。
getCurrentTime()方法用于获取当前时间并返回一个格式化后的字符串。
Calendar.getInstance().time获取当前时间的Date对象。
SimpleDateFormat("yyyy-MM-dd HH:mm:ss", Locale.getDefault())创建一个格式化日期的SimpleDateFormat对象，指定日期格式为"yyyy-MM-dd HH:mm:ss"。
dateFormat.format(currentTime)将currentTime按照指定的日期格式进行格式化。
currentTimeTextView.text = "Current time: $currentTime"将格式化后的时间字符串设置给currentTimeTextView的text属性，从而在应用程序界面上显示当前时间。
