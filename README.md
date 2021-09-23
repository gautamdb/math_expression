# math_expression
A class to define "mathematical expressions", so that computers can understand them the same way human mathematicians would.

This repository is under construction.

I am considering using the programming language "Raku", so I am currently reading the book "Think Raku", freely available [here](https://greenteapress.com/wp/think-perl-6/).

## My thoughts while reading the book "Think Raku"
I think I chose well while considering the programming language "Raku". After all, I want the result of 0.3-0.2-0.1 to be zero, and according to the book, this is not naturally the case in Java, C and Python. So if I want a foundation for a system describing theoretical mathematics, the "numerical infrastructure" in Raku seems pretty good.

Because any unicode characters can be used in variable names, it would be possible to write the entire code in german, and use ä,ö,ü,ß,Ä,Ö,Ü without a problem wherever needed. :-)

Raku is a programming language where "0.3-0.2-0.1 == 0" is true, and not only approximately true. On the other hand, even in Raku, "pi / 4" is only approximately the same as "sqrt(2)/2".

```raku
say (1/sqrt(2) == sqrt(2)/2);
say (1/sqrt(2) == sin(pi/4));
say (sin(pi/4) == sqrt(2)/2);
```
