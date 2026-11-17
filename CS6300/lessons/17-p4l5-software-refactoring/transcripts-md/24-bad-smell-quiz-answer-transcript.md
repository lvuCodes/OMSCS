# CS6300 353 - Bad Smell Quiz Solution

| Timestamp | Content |
|-----------|---------|
| 00:00:00,110 --> 00:00:03,090 | So let's look at this one by one. The fact the program takes |
| 00:00:03,090 --> 00:00:06,620 | too long to execute is not really a bad smell. It probably indicates |
| 00:00:06,620 --> 00:00:08,800 | some problem with the code and the fact that we might need to |
| 00:00:08,800 --> 00:00:11,420 | modify the code to make it more efficient, but it's not something that |
| 00:00:11,420 --> 00:00:14,030 | we will normally classify it as a bad smell, so we're not going to |
| 00:00:14,030 --> 00:00:17,850 | mark it. The second one, conversely, is definitely a bad smell. The fact |
| 00:00:17,850 --> 00:00:21,700 | that the method is too long is a typical example of bad smell |
| 00:00:21,700 --> 00:00:25,000 | and one in which we might want to apply some refactoring, for example, |
| 00:00:25,000 --> 00:00:26,450 | the extract method or the |
| 00:00:26,450 --> 00:00:29,240 | decompose conditional refactorings. There's definitely |
| 00:00:29,240 --> 00:00:32,159 | nothing wrong with the fact that the classes cat and dog |
| 00:00:32,159 --> 00:00:35,600 | are subclasses of class animal. Actually, that sounds pretty appropriate, so |
| 00:00:35,600 --> 00:00:38,270 | this is not a problem and definitely not a bad smell. |
| 00:00:38,270 --> 00:00:40,990 | Whereas the fact that every time we modify method M1, |
| 00:00:40,990 --> 00:00:44,210 | we also need to modify some other method M2 is |
| 00:00:44,210 --> 00:00:46,690 | a typical example of bad smell. So this can actually be |
| 00:00:46,690 --> 00:00:50,590 | considered a specific example of what we just called "shotgun surgery." |
| 00:00:50,590 --> 00:00:52,500 | So it is a case in which we might want to |
| 00:00:52,500 --> 00:00:52,500 | use, for instance, the move method refactoring to fix the issue. |