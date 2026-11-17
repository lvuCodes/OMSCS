# CS6300 153 - Activity

| Timestamp | Content |
|-----------|---------|
| 00:00:00,250 --> 00:00:03,630 | Let's start with activities, in Android an activity is a single |
| 00:00:03,630 --> 00:00:06,490 | screen with a user interface. What I am showing here is a |
| 00:00:06,490 --> 00:00:09,500 | phone dialer, that you're probably pretty familiar with, because it is, |
| 00:00:09,500 --> 00:00:12,620 | you know, in one form or another, present in all smart |
| 00:00:12,620 --> 00:00:16,140 | phones. And this corresponds to an activity. There's another few things |
| 00:00:16,140 --> 00:00:20,170 | to know about activities. First of all, activities are independent units. |
| 00:00:20,170 --> 00:00:23,010 | But they can work together to form a cohesive whole and |
| 00:00:23,010 --> 00:00:25,490 | we'll see what that means. And one of the nice things about |
| 00:00:25,490 --> 00:00:28,940 | activities, is that they can be invoked by other applications. |
| 00:00:28,940 --> 00:00:31,700 | For example, assume that you're a runner and you're using the |
| 00:00:31,700 --> 00:00:34,450 | RunKeeper to keep track of your runs. RunKeeper |
| 00:00:34,450 --> 00:00:38,190 | can invoke a camera activity. When you're taking a picture during |
| 00:00:38,190 --> 00:00:40,450 | a run. So even though the camera activity is an |
| 00:00:40,450 --> 00:00:44,420 | independent one, it can be used by another application. Finally, from |
| 00:00:44,420 --> 00:00:47,070 | the programmatic standpoint, and as we will see in our |
| 00:00:47,070 --> 00:00:50,590 | demo, we can create an activity by simply extending the Activity |
| 00:00:50,590 --> 00:00:50,590 | class, which is part of the Android system. |