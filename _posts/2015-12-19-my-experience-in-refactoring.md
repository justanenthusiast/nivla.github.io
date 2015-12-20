---
layout: post
title: My Experience in refactoring
date: 2015-12-20 00:00:00
---

few months ago, I didn’t know the concept of refactoring,  without realize the benefits that I was losing for improve the quality of my code.

Always that I had write code, I’d write functions of 100 lines, too much nested conditionals,  functions names that doesn’t explain very well the meaning of it.

It was something good and normal have that kind of code, the application works and everything is fine but after few months when I come back to the code for change something or add a new feature it was hard, not because the difficult of the feature but for understand what I want to mean in this function or what does this class mean? It wasn’t readable.

I realize all my mistakes when I began to read  the book [ The clean coder ]( http://www.amazon.com/Clean-Coder-Conduct-Professional-Programmers/dp/0137081073/ref=sr_1_2?ie=UTF8&qid=1450624755&sr=8-2&keywords=the+clean+code )
*Thanks uncle ben*.
Read this book pushed me forward how to write better code and the benefits of it.

I learn that my application should be like a book:

**Must tell a history and each function tells a part of the history**

After reading *The clean coder* my next step was read [Refactoring Improving the Design of Existing Code](http://www.amazon.com/Refactoring-Improving-Design-Existing-Code/dp/0201485672/ref=sr_1_1?ie=UTF8&qid=1450625125&sr=8-1&keywords=refactoring+improving+the+design+of+existing+code), thanks *Martin Flower*, I could understand the idea of refactoring.

***Refactoring is improve the quality of the code without changing his behavior***

I learnt very techiques and patterns that I can apply for improve the quality and complexity of the code.

- Extract Method.
- Extract Class
- Replace Type Code with Class
- Replace Parameters with object
- Null Object
- Rename Method

*"Methods should be named in a
way that communicates their intention. A good way to do this is to think what the comment for the
method would be and turn that comment into the name of the method."*

- Replace Conditional with Polymorphism

And too many mores!!. You see the entire catalog [here](http://refactoring.com/catalog/).

**Now the good smell it’s real!**


###Remember
*"When you are refactoring,
your goal is to leave the code computing exactly the same answers it was when you found it.
Nothing more, nothing less."*


###Conclution

I encourage you to read “the clean code” and “Refactoring Improving the Design of Existing Code”. It won't disappoint you.

Apply refactoring whenever you can, if your write something, test it and apply refactoring again until you feel comfortable with the code.
