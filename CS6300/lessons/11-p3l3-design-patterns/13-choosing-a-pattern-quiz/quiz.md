# P3L3 Design Patterns: Choosing a Pattern Quiz

[[lessons/11-p3l3-design-patterns/13-choosing-a-pattern-quiz/quiz|quiz]] · [[lessons/11-p3l3-design-patterns/13-choosing-a-pattern-quiz/answers|answers]] · [[lessons/11-p3l3-design-patterns/13-choosing-a-pattern-quiz/submission|submission]]

## Question 1

Imagine that you have to write a class that can have one instance only.

Which of the design pattern that we've discussed is most appropriate?

- [ ] Factory
- [ ] Visitor
- [ ] Proxy
- [ ] Strategy

## Question 2

Imagine that you have to write a class that can have one instance only. Using one of the design patterns that we discussed in this lesson, write the code of a class with only one method (except for possible constructors) that satisfy this requirement.

Make sure to call the class Singleton.

```
public class Singleton {
    private _A_  _B_ instance;
    _C_ Singleton() { }

    public _D_ _E_ factory() {
        if(instance==null) {
           instance = new Singleton();
        }
        return _F_;
    }
}
```

**A:**<br>**B:**<br>**C:**<br>**D:<br>E:<br>F:**
