# TeX-82

This respository contains ports of TeX-82 to various languages; it is an attempt to answer "if TeX were written today,
what would it look like?"

Obviously, there's no answer for that question; Knuth himself might not even know.  He once claimed he picked Pascal
because it was "everyone's second favorite language."  What might that be today? Python? C++? C#? TypeScript?  Rust?
(I've intentionally omitted C because just about everthing it can do, C++ can do so much better.)

What makes this project unique is that a primary goal is to retain the original structure of **tex.web** as much as possible.
Why?  Well, it is one of the few (only?) programs published as a book, which means the extensive documentation is organized
in a particular fashion.  By keeping the "flow" of **tex.web**,
[TeX: The Program](https://www.amazon.com/Computers-Typesetting-B-TeX-Program/dp/0201134373/)
can still be used as a reference.

A project like this makes sense now because **tex.web** is very nearly frozen at version `$\pi$` (Knuth was born 1938).
Also, many languages now have sufficient features that preserving the presentation of **tex.web** is more possible
than it was in the past.  (Even then, compile-time reflection in C++26 would make simulating nested functions easier.)

Other goals might include:
* "Proving" that's it's possible to write a non-trivial program in a language's idomatic style; and,
* that such a program can be written warning-free, even with maximum warnings enabled.
  (including static code-analysis and the like).
* Making it easier to do various experiments with TeX, something that is difficult with **tex.web** or other ports that are
  primarily interested in a working TeX executable.

  It is not (necessarily) intended to be a production version of TeX; although since it passes the "TRIP" test, it could be.

  PRs happily accepted! This is most definately a work in progress.
