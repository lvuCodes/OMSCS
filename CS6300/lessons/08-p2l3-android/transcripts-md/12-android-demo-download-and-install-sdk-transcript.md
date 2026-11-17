# CS6300 160 - Android Demo_ Download & Install SDK

| Timestamp | Content |
|-----------|---------|
| 00:00:00,140 --> 00:00:02,480 | Now that we covered all the main conceptual |
| 00:00:02,480 --> 00:00:05,150 | aspects of the Android system, let's look at how |
| 00:00:05,150 --> 00:00:08,900 | these aspects work in practice through a demo. |
| 00:00:08,900 --> 00:00:12,220 | Let's start our Android demo by downloading the Android |
| 00:00:12,220 --> 00:00:17,000 | SDK, which will allow us to build Android apps. To do that, we need to go to |
| 00:00:17,000 --> 00:00:22,300 | the site developer.android.com. Here, we click on Develop. |
| 00:00:22,300 --> 00:00:25,270 | Then we click on Tools. And finally, we click |
| 00:00:25,270 --> 00:00:28,310 | on Download here on the left. This brings us to |
| 00:00:28,310 --> 00:00:31,780 | this page in which we can get the Android SDK. And |
| 00:00:31,780 --> 00:00:34,490 | we can get it as a bundle, where the bundle |
| 00:00:34,490 --> 00:00:38,209 | includes various things such as the Eclipse IDE, plus the ADT |
| 00:00:38,209 --> 00:00:42,520 | plugin, Android SDK Tools and other parts. So for now, |
| 00:00:42,520 --> 00:00:45,060 | what we're going to do, we're just going to download the Android SDK. |
| 00:00:45,060 --> 00:00:47,450 | So we're going to skip that and we're going to go to DOWNLOAD |
| 00:00:47,450 --> 00:00:50,970 | FOR OTHER PLATFORMS. And here where it says SDK Tools Only, |
| 00:00:50,970 --> 00:00:54,060 | you can pick the version of the Android SDK for your platform. |
| 00:00:54,060 --> 00:00:55,980 | So if you work on a Mac, you will pick this one |
| 00:00:55,980 --> 00:00:59,600 | and, otherwise, you can pick the Linux version or the Windows version. |
| 00:00:59,600 --> 00:01:02,490 | And once you click on that, you will get the SDK package. |
| 00:01:02,490 --> 00:01:05,880 | Now that you have downloaded the Android SDK for your platform, you |
| 00:01:05,880 --> 00:01:09,240 | can unzip it and you can do that graphically or as I'm |
| 00:01:09,240 --> 00:01:13,400 | doing here from the command line. So I'm just going to run unzip |
| 00:01:13,400 --> 00:01:16,080 | and pass the file as a parameter. And I'm doing the command |
| 00:01:16,080 --> 00:01:18,430 | line version because that's, you know, a little more |
| 00:01:18,430 --> 00:01:21,130 | challenging so the GUI one, you'll basically just click |
| 00:01:21,130 --> 00:01:24,145 | on the archive. And as soon as we have unpacked |
| 00:01:24,145 --> 00:01:28,320 | the SDK, we can move into the android-sdk directory. We |
| 00:01:28,320 --> 00:01:32,075 | can look at the content of the directory. And as |
| 00:01:32,075 --> 00:01:36,180 | you can see, there are several files and directories inside. |
| 00:01:36,180 --> 00:01:38,200 | And the one that we're interested in right now is |
| 00:01:38,200 --> 00:01:42,340 | the tools directory. So that's where we're going to go next. |
| 00:01:42,340 --> 00:01:45,084 | And again, if you're doing this through a GUI, we'll just click |
| 00:01:45,084 --> 00:01:48,550 | on the tools directory. And here, we have a bunch of applications. These |
| 00:01:48,550 --> 00:01:51,570 | are all part of the Android SDK. And what we're interested in is |
| 00:01:51,570 --> 00:01:54,995 | this android command. So we're going to run it, which you can do again |
| 00:01:54,995 --> 00:01:57,500 | from the command line or just by clicking on it. You'll probably |
| 00:01:57,500 --> 00:01:59,680 | get an error here but don't worry about it. We're going to fix it |
| 00:01:59,680 --> 00:02:02,310 | in a minute. So when we run the command, we're going to get the |
| 00:02:02,310 --> 00:02:04,710 | Android SDK Manager, which allows us |
| 00:02:04,710 --> 00:02:07,340 | to manage the different packages |
| 00:02:07,340 --> 00:02:09,150 | that are part of the Android SDK so to |
| 00:02:09,150 --> 00:02:12,720 | see which ones are installed and to install new ones. And |
| 00:02:12,720 --> 00:02:15,480 | as you can see, you can install different versions |
| 00:02:15,480 --> 00:02:18,640 | of Android. And for each version, there is a corresponding |
| 00:02:18,640 --> 00:02:22,005 | API version. And you can also see that |
| 00:02:22,005 --> 00:02:24,910 | the one selected by default is the latest version, which, |
| 00:02:24,910 --> 00:02:28,975 | in this case, is Android 4.4 and API version |
| 00:02:28,975 --> 00:02:32,850 | 19. So all the corresponding parts are selected for installation |
| 00:02:32,850 --> 00:02:36,100 | and, similarly, the platform tools and the build tools are also |
| 00:02:36,100 --> 00:02:38,710 | selected. And you can see on the right that none of |
| 00:02:38,710 --> 00:02:42,460 | these packages is currently installed. So we click Install to install |
| 00:02:42,460 --> 00:02:46,490 | these nine packages. Next, we have to accept the license in |
| 00:02:46,490 --> 00:02:48,530 | order to be able to install the packages. So we do |
| 00:02:48,530 --> 00:02:51,950 | that. We click Install again. And if you want, you can |
| 00:02:51,950 --> 00:02:54,440 | also look at the log here to see what's happening during |
| 00:02:54,440 --> 00:02:58,410 | the installation. And you can see that there's an error there referring |
| 00:02:58,410 --> 00:02:59,940 | to the fact that, you know, stopping |
| 00:02:59,940 --> 00:03:02,290 | the ADB server failed and that's okay because |
| 00:03:02,290 --> 00:03:04,110 | we haven't installed the server yet. So |
| 00:03:04,110 --> 00:03:06,261 | you might see exactly the same error. And |
| 00:03:06,261 --> 00:03:09,081 | at this point, you know, just you know, you just have to wait until the |
| 00:03:09,081 --> 00:03:11,990 | installation finishes. So we're going to stop here |
| 00:03:11,990 --> 00:03:11,990 | and we're going to go to the next step. |