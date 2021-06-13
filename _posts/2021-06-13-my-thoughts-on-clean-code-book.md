---
title: "My thoughts on Clean Code Book"
layout: post
---

## Clean Code
Clean code is a book about the best practices to write *clean code*. It is written by Robert C. Martin (aka Uncle Bob Martin) in 2008. It is accepted as a must read book if you want to learn how not to write bad code. 

<center>
    <figure>
    <img src="/assets/images/clean_code_pic1.jpeg" alt="clean code" width="400"/>
    <figcaption>Reading Clean Code on my Kobo.</figcaption>
    </figure>
</center>

I will confess that I did not (could not) read all the chapters of the book. The code examples in the book are in java and my experience on java is limited. This makes reading a bit difficult. For this reason, there were times that I focused more on the concept instead of code examples. There are seventeen chapters in the book. 

- Chapter 1: Clean Code  
- Chapter 2: Meaningful Names
- Chapter 3: Functions
- Chapter 4: Comments
- Chapter 5: Formatting
- Chapter 6: Objects and Data Structures
- Chapter 7: Error Handling
- Chapter 8: Boundaries
- Chapter 9: Unit Tests
- Chapter 10: Classes
- Chapter 11: Systems
- Chapter 12: Emergence
- Chapter 13: Concurrency
- Chapter 14: Successive Refinement
- Chapter 15: JUnit Internals
- Chapter 16: Refactoring SerialDate
- Chapter 17: Smells and Heuristics

Chapter 1-5 is must-read where the core-concepts are given. Here, I took it slow to enhance my understanding. Chapter 6-10 is helpful. Chapter 11-17 can be optional, because these concepts are either too java-centric or topics are difficult to follow (to me, it was).

## My quotes and notes

> Yet even in the auto industry, the bulk of the work lies not in manufacturing but in maintenance or its avoidance. 

This is so true. The effort for writing clean code is in fact for the sake of maintenance. The code should be maintainable, and for this it should be clean enough. 

> Learning to write clean code is hard work. 

Not going to speak a lot on this. It is a fact. Learning to write clean code requires writing tons of code, first. What makes software engineering hard is not finishing source code that works but writing clean and maintainable one.

> Code, without tests, is not clean.

Testing is essential. Without proper testing, the code will prone to fail. Whenever there is a change in the source code, it should be tested. Especially in enterprise software application, quality - assurance is vital because bugs should be identified before the customer. Chapter 9 is dedicated for writing clean unit tests. 

> Perhaps an appropriate subtitle would be How to Care for Code.

I guess many people who have read the book will agree on this quote. There is no such a thing like *clean code*. There is always something to improve in the code. Naming of variables and functions, abstractions, comments and formatting are all subject to change in the future if necessary. We should iteratively make the code better and by time it will be clean enough.

> We are constantly reading old code as part of the effort to write new code.

Once a software is written, thereafter, it is all about maintenance and adding features. Whenever we write code, there should be a big amount of effort to make it clean. Because one day, we will go back and read this code again. If we can understand what the code does easily, then it means code is clean. 

### Other quotes.
> Bad code tempts the mess to grow!

If you have questions or comments about this project, feel free to reach me via [twitter](https://twitter.com/earik87).