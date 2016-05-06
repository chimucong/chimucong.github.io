---
layout: post
section-type: post
title: Inner Class
category: java
tags: [ 'code' ]
---

```java
public class Me {
    private Heart heart;
    private You you;

    public Me() {
        heart = new Heart();
    }

    public You getYou() {
        if (you == null) {
            you = new You();
        }
        return you;
    }

    class You {
        public Heart getBoyfriendHeart() {
            return heart;
        }
    }
}
```
