# CS6300 154 - Service

| Timestamp | Content |
|-----------|---------|
| 00:00:00,160 --> 00:00:02,190 | The next component that I want to discuss is a |
| 00:00:02,190 --> 00:00:06,510 | service. A service is an application component that performs a usually |
| 00:00:06,510 --> 00:00:10,000 | long running operation in the background while not interacting with |
| 00:00:10,000 --> 00:00:13,490 | the user. A typical example of a service, is a service |
| 00:00:13,490 --> 00:00:16,260 | for playing music which will run in the background even |
| 00:00:16,260 --> 00:00:19,560 | when we are not using the music app directly. Another typical |
| 00:00:19,560 --> 00:00:22,070 | example is a download service, such as the one that |
| 00:00:22,070 --> 00:00:26,020 | takes care of downloading updates in the background. Once more services, |
| 00:00:26,020 --> 00:00:28,370 | they run in the background and they don't interact with |
| 00:00:28,370 --> 00:00:31,480 | the user. So they perform some long running function while not |
| 00:00:31,480 --> 00:00:35,930 | interacting with the user. Therefore, unlike an activity, services do not |
| 00:00:35,930 --> 00:00:38,190 | provide a user interface. Similar |
| 00:00:38,190 --> 00:00:40,460 | to activities from the programmatic standpoint, |
| 00:00:40,460 --> 00:00:42,680 | the way to create a service is simply to extend |
| 00:00:42,680 --> 00:00:45,150 | the Service class, and we'll talk more about this. And there's |
| 00:00:45,150 --> 00:00:48,150 | just a few things that I want to mention about services, |
| 00:00:48,150 --> 00:00:51,330 | just to further clarify what they are. A service is not |
| 00:00:51,330 --> 00:00:53,990 | a way to offload some work that should be logically done |
| 00:00:53,990 --> 00:00:56,820 | by the application. But the service is a way for the |
| 00:00:56,820 --> 00:00:59,180 | app to tell the system about something that it wants to |
| 00:00:59,180 --> 00:01:01,770 | continue doing in the background, even when the user leaves the |
| 00:01:01,770 --> 00:01:05,069 | application. In addition, a service is also a way for the |
| 00:01:05,069 --> 00:01:08,660 | application to expose some of this functionality, for example the music |
| 00:01:08,660 --> 00:01:12,940 | playing functionality. By doing so, applications can bind to the service |
| 00:01:12,940 --> 00:01:16,850 | and using the service. For example, imagine a turn by turn navigation |
| 00:01:16,850 --> 00:01:20,690 | app, such an app will bind to the music player service to be able to |
| 00:01:20,690 --> 00:01:23,510 | stop the audio temporarily when making an announcement. |
| 00:01:23,510 --> 00:01:23,510 | For example, when a turn is upcoming. |