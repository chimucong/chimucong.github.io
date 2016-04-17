---
layout: post
section-type: post
title: Say I Love You
category: java
tags: [ 'code' ]
---

```java
public void speak() {
    try {
        me.say("I love you");
    } catch (Exception heartBeatingTooFast) {
        me.rest();
        speak();
    }
}
```
