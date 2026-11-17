# CS6300 156 - Broadcast Receiver

| Timestamp | Content |
|-----------|---------|
| 00:00:00,168 --> 00:00:02,848 | The fourth and final component that we are going to |
| 00:00:02,848 --> 00:00:05,997 | cover is the broadcast receiver, which is a receiver, |
| 00:00:05,997 --> 00:00:08,409 | as the name says, that can be registered to |
| 00:00:08,409 --> 00:00:12,440 | receive system or application events. To illustrate, consider here, my |
| 00:00:12,440 --> 00:00:14,730 | broadcast receiver. Whereas here, we have the Android |
| 00:00:14,730 --> 00:00:17,510 | system. What the broadcast receiver can do is to |
| 00:00:17,510 --> 00:00:20,920 | register with the Android system for a specific event of |
| 00:00:20,920 --> 00:00:25,350 | interest. And the Android system will notify the broadcast receiver |
| 00:00:25,350 --> 00:00:28,930 | every time an event of that kind will occur. For |
| 00:00:28,930 --> 00:00:32,310 | an example, consider a music player. A music player could |
| 00:00:32,310 --> 00:00:35,740 | use a broadcast receiver to register for the event of |
| 00:00:35,740 --> 00:00:39,230 | incoming phone calls, because it wants to suspend playing music |
| 00:00:39,230 --> 00:00:42,460 | every time that there is a phone call incoming. Similarly, |
| 00:00:42,460 --> 00:00:44,940 | it could also register for the end of the phone |
| 00:00:44,940 --> 00:00:47,610 | call because it might want to resume playing music every |
| 00:00:47,610 --> 00:00:50,420 | time a phone call is ended. So broadcast receivers are extremely |
| 00:00:50,420 --> 00:00:50,420 | useful and can be used in many, many applications. |