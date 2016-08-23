---
layout: post
title: "Rust: Recursive Types are Tricky"
date: 2016-08-23 17:40:00 +0300
categories: rust data structures types
---

As probably any other newbish Rust programmer I'm running into different mind blowing issues while actually writing [little educational purposes programs](https://github.com/alopatindev/rust-experiments/).

The major challenges are probably:

- Borrow Checker (especially when dealing with Recursive Types, like Trees or Lists)
- Program Design (my background is mostly OOP and some FP)

By reading the standard guides like ["The Book"](https://doc.rust-lang.org/book/) and ["Rust By Example"](http://rustbyexample.com)
I only got the idea of writing very trivial programs.
When dealing with something more complicated I run into borrow checker hell and other non-obvious compilation issues.

I've been [reading the articles](https://tagpacker.com/user/alopatindev?t=rust), listening to [podcasts](http://www.newrustacean.com/show_notes/index.html) and watching some video lectures with a hope to understand what the heck are Box, Cell, RefCell, etc. and how to properly deal with all this stuff.

While trying to implement a trivial "push" method for a mutable Singly Linked List I was frustrated a lot.
Then I found [this depressive post](https://stackoverflow.com/questions/28608823/how-to-model-complex-recursive-data-structures-graphs/28622326#28622326) that literally says "you can't really do this safely in Rust".

Looking into [std implementation of LinkedList](https://github.com/rust-lang/rust/blob/99867ee88380062827b63ce547603eea5fd3136c/src/libcollections/linked_list.rs#L93) I surprisingly found out that it's implemented using **unsafe blocks**.

### Good News

Eventually I found **[this awesome book](http://cglab.ca/~abeinges/blah/too-many-lists/book)**!

This is *"a guided tour of having the compiler scream at us"*, an emotional step-by-step **linked lists implementation** tutorial.

I **highly recommend this book** to all Rust newcomers.
This is the only reasonable book for today that helps me figure out the black magic of safe recursive data structures design in Rust.
