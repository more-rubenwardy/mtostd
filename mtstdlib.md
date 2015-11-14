---
title: mtstdlib
layout: default
---

## mtstdlib

### Notes

* mtstdlib is a WIP name for a mod.
* This is a proposal, the mod hasn't actually been written yet.

## Requiring a Group

## check_that

{% highlight lua %}
mtstdlib.check_that("group:group_name")
{% endhighlight %}

After all mods are loaded, it will check whether that group exists. If it doesn't,
then it will through and error (or call the callback)
