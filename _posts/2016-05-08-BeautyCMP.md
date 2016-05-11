---
layout: post
section-type: post
title: BeautyCMP
category: java
tags: [ 'code' ]
---

```java
public class BeautyCMP implements Comparable {
    public BeautyCMP(Object you) {
        this.you = you;
    }

    private Object you;

    @Override
    public int compareTo(Object o) {
        if (o == you) {
            return 0;
        } else {
            return 1;
        }
    }
}
```
