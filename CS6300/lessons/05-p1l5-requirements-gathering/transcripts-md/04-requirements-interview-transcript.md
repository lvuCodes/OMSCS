# CS6300 77 - Requirements Interview

| Timestamp | Content |
|-----------|---------|
| 00:00:00,430 --> 00:00:01,050 | Hi, I'm Lauren. |
| 00:00:01,050 --> 00:00:01,990 | >> Hi, I'm Alvin. |
| 00:00:01,990 --> 00:00:06,470 | >> I'm an instructor at a university nearby and I've been noticing that when |
| 00:00:06,470 --> 00:00:09,700 | my students write their essays, they have |
| 00:00:09,700 --> 00:00:13,100 | very long, very wordy sentences and I would |
| 00:00:13,100 --> 00:00:17,600 | like to develop some kind of tool that they can use to keep track of |
| 00:00:17,600 --> 00:00:20,440 | this and maybe perfect their writing style. |
| 00:00:20,440 --> 00:00:21,410 | Do you think that's something you could do? |
| 00:00:21,410 --> 00:00:25,850 | >> I think so. Let's start by helping me get acquainted with the students |
| 00:00:25,850 --> 00:00:29,620 | in the class. So how many students do we have in this class typically? |
| 00:00:29,620 --> 00:00:34,000 | >> Usually about 45 per unit, but I can have up to six units a semester. |
| 00:00:34,000 --> 00:00:36,420 | >> 45 students, and six sections per |
| 00:00:36,420 --> 00:00:39,220 | semester. That's a fairly reasonable size. So, |
| 00:00:39,220 --> 00:00:42,790 | do you know anything about what the students are using as far as computers go? |
| 00:00:42,790 --> 00:00:46,640 | >> I don't know what kind of computers they're using. And they |
| 00:00:46,640 --> 00:00:50,960 | could be, I don't know, anywhere from having no tech experience to |
| 00:00:50,960 --> 00:00:52,200 | being pretty proficient. |
| 00:00:52,200 --> 00:00:54,930 | >> Do you know anything about how |
| 00:00:54,930 --> 00:00:57,350 | familiar the students are with computers in general? |
| 00:00:57,350 --> 00:00:59,540 | >> I'm sure we have some people on the low end that have |
| 00:00:59,540 --> 00:01:01,430 | never done any type of programming, and |
| 00:01:01,430 --> 00:01:03,680 | then some people who are pretty self-sufficient. |
| 00:01:03,680 --> 00:01:07,210 | >> Okay, and I guess my last question related to |
| 00:01:07,210 --> 00:01:10,170 | the students is, what is the students actually submitting to you. |
| 00:01:10,170 --> 00:01:14,080 | >> They've been sending just raw text files via email to me. |
| 00:01:14,080 --> 00:01:16,660 | >> So from the sounds of things |
| 00:01:16,660 --> 00:01:19,140 | we have a fairly broad, I guess base |
| 00:01:19,140 --> 00:01:23,100 | of students to work with, both in technical proficiency |
| 00:01:23,100 --> 00:01:27,180 | as well as their operating system environments potentially. |
| 00:01:27,180 --> 00:01:29,420 | So I think what we'll probably do to start |
| 00:01:29,420 --> 00:01:33,270 | off with is make a command line, Java |
| 00:01:33,270 --> 00:01:36,760 | based tool. That the students can run and we'll |
| 00:01:36,760 --> 00:01:39,910 | give them a fair amount of you know, documentation |
| 00:01:39,910 --> 00:01:41,690 | on how to use the tool. And I expect |
| 00:01:41,690 --> 00:01:45,090 | that there will be a lot of little error conditions that may happen |
| 00:01:45,090 --> 00:01:49,320 | that we want to produce a reasonably friendly message were anything to go wrong. |
| 00:01:49,320 --> 00:01:50,480 | >> Yeah. That'd be great. |
| 00:01:50,480 --> 00:01:54,750 | >> So, a little bit more, I guess about |
| 00:01:54,750 --> 00:01:59,820 | the actual essay itself, its submission, what constitutes a word? |
| 00:01:59,820 --> 00:02:03,190 | >> I really only care about the longer words, so, is there a |
| 00:02:03,190 --> 00:02:06,140 | way that we can only count words that are maybe above three letters? |
| 00:02:06,140 --> 00:02:06,830 | >> I think |
| 00:02:06,830 --> 00:02:08,508 | that's something we can do. And I think |
| 00:02:08,508 --> 00:02:10,030 | that because you seem a little bit unsure |
| 00:02:10,030 --> 00:02:11,540 | we might be able to have that be |
| 00:02:11,540 --> 00:02:13,820 | a little bit more flexible than we otherwise would. |
| 00:02:13,820 --> 00:02:14,500 | >> Great. |
| 00:02:14,500 --> 00:02:18,330 | >> What does a sentence mean to you? Is it kind of flexible? |
| 00:02:18,330 --> 00:02:21,280 | >> I would say anything that ends in a period or |
| 00:02:21,280 --> 00:02:25,870 | even a question mark. Maybe even an exclamation mark. or, something |
| 00:02:25,870 --> 00:02:28,760 | even, maybe even with a comma or semi-colon. I really only |
| 00:02:28,760 --> 00:02:32,370 | care about the sentences that aren't grammatically correct and are too long. |
| 00:02:32,370 --> 00:02:35,180 | >> I think we can probably make that a little bit more flexible too |
| 00:02:35,180 --> 00:02:37,520 | so that way, you can kind of say we're going to, or you want to include them. |
| 00:02:37,520 --> 00:02:38,020 | >> Mm-hm. |
| 00:02:38,020 --> 00:02:41,786 | >> So maybe, sounds like you are little bit on the fence |
| 00:02:41,786 --> 00:02:45,100 | about whether or not say, a comma should be considered a sentence. |
| 00:02:45,100 --> 00:02:45,130 | >> Mm. |
| 00:02:45,130 --> 00:02:46,370 | >> Entirely on its own or not. So we |
| 00:02:46,370 --> 00:02:51,880 | can probably make that a little bit configurable as well. |
| 00:02:51,880 --> 00:02:56,510 | And so, just to confirm the actual end result to |
| 00:02:56,510 --> 00:02:59,870 | the student is the average number of words per sentence? |
| 00:02:59,870 --> 00:03:01,610 | >> Yeah, yeah that'd be fine. |
| 00:03:01,610 --> 00:03:07,430 | >> Okay, overall to start off with, looks like we have some |
| 00:03:07,430 --> 00:03:10,280 | sort of customization of the word length that we want to look for. |
| 00:03:10,280 --> 00:03:12,000 | >> Mm-hm. Yeah. |
| 00:03:12,000 --> 00:03:14,650 | >> We have some kind of variability in |
| 00:03:14,650 --> 00:03:17,880 | what we want to have as acceptable sentence structure. |
| 00:03:17,880 --> 00:03:24,570 | So, periods, question marks, semicolons, things like that. And, the end result |
| 00:03:24,570 --> 00:03:27,260 | to the student is if we're successful, they'll get the average number of |
| 00:03:27,260 --> 00:03:31,060 | words per sentence. Otherwise we tell them something a little bit helpful to |
| 00:03:31,060 --> 00:03:33,240 | kind of put them on the right track to use the tool correctly. |
| 00:03:33,240 --> 00:03:35,850 | >> Yeah that's the error codes right? |
| 00:03:35,850 --> 00:03:38,150 | >> Hopefully not error codes but something a little bit nicer. |
| 00:03:38,150 --> 00:03:39,800 | >> [LAUGH] Okay. |
| 00:03:39,800 --> 00:03:41,150 | >> So I think I have enough to |
| 00:03:41,150 --> 00:03:43,440 | get started and produce something that's you know, |
| 00:03:43,440 --> 00:03:47,150 | a reasonable I guess, rough draft. Of something |
| 00:03:47,150 --> 00:03:48,700 | that you can use to help your class out. |
| 00:03:48,700 --> 00:03:49,590 | >> Great. Thank you. |
| 00:03:49,590 --> 00:03:49,590 | >> Thank you. |