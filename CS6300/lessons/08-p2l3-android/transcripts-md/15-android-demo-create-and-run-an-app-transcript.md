# CS6300 163 - Android Demo_ Create & Run an App

| Timestamp | Content |
|-----------|---------|
| 00:00:00,340 --> 00:00:02,560 | So let's create our first Android app. To do |
| 00:00:02,560 --> 00:00:07,560 | that, we go to the Package Explorer>Contextual Menu>New>Other. This brings |
| 00:00:07,560 --> 00:00:09,990 | up the window in which we can select different types |
| 00:00:09,990 --> 00:00:13,490 | of applications and in particular Android applications. As you can |
| 00:00:13,490 --> 00:00:15,810 | see, we have several options. And the one that |
| 00:00:15,810 --> 00:00:19,090 | we want to pick is Android application project, so we select |
| 00:00:19,090 --> 00:00:22,790 | it. We click Next. So this will start this wizard |
| 00:00:22,790 --> 00:00:25,320 | in which we can choose different properties of the application, |
| 00:00:25,320 --> 00:00:28,610 | in particular the name. I'm going to call the application converter because |
| 00:00:28,610 --> 00:00:31,300 | the application I want to write is a simple application that |
| 00:00:31,300 --> 00:00:35,270 | converts between kilometers and miles. The next thing I can select |
| 00:00:35,270 --> 00:00:38,260 | is the Minimal Required SDK. So this is the information for |
| 00:00:38,260 --> 00:00:42,000 | backward compatibility. So it's saying that my application should run for |
| 00:00:42,000 --> 00:00:45,590 | any version of Android between 2.2 and 4.4, which is the |
| 00:00:45,590 --> 00:00:48,170 | current version. And the next thing I want to do is |
| 00:00:48,170 --> 00:00:50,570 | to change the package name, so I'm going to use the |
| 00:00:50,570 --> 00:00:53,315 | package name that we usually use for our example, so |
| 00:00:53,315 --> 00:00:58,720 | edu.gatech. Now we click Next to continue. This brings up this, |
| 00:00:58,720 --> 00:01:01,670 | new window in which we can select our configuration options. |
| 00:01:01,670 --> 00:01:03,510 | We're just not going to change any of those, so we |
| 00:01:03,510 --> 00:01:06,600 | just click Next again. More options here. So for example, |
| 00:01:06,600 --> 00:01:09,725 | you can select the foreground. You can select whether you want to |
| 00:01:09,725 --> 00:01:12,120 | trim the surrounding black space for your application. You can |
| 00:01:12,120 --> 00:01:15,780 | select the icons again. We're just going to keep the default values. |
| 00:01:15,780 --> 00:01:18,090 | And, we're going to move forward. The next thing we can do |
| 00:01:18,090 --> 00:01:21,170 | is to choose the type of activity that we want to create. |
| 00:01:21,170 --> 00:01:23,600 | And, in this case, we're going to go with a blank activity. |
| 00:01:23,600 --> 00:01:26,800 | And, this leads us to the last screen of the wizard in |
| 00:01:26,800 --> 00:01:29,650 | which we can pick the activity name. We're fine with Main |
| 00:01:29,650 --> 00:01:32,690 | Activity. You can choose the name for the layout and the navigation |
| 00:01:32,690 --> 00:01:35,890 | type. We're just going to keep none for the navigation type. And we |
| 00:01:35,890 --> 00:01:41,150 | click Finish. So at this point our app and initial activity gets created. |
| 00:01:41,150 --> 00:01:43,162 | So now you can see that our Android project has |
| 00:01:43,162 --> 00:01:46,690 | been created, so we can click here and expand the project |
| 00:01:46,690 --> 00:01:48,810 | and see the content of the project. As you can |
| 00:01:48,810 --> 00:01:52,420 | see here, we have a source folder that contains our package |
| 00:01:52,420 --> 00:01:55,570 | and main activity. We have the libraries required for Android, |
| 00:01:55,570 --> 00:01:59,430 | an assets folder, the binary folder where our compiled code will |
| 00:01:59,430 --> 00:02:03,160 | go. Then the libraries, in particular the Android support library. |
| 00:02:03,160 --> 00:02:06,880 | And finally, a directory with all the resources for my project. |
| 00:02:06,880 --> 00:02:09,889 | So, just for example, the icons for the project, and here |
| 00:02:09,889 --> 00:02:12,380 | want to point out a few things. So, I'm going to open the |
| 00:02:12,380 --> 00:02:16,280 | layout folder and here you can see that there's a layout file |
| 00:02:16,280 --> 00:02:19,830 | for the main activity. It's in XML format. So if I click |
| 00:02:19,830 --> 00:02:22,040 | and open this file, I can see that we have two views |
| 00:02:22,040 --> 00:02:26,230 | of this file, a graphical layout view, and, an XML view. So, |
| 00:02:26,230 --> 00:02:28,570 | the nice thing about this is that, with the visual editor I |
| 00:02:28,570 --> 00:02:32,430 | can actually drag and drop widgets into my layout, into my activity. |
| 00:02:32,430 --> 00:02:35,210 | And then those will be automatically reflected in the XML |
| 00:02:35,210 --> 00:02:38,540 | view. So, next I'd like to look at the strings.xml file in the |
| 00:02:38,540 --> 00:02:41,480 | values folder. So, this is the file that contains all of |
| 00:02:41,480 --> 00:02:44,610 | the strings that are defined within your application. So, it's a |
| 00:02:44,610 --> 00:02:47,400 | centralized place where you can change the strings for your |
| 00:02:47,400 --> 00:02:50,760 | app. So, next I want to look at the Android manifest file |
| 00:02:50,760 --> 00:02:53,610 | which is something that we discussed in our lesson. So, basically, |
| 00:02:53,610 --> 00:02:57,550 | this is the file that defines the structure and some configuration |
| 00:02:57,550 --> 00:03:00,522 | options for our app. So, now let's go back to our |
| 00:03:00,522 --> 00:03:04,260 | main activity layout. Let me make this full screen so that we |
| 00:03:04,260 --> 00:03:07,210 | can see better, and zoom in a little bit. Let's go |
| 00:03:07,210 --> 00:03:10,670 | to graphical layout, by default it will just have a hello world |
| 00:03:10,670 --> 00:03:13,230 | string here, so we're just going to delete that. What we need |
| 00:03:13,230 --> 00:03:16,320 | first is a text view So I'm going to take the text view |
| 00:03:16,320 --> 00:03:19,110 | and drag it here. Then I can change the text in this |
| 00:03:19,110 --> 00:03:22,630 | text view by using the property window here on the right and |
| 00:03:22,630 --> 00:03:25,460 | put the text distance here and as you can see that gets |
| 00:03:25,460 --> 00:03:28,840 | reflected in the GUI. Now we're going to add a text field, a numeric |
| 00:03:28,840 --> 00:03:31,790 | text field in particular. Here it is, we want to use one with |
| 00:03:31,790 --> 00:03:35,500 | decimal values. And as you can see here, you can also check what's |
| 00:03:35,500 --> 00:03:38,280 | the distance between the different widgets. And as you can see, each |
| 00:03:38,280 --> 00:03:41,920 | of these elements has got an assigned ID, which you can see here |
| 00:03:41,920 --> 00:03:44,376 | on the right. And if you want, you can go and change |
| 00:03:44,376 --> 00:03:47,820 | that ID. And the ID is then used within the application to refer |
| 00:03:47,820 --> 00:03:50,260 | to this element. In this case, we're going to call it |
| 00:03:50,260 --> 00:03:52,860 | text1. So if you change that, Android will ask you whether |
| 00:03:52,860 --> 00:03:56,340 | you want to update all of the references to this element, because |
| 00:03:56,340 --> 00:03:59,430 | you changed its ID. So let's say Yes in this case, and |
| 00:03:59,430 --> 00:04:02,870 | that will change all the XML and Java resources accordingly. Now |
| 00:04:02,870 --> 00:04:06,850 | that we added this, let's add some radio buttons to our activity. |
| 00:04:06,850 --> 00:04:10,410 | We can do that from our form widgets set of entries. So |
| 00:04:10,410 --> 00:04:12,860 | in particular here you can see that we have the radio button |
| 00:04:12,860 --> 00:04:16,019 | group, so we just place it at the appropriate distance from |
| 00:04:16,019 --> 00:04:18,649 | the other widgets. So, now let's go and check out our |
| 00:04:18,649 --> 00:04:22,040 | XML view, of the layout and as you can see, |
| 00:04:22,040 --> 00:04:24,610 | all the changes that we made, all the elements that we added, |
| 00:04:24,610 --> 00:04:28,650 | are now reflected automatically, as I said, into the XML view. |
| 00:04:28,650 --> 00:04:32,420 | So, you can also change the properties and attributes of these elements |
| 00:04:32,420 --> 00:04:35,214 | here and they will be reflected in the graphical layout, as |
| 00:04:35,214 --> 00:04:37,960 | well. So, for example in this case, let's imagine that we want |
| 00:04:37,960 --> 00:04:40,350 | to delete the last radio button. So we can do |
| 00:04:40,350 --> 00:04:44,330 | it here in the XML file. Let's give some names at |
| 00:04:44,330 --> 00:04:47,580 | the first radio button. Let's call it miles and the second |
| 00:04:47,580 --> 00:04:50,970 | radio button we will give it the name kilometers. So now, let's |
| 00:04:50,970 --> 00:04:54,100 | see how this is reflected into our graphical layout. As |
| 00:04:54,100 --> 00:04:57,210 | you can see, we have only two radio buttons, as expected. |
| 00:04:57,210 --> 00:04:59,920 | And the labels for these radio buttons are miles and kilometers. |
| 00:04:59,920 --> 00:05:02,900 | At this point, let's try to run this on our emulator. |
| 00:05:02,900 --> 00:05:04,220 | So to do that, we have to go to the |
| 00:05:04,220 --> 00:05:07,290 | menu up there and select the virtual device that we |
| 00:05:07,290 --> 00:05:10,176 | created earlier, the one for the Nexus 4. At this |
| 00:05:10,176 --> 00:05:13,043 | point, to run it, we minimize again our windows so that |
| 00:05:13,043 --> 00:05:16,956 | we can go to the package explorer. We select Converter>Run |
| 00:05:16,956 --> 00:05:21,940 | As>Android Application. And when we do that, Eclipse will deploy |
| 00:05:21,940 --> 00:05:25,380 | our application on the emulator and will run it there. |
| 00:05:25,380 --> 00:05:27,970 | And before the emulator is actually launched you will get this |
| 00:05:27,970 --> 00:05:30,470 | option in which you can decide whether you want to monitor |
| 00:05:30,470 --> 00:05:33,700 | logcat or not and what logcat basically does is |
| 00:05:33,700 --> 00:05:37,680 | to show you logs from the emulator within the IDE. So |
| 00:05:37,680 --> 00:05:40,670 | normally you might want to say yes to see what's happening inside |
| 00:05:40,670 --> 00:05:42,700 | the emulator. As you can see, now we have the logcat |
| 00:05:42,700 --> 00:05:46,120 | view down there. We're going to maximize it. You can see |
| 00:05:46,120 --> 00:05:49,850 | there's some information about the emulator. So now let's look at |
| 00:05:49,850 --> 00:05:52,980 | our console. Let's change to the Android console. And if you look |
| 00:05:52,980 --> 00:05:55,200 | at the output here on the console you can see that our |
| 00:05:55,200 --> 00:05:58,400 | activity has been started so we can switch to the emulator to |
| 00:05:58,400 --> 00:06:01,680 | see how our activity running. And in the device, you can see |
| 00:06:01,680 --> 00:06:04,590 | that we have the widgets that we added. So we have the distance, |
| 00:06:04,590 --> 00:06:07,440 | we have the two radio buttons and what we can do here, |
| 00:06:07,440 --> 00:06:11,140 | we can enter an actual value. Like for example, two, three, four, five. |
| 00:06:11,140 --> 00:06:13,900 | And the way we want our application to behave, is that when |
| 00:06:13,900 --> 00:06:16,230 | we click kilometers, the application will |
| 00:06:16,230 --> 00:06:18,220 | do the conversion automatically, and vice versa. |
| 00:06:18,220 --> 00:06:21,230 | So let's go and implement this functionality in our |
| 00:06:21,230 --> 00:06:25,170 | app. So, to do that, I'm going to minimize the console. |
| 00:06:25,170 --> 00:06:27,880 | going to go back to my IDE, and I'm going to |
| 00:06:27,880 --> 00:06:31,650 | select again, Activity Main. In this case, I want to have |
| 00:06:31,650 --> 00:06:34,080 | the XML view. And the way which I can |
| 00:06:34,080 --> 00:06:37,350 | do this, is by connecting my widget to the code |
| 00:06:37,350 --> 00:06:39,610 | and I do that by adding this entry here, |
| 00:06:39,610 --> 00:06:43,580 | in which I say that onClick so the onClick property |
| 00:06:43,580 --> 00:06:46,710 | is linked to the handleClick method and I'm going to |
| 00:06:46,710 --> 00:06:50,635 | copy this and do exactly the same for the second radio |
| 00:06:50,635 --> 00:06:53,270 | button. So what that means is that every time you click |
| 00:06:53,270 --> 00:06:57,020 | the radio button, handleClick will be invoked. So now we need |
| 00:06:57,020 --> 00:07:00,260 | to implement the handleClick method in our activity. So let's go |
| 00:07:00,260 --> 00:07:02,610 | back to the main activity, to the Java code. And as |
| 00:07:02,610 --> 00:07:05,310 | you can see, this is the code that was auto generated. |
| 00:07:05,310 --> 00:07:08,820 | So first I'm going to be writing the signature of my callback |
| 00:07:08,820 --> 00:07:11,780 | on my handle, so the name is handleClick, and the |
| 00:07:11,780 --> 00:07:14,950 | parameter is a parameter of type view. Next, we're going to |
| 00:07:14,950 --> 00:07:18,700 | check the status of a radio button that's been clicked. |
| 00:07:18,700 --> 00:07:21,350 | So we want to see whether it's checked or unchecked, and |
| 00:07:21,350 --> 00:07:24,500 | I do this using the method isChecked of the view |
| 00:07:24,500 --> 00:07:26,960 | object, of the view class. Next we want to get a |
| 00:07:26,960 --> 00:07:30,200 | reference to our text box, and we're going to do this |
| 00:07:30,200 --> 00:07:33,850 | using the ID for the text box that I mentioned before. |
| 00:07:33,850 --> 00:07:35,920 | And we're not looking at all the details of this code, |
| 00:07:35,920 --> 00:07:38,290 | but there's something I want to clarify here, is that we're |
| 00:07:38,290 --> 00:07:41,760 | using this class R here, that we haven't mentioned before. And |
| 00:07:41,760 --> 00:07:45,435 | R is basically a static class that gets associated to your Android |
| 00:07:45,435 --> 00:07:48,680 | app, and contains references to all of your resources. So for |
| 00:07:48,680 --> 00:07:52,260 | example in this case we're using R to access the IDs and |
| 00:07:52,260 --> 00:07:55,510 | within these IDs the text1 ID which is the one |
| 00:07:55,510 --> 00:07:59,320 | corresponding to our text entry. And now that we have a reference |
| 00:07:59,320 --> 00:08:02,070 | to the text entry, we can actually use that to read |
| 00:08:02,070 --> 00:08:05,320 | the value that was entered by the user in that entry |
| 00:08:05,320 --> 00:08:08,450 | and we're going to use the method parseDouble of the Double |
| 00:08:08,450 --> 00:08:11,490 | class to do that. So we're going to get from the text |
| 00:08:11,490 --> 00:08:14,780 | entry the text. We're going to convert it to a string, and |
| 00:08:14,780 --> 00:08:17,520 | then we're going to parse it into a double. At this point, |
| 00:08:17,520 --> 00:08:20,340 | what we need to do is to figure out which radio |
| 00:08:20,340 --> 00:08:24,510 | button was actually clicked. If you remember, we associated the same method |
| 00:08:24,510 --> 00:08:28,010 | handleClick to both radio buttons. So this method gets |
| 00:08:28,010 --> 00:08:31,510 | invoked when either one is clicked. So in order to be |
| 00:08:31,510 --> 00:08:34,299 | able to distinguish between the two, and in order to know |
| 00:08:34,299 --> 00:08:36,549 | which one was actually clicked, what we need to do is |
| 00:08:36,549 --> 00:08:39,159 | to get the ID of the element that was clicked. |
| 00:08:39,159 --> 00:08:41,679 | And we do that by using the method, getId of |
| 00:08:41,679 --> 00:08:45,380 | the view object. Now to match the ID, we use again, |
| 00:08:45,380 --> 00:08:49,520 | class R, as before. And in particular, ID of class R, |
| 00:08:49,520 --> 00:08:52,900 | so we have the first, ID which is our ID radio0, |
| 00:08:52,900 --> 00:08:55,720 | which is the one corresponding to miles. So now we're |
| 00:08:55,720 --> 00:08:58,720 | going to use the value that we set before and if |
| 00:08:58,720 --> 00:09:01,750 | check is true. So if the radio button corresponding to the |
| 00:09:01,750 --> 00:09:05,030 | miles was actually clicked, that means that we are converting |
| 00:09:05,030 --> 00:09:08,560 | the value that was in the text entry from kilometers to |
| 00:09:08,560 --> 00:09:12,001 | miles. So we're going to use this method kilometer to miles which |
| 00:09:12,001 --> 00:09:14,820 | we haven't written yet and we're going to pass the distance which |
| 00:09:14,820 --> 00:09:18,110 | is the current value in the text entry to this method. This |
| 00:09:18,110 --> 00:09:21,170 | method will return the corresponding value in miles and then we'll use |
| 00:09:21,170 --> 00:09:24,230 | that to update the text in the text field. So at this |
| 00:09:24,230 --> 00:09:27,030 | point our conversion would be complete. So at this point we need |
| 00:09:27,030 --> 00:09:29,820 | to handle the second case. Which is of course the case in |
| 00:09:29,820 --> 00:09:33,590 | which we click the other radio button. So the one with id |
| 00:09:33,590 --> 00:09:36,960 | radio1, also here, we make sure that the radio button is |
| 00:09:36,960 --> 00:09:40,130 | actually checked. And if it is, in this case we are converting |
| 00:09:40,130 --> 00:09:43,450 | from miles, to kilometers. So we do exactly the same thing |
| 00:09:43,450 --> 00:09:46,130 | that we did before, but we invoke a different method. So |
| 00:09:46,130 --> 00:09:49,730 | in this case we invoke the method miles to kilometers, again |
| 00:09:49,730 --> 00:09:53,310 | passing the distance as an input. At this point we're almost done, |
| 00:09:53,310 --> 00:09:56,010 | so we're just going to clean up the code a bit here, |
| 00:09:56,010 --> 00:09:59,150 | then I'm just going to copy and paste in the two methods, |
| 00:09:59,150 --> 00:10:02,200 | the kilometer to miles, and the miles to kilometer, in the |
| 00:10:02,200 --> 00:10:05,100 | interest of time. So I'm not going to write them in real time. |
| 00:10:05,100 --> 00:10:07,140 | And as you can see, the first method performed the |
| 00:10:07,140 --> 00:10:10,960 | conversion from miles to kilometers by using the proper conversion |
| 00:10:10,960 --> 00:10:14,630 | factor and returning a string value for the converted value |
| 00:10:14,630 --> 00:10:18,400 | and the second method does the opposite. So converts kilometers to |
| 00:10:18,400 --> 00:10:20,850 | miles. So at this point we're ready to run our |
| 00:10:20,850 --> 00:10:23,620 | code. To do that we use the run menu here, |
| 00:10:23,620 --> 00:10:26,680 | which allows to run the Converter application and as we |
| 00:10:26,680 --> 00:10:30,380 | did before, we can go and look at the console |
| 00:10:30,380 --> 00:10:32,550 | to figure out what's going on and as you can see |
| 00:10:32,550 --> 00:10:36,170 | the console tells us that our app is being installed on the |
| 00:10:36,170 --> 00:10:40,250 | emulator, successful install, and after it's done we can switch to |
| 00:10:40,250 --> 00:10:43,790 | our emulator and we can see our application running as we did |
| 00:10:43,790 --> 00:10:47,100 | before. But in this case, with a complete code behind it. |
| 00:10:47,100 --> 00:10:50,160 | So here we can enter, for example, our distance in miles, so |
| 00:10:50,160 --> 00:10:52,780 | let's just put one mile to see how the conversion works |
| 00:10:52,780 --> 00:10:55,890 | in this case and as you can see, the distance gets converted |
| 00:10:55,890 --> 00:10:58,240 | back and forth correctly. So, now let's use a |
| 00:10:58,240 --> 00:11:01,260 | slightly larger number. So for example, let's use the |
| 00:11:01,260 --> 00:11:04,880 | distance between the Earth and the moon and we |
| 00:11:04,880 --> 00:11:08,090 | can convert that from miles to kilometers and back |
| 00:11:08,090 --> 00:11:11,400 | to miles again. So, we have successfully written, deployed |
| 00:11:11,400 --> 00:11:15,018 | and ran in an emulator, our first Android app. |
| 00:11:15,018 --> 00:11:17,040 | And notice that you can run exactly the same |
| 00:11:17,040 --> 00:11:17,040 | app on any of your mobile devices, if you want. |