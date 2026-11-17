# CS6300 158 - Manifest

| Timestamp | Content |
|-----------|---------|
| 00:00:00,150 --> 00:00:02,300 | If you remember at the beginning of the lesson, I said |
| 00:00:02,300 --> 00:00:06,340 | the Manifest is what keeps an Android application together. So |
| 00:00:06,340 --> 00:00:08,780 | what is a Manifest exactly? A Manifest is an |
| 00:00:08,780 --> 00:00:12,670 | XML file that declares, among other things, all of the static |
| 00:00:12,670 --> 00:00:17,730 | components of your app. Activities, services and content providers. Broadcast |
| 00:00:17,730 --> 00:00:20,535 | receivers could be defined in either statically in the Manifest or |
| 00:00:20,535 --> 00:00:23,210 | dynamically at runtime. So they don't necessarily have to |
| 00:00:23,210 --> 00:00:25,840 | be in the Manifest, but they might be. The second thing. |
| 00:00:25,840 --> 00:00:28,830 | That the manifest declares are all the permissions required |
| 00:00:28,830 --> 00:00:31,860 | for your app to work. For example, if the application |
| 00:00:31,860 --> 00:00:35,760 | requires network access or access to calling and messaging capabilities, |
| 00:00:35,760 --> 00:00:39,440 | that must be specified in the manifest. The manifest also |
| 00:00:39,440 --> 00:00:42,710 | specifies the entry point for the application. That is, |
| 00:00:42,710 --> 00:00:46,490 | which activity should be launched when the application is executed. |
| 00:00:46,490 --> 00:00:48,530 | So what that means is that when you click on |
| 00:00:48,530 --> 00:00:51,100 | an app to start the app up the system will |
| 00:00:51,100 --> 00:00:53,740 | look into the Manifest to see which activity has to be |
| 00:00:53,740 --> 00:00:56,410 | started as a consequence of that. So which one is the |
| 00:00:56,410 --> 00:00:59,559 | entry point for your application as we were saying. The Manifest |
| 00:00:59,559 --> 00:01:02,490 | also declares the version of the app, and this is used for |
| 00:01:02,490 --> 00:01:05,590 | updates. Because the system is able to check which version you |
| 00:01:05,590 --> 00:01:09,300 | have and which one is the latest version available for that application. |
| 00:01:09,300 --> 00:01:13,520 | And finally, the manifest also declares the lowest Android SDK version |
| 00:01:13,520 --> 00:01:16,200 | for which this app is valid. So this is something that is |
| 00:01:16,200 --> 00:01:20,220 | checked at installation time to make sure that the application can run on |
| 00:01:20,220 --> 00:01:22,250 | your version of the operating system. So |
| 00:01:22,250 --> 00:01:24,690 | again, nothing too exciting, but information that |
| 00:01:24,690 --> 00:01:26,930 | is necessary for the system to understand |
| 00:01:26,930 --> 00:01:29,080 | how your application is structured and what |
| 00:01:29,080 --> 00:01:30,520 | the different parts are and what is |
| 00:01:30,520 --> 00:01:30,520 | needed for the application to operate correctly. |