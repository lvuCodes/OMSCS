# CS6300 159 - Android Activity Lifecycle

| Timestamp | Content |
|-----------|---------|
| 00:00:00,180 --> 00:00:02,100 | Now that we saw the main components of an Android |
| 00:00:02,100 --> 00:00:05,860 | application, there is one last, but very important aspect of |
| 00:00:05,860 --> 00:00:08,610 | Android that we need to cover, which is the Android |
| 00:00:08,610 --> 00:00:12,470 | activity lifecycle. So I'm going to use this classic diagram |
| 00:00:12,470 --> 00:00:16,621 | to illustrate such lifecycle. But before getting to describing the |
| 00:00:16,621 --> 00:00:18,875 | different parts, let's see why we have a lifecycle in |
| 00:00:18,875 --> 00:00:21,730 | the first place. The point here is that because Android |
| 00:00:21,730 --> 00:00:25,510 | apps run in a multitasking environment, the runtime system routinely |
| 00:00:25,510 --> 00:00:30,160 | suspends, stops, and even kills applications and activities. If |
| 00:00:30,160 --> 00:00:31,920 | you want an example, just think of the case of |
| 00:00:31,920 --> 00:00:33,850 | a phone call that arrives while you're writing an |
| 00:00:33,850 --> 00:00:36,630 | email message. In such cases, what happens is that the |
| 00:00:36,630 --> 00:00:40,430 | phone application replaces your email client and gets in |
| 00:00:40,430 --> 00:00:43,632 | the forefront. So apps must be able to react to |
| 00:00:43,632 --> 00:00:47,520 | these occurrences and suitably handle them. Luckily, the Android system |
| 00:00:47,520 --> 00:00:50,590 | is nice enough to notify activities when it needs to |
| 00:00:50,590 --> 00:00:53,712 | change their state, for example, when it needs to suspend, or |
| 00:00:53,712 --> 00:00:56,950 | kill them. And it does so by calling some special methods in |
| 00:00:56,950 --> 00:01:00,800 | the activities. Therefore, when you develop an application, an Android app, |
| 00:01:00,800 --> 00:01:04,019 | you must be aware of what these methods are, and suitably implement |
| 00:01:04,019 --> 00:01:06,620 | them. We will therefore now have a look at these methods, |
| 00:01:06,620 --> 00:01:09,710 | and see what they mean when they get called, and how this |
| 00:01:09,710 --> 00:01:12,792 | relates to the different states of an activity. And we're going to |
| 00:01:12,792 --> 00:01:15,720 | do that using this diagram that I introduced here. In order to |
| 00:01:15,720 --> 00:01:18,140 | better illustrate how this all works I'm going to |
| 00:01:18,140 --> 00:01:21,920 | complicate the picture a little bit by adding information about |
| 00:01:21,920 --> 00:01:26,080 | what happens when going from one phase of the lifecycle |
| 00:01:26,080 --> 00:01:28,150 | to another one. Because this will help make the |
| 00:01:28,150 --> 00:01:31,630 | diagram more self-explanatory. Let's start from here, from the |
| 00:01:31,630 --> 00:01:34,340 | moment when an activity, or an app is launched. We |
| 00:01:34,340 --> 00:01:37,140 | will call our activity A, and what happens is that |
| 00:01:37,140 --> 00:01:40,900 | when A is started, the system will call different methods |
| 00:01:40,900 --> 00:01:44,340 | on the activity, and will put the activity in the foreground. |
| 00:01:44,340 --> 00:01:46,490 | What that means is that the activity will stay on the |
| 00:01:46,490 --> 00:01:49,600 | screen, visible, the user will be able to interact with the |
| 00:01:49,600 --> 00:01:53,660 | activity, and the activity will be in the running state. And so |
| 00:01:53,660 --> 00:01:56,140 | this is when you're looking at your device and you are |
| 00:01:56,140 --> 00:01:59,380 | seeing in the foreground your activity and you can interact with it. |
| 00:01:59,380 --> 00:02:02,590 | At this point two things might happen if another activity is |
| 00:02:02,590 --> 00:02:06,000 | launched. In the first case A might lose its focus but still |
| 00:02:06,000 --> 00:02:08,222 | be visible. This is the case in which the new |
| 00:02:08,222 --> 00:02:11,280 | activity that is being created is maybe an activity that doesn't |
| 00:02:11,280 --> 00:02:13,750 | take up the whole screen, so my original activity is still |
| 00:02:13,750 --> 00:02:16,875 | visible in the background. Or a case in which the activity |
| 00:02:16,875 --> 00:02:19,584 | is a transparent activity, so it has focus but I can |
| 00:02:19,584 --> 00:02:22,920 | still see the original activity behind it. In this case the |
| 00:02:22,920 --> 00:02:26,960 | system will call onPause on Activity A. And the activity will |
| 00:02:26,960 --> 00:02:31,280 | be in the paused state. A paused activity is completely alive |
| 00:02:31,280 --> 00:02:33,900 | in the sense that it maintains all state information and |
| 00:02:33,900 --> 00:02:36,850 | remains attached to the window manager. But what can happen is |
| 00:02:36,850 --> 00:02:40,710 | that the activity might be killed or destroyed for example in |
| 00:02:40,710 --> 00:02:43,620 | case in which there is not enough memory to run both |
| 00:02:43,620 --> 00:02:47,030 | the new activity and the original activity. So the second case |
| 00:02:47,030 --> 00:02:49,550 | is a case in which the new activity that is being |
| 00:02:49,550 --> 00:02:53,550 | launched is completely obscuring my original activity. Which is a kind |
| 00:02:53,550 --> 00:02:56,280 | of more standard case. So, for example, you receive a phone |
| 00:02:56,280 --> 00:02:59,380 | call while you're editing a message. The phone app completely |
| 00:02:59,380 --> 00:03:03,300 | replaces the email client on your device, and becomes the |
| 00:03:03,300 --> 00:03:06,280 | new running activity, the one in the foreground. In this |
| 00:03:06,280 --> 00:03:09,470 | case the system will call onStop on the original activity and |
| 00:03:09,470 --> 00:03:11,930 | the activity will be in the stopped state. Similar to |
| 00:03:11,930 --> 00:03:15,480 | the paused state, also in this case the activity A |
| 00:03:15,480 --> 00:03:18,110 | still retains all of its state information but it is more |
| 00:03:18,110 --> 00:03:21,290 | likely that it will be killed or destroyed by the system. |
| 00:03:21,290 --> 00:03:23,640 | So let's look at what can happen from these two states |
| 00:03:23,640 --> 00:03:26,520 | in a little more detail. As we said there are cases |
| 00:03:26,520 --> 00:03:30,490 | in which an app with higher priority might need memory from |
| 00:03:30,490 --> 00:03:33,655 | the system, resources from the system. And the activity that's paused or |
| 00:03:33,655 --> 00:03:36,800 | stopped will be killed. In this case, if the user happens |
| 00:03:36,800 --> 00:03:39,580 | to go back to the activity, the system will recreate it |
| 00:03:39,580 --> 00:03:42,710 | basically, so it will restart it from scratch. So this is |
| 00:03:42,710 --> 00:03:46,310 | the reason why it is very important that when your application goes |
| 00:03:46,310 --> 00:03:48,900 | into the paused or stopped state, which means when the |
| 00:03:48,900 --> 00:03:52,970 | system calls onPause or onStop in your app, you suitably save |
| 00:03:52,970 --> 00:03:55,010 | the state of the application so that the state can |
| 00:03:55,010 --> 00:03:58,980 | be restored if the activity is killed and recreated afterwards. A |
| 00:03:58,980 --> 00:04:02,180 | second possibility when your activity is paused or stopped is |
| 00:04:02,180 --> 00:04:05,430 | that the activity is finishing or is being completely destroyed by |
| 00:04:05,430 --> 00:04:08,410 | the system. In this case, the onDestroy method is called and |
| 00:04:08,410 --> 00:04:11,390 | the activity is shut down for good. The third possibility is |
| 00:04:11,390 --> 00:04:14,620 | that the activity is not killed, is not destroyed, and the user |
| 00:04:14,620 --> 00:04:17,850 | simply returns to the activity. For example, you go back to editing |
| 00:04:17,850 --> 00:04:21,180 | your email after finishing your phone call. In this case, the system |
| 00:04:21,180 --> 00:04:24,880 | will call onRestart() on the activity and the activity will go back |
| 00:04:24,880 --> 00:04:27,390 | to the running state. So what I just covered are kind of |
| 00:04:27,390 --> 00:04:31,410 | the main paths through an activity lifecycle. But I'll strongly encourage you |
| 00:04:31,410 --> 00:04:33,490 | to read more about this, and to make sure to go through |
| 00:04:33,490 --> 00:04:36,690 | this lifecycle until it is clear to you what the different states |
| 00:04:36,690 --> 00:04:38,710 | are, and what you should do for each of them |
| 00:04:38,710 --> 00:04:38,710 | when the system invokes state changing methods on your activity. |