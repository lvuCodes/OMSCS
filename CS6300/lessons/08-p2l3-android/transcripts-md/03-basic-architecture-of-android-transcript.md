# CS6300 151 - Basic Architecture of Android

| Timestamp | Content |
|-----------|---------|
| 00:00:00,180 --> 00:00:02,390 | Now that we saw some high level information on what |
| 00:00:02,390 --> 00:00:05,770 | Android is, let's discuss the basic architecture of the Android |
| 00:00:05,770 --> 00:00:08,390 | system. Let's start at the highest level where we have |
| 00:00:08,390 --> 00:00:11,570 | the Android apps which are applications, as we just saw, |
| 00:00:11,570 --> 00:00:14,000 | that are written in Java, and that get compiled into |
| 00:00:14,000 --> 00:00:18,120 | byte code, packaged and installed on the Android system. Basically, any |
| 00:00:18,120 --> 00:00:21,430 | applications that you ever used on any Android-powered phone or |
| 00:00:21,430 --> 00:00:25,020 | tablet is an app. Typical examples will be the Contacts app, |
| 00:00:25,020 --> 00:00:27,700 | so your address book. The Phone app in your smartphone, |
| 00:00:27,700 --> 00:00:30,020 | this is the app that allows you to make and receive |
| 00:00:30,020 --> 00:00:33,320 | phone calls. The browser, and of course games are also |
| 00:00:33,320 --> 00:00:36,520 | apps. Like for example, Angry Birds or Candy Crush, just in |
| 00:00:36,520 --> 00:00:39,280 | case you ever played any of those. Right underneath the |
| 00:00:39,280 --> 00:00:43,700 | apps, we have the application framework. The application framework is that |
| 00:00:43,700 --> 00:00:46,910 | layer that provides the services that are needed by Android |
| 00:00:46,910 --> 00:00:50,500 | apps to run. Such as the Window manager, the telephony manager, |
| 00:00:50,500 --> 00:00:53,130 | the location manager and the resource managers and there's |
| 00:00:53,130 --> 00:00:55,870 | many more. So basically, the apps rely on this |
| 00:00:55,870 --> 00:00:57,980 | layer to get information and to be able to |
| 00:00:57,980 --> 00:01:00,850 | work, to operate and to interact with the underlying |
| 00:01:00,850 --> 00:01:03,810 | phone. Going down one more layer, we have the |
| 00:01:03,810 --> 00:01:08,310 | Android native libraries which provide APIs for various functionalities. |
| 00:01:08,310 --> 00:01:11,490 | For example, the DB APIs, the WebKit APIs, the |
| 00:01:11,490 --> 00:01:15,710 | SSL APIs, OpenGL and so on. For instance, SQLite is |
| 00:01:15,710 --> 00:01:18,800 | the library that provides DB implementation for the |
| 00:01:18,800 --> 00:01:21,380 | DB APIs that your applications can use to |
| 00:01:21,380 --> 00:01:23,920 | store information. This layer, in addition to the |
| 00:01:23,920 --> 00:01:27,900 | libraries, also contains the Android runtime which consists of |
| 00:01:27,900 --> 00:01:30,760 | the Dalvik virtual machine which we just discussed, |
| 00:01:30,760 --> 00:01:33,820 | and also the core Java libraries. Basically the core |
| 00:01:33,820 --> 00:01:36,170 | Java libraries are the Android version of the |
| 00:01:36,170 --> 00:01:40,820 | standard Java libraries, also called JDKs. Finally, the basic |
| 00:01:40,820 --> 00:01:44,020 | layer, the layer on which all of this runs, is |
| 00:01:44,020 --> 00:01:47,350 | the Linux kernel, which is the core of the Android operating |
| 00:01:47,350 --> 00:01:49,930 | system and it is a standard Linux kernel, as we said, |
| 00:01:49,930 --> 00:01:53,240 | with some customizations made by Google. The Kernel interacts with the |
| 00:01:53,240 --> 00:01:56,480 | hardware and includes all the essential hardware drivers to access the |
| 00:01:56,480 --> 00:01:59,770 | network, the file system, the screen, and so on. So basically, |
| 00:01:59,770 --> 00:02:02,820 | these layers give you an idea of how the whole system |
| 00:02:02,820 --> 00:02:06,270 | works, starting from the apps, which are at the highest level, |
| 00:02:06,270 --> 00:02:07,690 | down to the lowest level, which is |
| 00:02:07,690 --> 00:02:07,690 | the Linux Kernel that interacts with the hardware. |