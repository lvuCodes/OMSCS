# P4L5 Software Refactoring

## P4L5 Software Refactoring

Welcome to **P4L5 Software Refactoring**! This lesson has 20 sections.

To start watching this lesson, click Next at the top of the screen. You may also [download](https://www.dropbox.com/s/e7wcd4l82sd5bz5/CS6300_Lectures.zip?dl=0) this course's videos to watch offline. Remember, you may give feedback on this course experience, report bugs, or submit feature requests to [the feedback form](http://bit.ly/EdLessonsFeedback).

## 1. Software Refactoring Overview

[Video](https://cdnapisec.kaltura.com/p/2019031/sp/201903100/embedIframeJs/uiconf_id/43123921/partner_id/2019031?iframeembed=true&playerId=kaltura_player&entry_id=1_m5l7qtg9)

[[lessons/17-p4l5-software-refactoring/transcripts-md/01-software-refactoring-overview-transcript|transcript]]

This is section 1 of 20 in this lesson.

## 2. Software Refactoring Introduction

[Video](https://cdnapisec.kaltura.com/p/2019031/sp/201903100/embedIframeJs/uiconf_id/43123921/partner_id/2019031?iframeembed=true&playerId=kaltura_player&entry_id=1_li9e3cx9)

[[lessons/17-p4l5-software-refactoring/transcripts-md/02-software-refactoring-introduction-transcript|transcript]]

This is section 2 of 20 in this lesson.

## 3. Software Refactoring Quiz

[Video](https://cdnapisec.kaltura.com/p/2019031/sp/201903100/embedIframeJs/uiconf_id/43123921/partner_id/2019031?iframeembed=true&playerId=kaltura_player&entry_id=1_q7kqhpxm)

[[lessons/17-p4l5-software-refactoring/transcripts-md/03-software-refactoring-quiz-transcript|transcript]]

This is section 3 of 20 in this lesson.

## P4L5 Software Refactoring: Introduction

[[lessons/17-p4l5-software-refactoring/05-introduction/quiz|P4L5 Software Refactoring: Introduction]] · [[lessons/17-p4l5-software-refactoring/05-introduction/answers|answers]] · [[lessons/17-p4l5-software-refactoring/05-introduction/submission|submission]]

## 3. Software Refactoring Quiz (Answer)

[Video](https://cdnapisec.kaltura.com/p/2019031/sp/201903100/embedIframeJs/uiconf_id/43123921/partner_id/2019031?iframeembed=true&playerId=kaltura_player&entry_id=1_2wbfi2ar)

[[lessons/17-p4l5-software-refactoring/transcripts-md/04-software-refactoring-quiz-answer-transcript|transcript]]

This is section 3 of 20 in this lesson.

## 4. Reasons to Refactor

[Video](https://cdnapisec.kaltura.com/p/2019031/sp/201903100/embedIframeJs/uiconf_id/43123921/partner_id/2019031?iframeembed=true&playerId=kaltura_player&entry_id=1_4khux7np)

[[lessons/17-p4l5-software-refactoring/transcripts-md/05-reasons-to-refactor-transcript|transcript]]

This is section 4 of 20 in this lesson.

## 5. History of Refactoring

[Video](https://cdnapisec.kaltura.com/p/2019031/sp/201903100/embedIframeJs/uiconf_id/43123921/partner_id/2019031?iframeembed=true&playerId=kaltura_player&entry_id=1_taaek7k4)

[[lessons/17-p4l5-software-refactoring/transcripts-md/06-history-of-refactoring-transcript|transcript]]

This is section 5 of 20 in this lesson.

## 6. Types of Refactorings

[Video](https://cdnapisec.kaltura.com/p/2019031/sp/201903100/embedIframeJs/uiconf_id/43123921/partner_id/2019031?iframeembed=true&playerId=kaltura_player&entry_id=1_n3sq9eb7)

[[lessons/17-p4l5-software-refactoring/transcripts-md/07-types-of-refactorings-transcript|transcript]]

This is section 6 of 20 in this lesson.

## 7. Collapse Hierarchy

[Video](https://cdnapisec.kaltura.com/p/2019031/sp/201903100/embedIframeJs/uiconf_id/43123921/partner_id/2019031?iframeembed=true&playerId=kaltura_player&entry_id=1_20gym3eg)

[[lessons/17-p4l5-software-refactoring/transcripts-md/08-collapse-hierarchy-transcript|transcript]]

This is section 7 of 20 in this lesson.

## 8. Consolidate Conditional Expression

[Video](https://cdnapisec.kaltura.com/p/2019031/sp/201903100/embedIframeJs/uiconf_id/43123921/partner_id/2019031?iframeembed=true&playerId=kaltura_player&entry_id=1_cvfuqb65)

[[lessons/17-p4l5-software-refactoring/transcripts-md/09-consolidate-conditional-expression-transcript|transcript]]

This is section 8 of 20 in this lesson.

## Consolidate Conditional Expression

The code below is given for this exercise. Work it out on your own, then view the answer video to see if you're correct.

```
public class Employee {
	private boolean isPartTime;
	private int seniority;
	private int monthsDisabled;
	
	public Employee(boolean isPartTime, int seniority, int monthsDisabled) {
		this.isPartTime = isPartTime;
		this.seniority = seniority;
		this.monthsDisabled = monthsDisabled;
	}

	// TODO: add a function here with the signature: public boolean notEligibleForDisability()

	public double disabilityAmount() {
		// TODO: replace these checks with a single function call
		if (seniority < 2)
			return 0;
		if (monthsDisabled > 12)
			return 0;
		if (isPartTime)
			return 0;

		// in a real program, there would be other logic for determining
		// the amount of disability the employee is eligible for here

		// the following is a dummy return value to make the compiler happy
		// and differentiate between the above cases and others
		return 1;
	}

}
```

## 8. Consolidate Conditional Expression (Answer)

[Video](https://cdnapisec.kaltura.com/p/2019031/sp/201903100/embedIframeJs/uiconf_id/43123921/partner_id/2019031?iframeembed=true&playerId=kaltura_player&entry_id=1_vf15hom3)

[[lessons/17-p4l5-software-refactoring/transcripts-md/10-consolidate-conditional-expression-answer-transcript|transcript]]

This is section 8 of 20 in this lesson.

## 9. Decompose Conditionals

[Video](https://cdnapisec.kaltura.com/p/2019031/sp/201903100/embedIframeJs/uiconf_id/43123921/partner_id/2019031?iframeembed=true&playerId=kaltura_player&entry_id=1_yedyi6xx)

[[lessons/17-p4l5-software-refactoring/transcripts-md/11-decompose-conditionals-transcript|transcript]]

This is section 9 of 20 in this lesson.

## 10. Extract Class

[Video](https://cdnapisec.kaltura.com/p/2019031/sp/201903100/embedIframeJs/uiconf_id/43123921/partner_id/2019031?iframeembed=true&playerId=kaltura_player&entry_id=1_z8gejmcx)

[[lessons/17-p4l5-software-refactoring/transcripts-md/12-extract-class-transcript|transcript]]

This is section 10 of 20 in this lesson.

## 11. Inline Class

[Video](https://cdnapisec.kaltura.com/p/2019031/sp/201903100/embedIframeJs/uiconf_id/43123921/partner_id/2019031?iframeembed=true&playerId=kaltura_player&entry_id=1_3qtf82jt)

[[lessons/17-p4l5-software-refactoring/transcripts-md/13-inline-class-transcript|transcript]]

This is section 11 of 20 in this lesson.

## 12. Extract Method

[Video](https://cdnapisec.kaltura.com/p/2019031/sp/201903100/embedIframeJs/uiconf_id/43123921/partner_id/2019031?iframeembed=true&playerId=kaltura_player&entry_id=1_se8zy1ie)

[[lessons/17-p4l5-software-refactoring/transcripts-md/14-extract-method-transcript|transcript]]

This is section 12 of 20 in this lesson.

## 13. Refactoring Demo

[Video](https://cdnapisec.kaltura.com/p/2019031/sp/201903100/embedIframeJs/uiconf_id/43123921/partner_id/2019031?iframeembed=true&playerId=kaltura_player&entry_id=1_r9sc0jq8)

[[lessons/17-p4l5-software-refactoring/transcripts-md/15-refactoring-demo-transcript|transcript]]

This is section 13 of 20 in this lesson.

## 14. Extract Method Refactoring Quiz

[Video](https://cdnapisec.kaltura.com/p/2019031/sp/201903100/embedIframeJs/uiconf_id/43123921/partner_id/2019031?iframeembed=true&playerId=kaltura_player&entry_id=1_5x8lbppu)

[[lessons/17-p4l5-software-refactoring/transcripts-md/16-extract-method-refactoring-quiz-transcript|transcript]]

This is section 14 of 20 in this lesson.

## P4L5 Software Refactoring: Extract Method Refactoring Quiz

[[lessons/17-p4l5-software-refactoring/20-extract-method-refactoring-quiz/quiz|P4L5 Software Refactoring: Extract Method Refactoring Quiz]] · [[lessons/17-p4l5-software-refactoring/20-extract-method-refactoring-quiz/answers|answers]] · [[lessons/17-p4l5-software-refactoring/20-extract-method-refactoring-quiz/submission|submission]]

## 14. Extract Method Refactoring Quiz (Answer)

[Video](https://cdnapisec.kaltura.com/p/2019031/sp/201903100/embedIframeJs/uiconf_id/43123921/partner_id/2019031?iframeembed=true&playerId=kaltura_player&entry_id=1_yorkpmqt)

[[lessons/17-p4l5-software-refactoring/transcripts-md/17-extract-method-refactoring-quiz-answer-transcript|transcript]]

This is section 14 of 20 in this lesson.

## 15. Refactoring Risks

[Video](https://cdnapisec.kaltura.com/p/2019031/sp/201903100/embedIframeJs/uiconf_id/43123921/partner_id/2019031?iframeembed=true&playerId=kaltura_player&entry_id=1_p29i5hxk)

[[lessons/17-p4l5-software-refactoring/transcripts-md/18-refactoring-risks-transcript|transcript]]

This is section 15 of 20 in this lesson.

## 16. Cost of Refactoring

[Video](https://cdnapisec.kaltura.com/p/2019031/sp/201903100/embedIframeJs/uiconf_id/43123921/partner_id/2019031?iframeembed=true&playerId=kaltura_player&entry_id=1_rb311hjn)

[[lessons/17-p4l5-software-refactoring/transcripts-md/19-cost-of-refactoring-transcript|transcript]]

This is section 16 of 20 in this lesson.

## 17. When Not To Refactor

[Video](https://cdnapisec.kaltura.com/p/2019031/sp/201903100/embedIframeJs/uiconf_id/43123921/partner_id/2019031?iframeembed=true&playerId=kaltura_player&entry_id=1_h5327deb)

[[lessons/17-p4l5-software-refactoring/transcripts-md/20-when-not-to-refactor-transcript|transcript]]

This is section 17 of 20 in this lesson.

## 18. Bad Smells

[Video](https://cdnapisec.kaltura.com/p/2019031/sp/201903100/embedIframeJs/uiconf_id/43123921/partner_id/2019031?iframeembed=true&playerId=kaltura_player&entry_id=1_bxp2y1z4)

[[lessons/17-p4l5-software-refactoring/transcripts-md/21-bad-smells-transcript|transcript]]

This is section 18 of 20 in this lesson.

## 19. Bad Smell Examples

[Video](https://cdnapisec.kaltura.com/p/2019031/sp/201903100/embedIframeJs/uiconf_id/43123921/partner_id/2019031?iframeembed=true&playerId=kaltura_player&entry_id=1_2nx7mlmt)

[[lessons/17-p4l5-software-refactoring/transcripts-md/22-bad-smell-examples-transcript|transcript]]

This is section 19 of 20 in this lesson.

## 20. Bad Smell Quiz

[Video](https://cdnapisec.kaltura.com/p/2019031/sp/201903100/embedIframeJs/uiconf_id/43123921/partner_id/2019031?iframeembed=true&playerId=kaltura_player&entry_id=1_aj11q9j9)

[[lessons/17-p4l5-software-refactoring/transcripts-md/23-bad-smell-quiz-transcript|transcript]]

This is section 20 of 20 in this lesson.

## P4L5 Software Refactoring: Bad Smell Quiz

[[lessons/17-p4l5-software-refactoring/28-bad-smell-quiz/quiz|P4L5 Software Refactoring: Bad Smell Quiz]] · [[lessons/17-p4l5-software-refactoring/28-bad-smell-quiz/answers|answers]] · [[lessons/17-p4l5-software-refactoring/28-bad-smell-quiz/submission|submission]]

## 20. Bad Smell Quiz (Answer)

[Video](https://cdnapisec.kaltura.com/p/2019031/sp/201903100/embedIframeJs/uiconf_id/43123921/partner_id/2019031?iframeembed=true&playerId=kaltura_player&entry_id=1_6023iini)

[[lessons/17-p4l5-software-refactoring/transcripts-md/24-bad-smell-quiz-answer-transcript|transcript]]

This is section 20 of 20 in this lesson.
