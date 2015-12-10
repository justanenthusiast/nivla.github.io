---
layout: post
title:  Lazy explanation about symbols in ruby
date:   2015-11-16  00:00:00
---

I want to explain in brief about symbols. I will resume the list of questions in this.

1. **“What are symbols in ruby?”**

2. **“Advantage of symbols instead of simple string”**

3. **“When I can use symbols in my code”**

**What are Symbols?** 

A ruby symbol is like a string with some peculiarity.

Symbols are immutable. That means that symbols only created once and any part of your code your 

reference that symbol will be call the same reference.

Example
{% highlight ruby %}
‘foo’.object_id # 17687064

‘foo’ .objet_id # 16335432

:foo.object_id  # 396584

:foo.objecT_id  # 396584
{% endhighlight %}
This feature is pretty cool, beside you saves time when comparison, also saves memory, because they are only store once.

Any time you refer your symbol you will be pointing the same slot memory.

“Advantage of symbols instead of simple string””

1. **Performance Benefits**

When two strings are compared, under the ground it must walk both string looking for 

mismatch, when two ruby symbols are compared, it just compared if the numeric 

representation is equal, if so, and then are equals.

If you were to the :name symbol twenty twice in your code, every use of: name would be 

referring to exactly the same object. 

**When I can use symbols in my code**

Any time you want to

If what you are looking for is an identifier to be used internally at your code, you should be using 

symbols.

If you are using rails, you will see symbols a lot around your code.

{% highlight ruby %}
validates ,:lastname, presence: true

validates :name,length:{ minimum: 2}
{% endhighlight %}
*instead of*
{% highlight ruby %}
validates  “name”,presence: true

validates “name”,length:{ minimum: 2}
{% endhighlight %}
both work correctly but I think you already know why symbols are better in this scenario.

