---
layout: post
section-type: post
title: class Person
category: java
tags: [ 'code' ]
---

```java
public class Person {
    private Person lover;

    public Person() {
    }

    public Person(Person lover) {
        this.lover = lover;
    }

    public void setLover(Person lover) {
        this.lover = lover;
    }

    public static void main(String[] args) {
        Person you = new Person();
        Person me = new Person(you);
        you.setLover(me);
    }
}
```
