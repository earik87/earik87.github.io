---
title: "My thoughts on Clean Code"
layout: post
---

Clean code is a book about the best practices on how to write *clean code*. It is written by Robert C. Martin (aka Uncle Bob Martin) in 2008, and became a classic. I enjoyed reading it and wanted to share my thoughts with quotes on the book.

<center>
    <figure>
    <img src="/assets/images/clean_code_pic1.jpeg" alt="clean code" width="400"/>
    <figcaption>Reading Clean Code on my Kobo.</figcaption>
    </figure>
</center>

I would recommend to review java language before reading this book. The code examples in the book are in java and concepts are java-centric. Plus, get ready to see bunch of code blocks in the book.

## My quotes and notes

> Yet even in the auto industry, the bulk of the work lies not in manufacturing but in maintenance or its avoidance. 

This is so true. The effort for writing clean code is in fact for the sake of maintenance. The code should be maintainable, and for this it must be clean.

> Learning to write clean code is hard work. 

Not going to speak a lot on this. It is a fact. Learning to write clean code requires writing tons of code. What makes software engineering hard is not finishing source code that works but writing clean and maintainable one.

> Code, without tests, is not clean.

Testing is essential. Without proper testing, the code will prone to fail. Whenever there is a change in the source code, it should be tested. Especially in enterprise software application, quality - assurance is vital because bugs should be identified before the customer. Chapter 9 is dedicated for writing clean unit tests. 

> Perhaps an appropriate subtitle would be How to Care for Code.

I guess many people who have read the book will agree on this quote. There is no such a thing like *clean code* because there is always something to improve. Naming of variables and functions, abstractions, comments and formatting are all subject to change in the future if necessary. We should iteratively make the code better and everytime we touch the code, it should become cleaner.

> We are constantly reading old code as part of the effort to write new code.

If we analyze the time we spend on writing and reading the code, reading will be dominant over writing. This is another reason why we should write clean code. Because we are going to read it later.

### Other quotes.
> Bad code tempts the mess to grow!

If you have questions or comments about this project, feel free to reach me via [twitter](https://twitter.com/earik87).