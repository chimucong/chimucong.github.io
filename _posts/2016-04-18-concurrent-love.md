---
layout: post
section-type: post
title: Concurrent Love
category: Erlang
tags: [ 'code' ]
---

```erlang
concurrent_love() ->
  Seq = lists:seq(1, 9),
  Task_List = lists:map(
    fun(_) ->
      fun() ->
        io:format("I Love You.~n")
      end
    end,
    Seq),
  lists:foreach(fun(Task) -> spawn(Task) end, Task_List).
```
