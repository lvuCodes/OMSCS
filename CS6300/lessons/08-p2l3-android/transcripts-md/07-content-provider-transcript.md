# CS6300 155 - Content Provider

| Timestamp | Content |
|-----------|---------|
| 00:00:00,280 --> 00:00:02,330 | The third kind of component that I want to mention |
| 00:00:02,330 --> 00:00:07,120 | is the content provider. The content provider provides a structured interface |
| 00:00:07,120 --> 00:00:09,430 | to a set of data such as for example a set |
| 00:00:09,430 --> 00:00:12,950 | of pictures or media files in general. As we saw earlier, |
| 00:00:12,950 --> 00:00:16,948 | Android contains an implementation of the SQLite Database manager. So, |
| 00:00:16,948 --> 00:00:19,829 | very often, apps rely on a SQLite database to store |
| 00:00:19,829 --> 00:00:22,442 | the data and a provider to give it access to such |
| 00:00:22,442 --> 00:00:25,770 | data. In some cases, a provider can be used for accessing |
| 00:00:25,770 --> 00:00:28,450 | data within an application. In which case the data will |
| 00:00:28,450 --> 00:00:31,010 | be application data, such as a list of items to be |
| 00:00:31,010 --> 00:00:34,160 | bought for a shopping list management application. There is a |
| 00:00:34,160 --> 00:00:37,640 | much more interesting case, though. More generally a provider can be |
| 00:00:37,640 --> 00:00:40,820 | used by an application also to share data with other |
| 00:00:40,820 --> 00:00:44,930 | applications. In the case represented here for instance, this content provider |
| 00:00:44,930 --> 00:00:47,920 | is being accessed by three different applications. If you want an |
| 00:00:47,920 --> 00:00:51,500 | example, a typical one will be an address book, the contact |
| 00:00:51,500 --> 00:00:53,950 | app in your smartphone, for instance. The address |
| 00:00:53,950 --> 00:00:55,950 | book could use a provider to give access to |
| 00:00:55,950 --> 00:00:58,440 | the user contacts to other applications such as, for |
| 00:00:58,440 --> 00:01:01,820 | example, a telephone application, a voice over IP application, |
| 00:01:01,820 --> 00:01:04,349 | a messaging application, and so on. So in |
| 00:01:04,349 --> 00:01:07,040 | this case, all these applications will be able to |
| 00:01:07,040 --> 00:01:10,590 | access the same data through a common, well-structured interface, |
| 00:01:10,590 --> 00:01:10,590 | which is the one provided by the content provider. |