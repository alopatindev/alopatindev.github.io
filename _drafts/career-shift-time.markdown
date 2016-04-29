---
layout: post
title: "Career Shift Time!"
date: 2016-04-29 13:32:00 +0300
categories: career
---

That might looks funny for some people but I'm thinking about my next major career change for a long time (about two years now).

My career history is pretty short:

- started as a QA guy in a small game development company
- quickly shifted to Software Engineering
- eventually got hired by [Electronic Arts](http://www.ea.com), still working there

### Organizational Culture

Culture varies between studios/offices of a particular company.
Often relates to a particular country.

I think that culture directly affects engineers: the tools, methodologies and principles they use.
And their behavior.

#### "Proprietary" Culture

Some of my friends suggest it's not important at all: commercial secrets don't limit anything related to engineers (like productivity for example).
Unless they've been working at a big company with relatively strict NDA, I guess.

Let me try to explain what I mean on the concrete examples.

Sometimes I saw weird things:

- some people are **afraid of fail** at anything: they are so afraid that take too much responsibility by not telling about risky code changes they gonna make, for example
  - and that's completely opposite to what Google guys [were talking about](https://www.youtube.com/watch?v=0SARbwvhupQ) some time ago
- some people are literally **afraid of becoming useless** if they share too much information **with their co-workers**

And that's just not possible at all in the case if the whole project is Open Source, for example.

Another example.
I've been told a weird fact about one famous (non-gamedev) company: two engineers of **the same project** are prohibited to know what **each of them** are working on.
That sounds totally insane to me.

But anyway **I respect** any kind of organizational culture.
The problem is the particular one doesn't let me grow in the way I need.

### Choosing things based on Technologies

Eventually I decided to rate different activities (I called them "industries" here, but it's not really accurate) by my personal

- tech interest (interest in technologies the industry relates to)
- interest in the industry
- experience
- simplicity (how quickly it's possible to learn)

by writing [a small program in Scala](https://gist.github.com/alopatindev/9fa774c7a375b1772083fc976f6ce168) to see what happens. The last time the output looked like this:

```
Industries
industry                   tech.interest  ind.interest   knowledge      xp             simplicity     average
-------------------------------------------------------------------------------------------------------------
GNU/Linux Distro Dev       75%            70%            67%            77%            93%            76%
Linux Kernel Dev           66%            60%            50%            51%            89%            63%
Backend                    62%            100%           32%            27%            63%            57%
Android Dev                43%            60%            41%            47%            74%            53%
Frontend                   46%            50%            32%            39%            96%            53%
Desktop Apps               35%            70%            44%            42%            63%            51%
Embedded                   32%            30%            33%            35%            100%           46%
Fullstack                  53%            50%            27%            27%            41%            40%
QA Engineer (Backend)      61%            10%            31%            26%            59%            37%
Enterprise                 45%             0%            31%            27%            78%            36%
Finance / Bank             52%            10%            30%            29%            48%            34%
GameDev (Desktop)          27%            10%            41%            45%            44%            33%
GameDev (Mobile)           26%            10%            46%            51%            30%            33%
Data Science               61%            10%            26%            20%            37%            31%

Top 20 Technologies
technology                 interest       knowledge      xp             pop            average
----------------------------------------------------------------------------------------------
GNU/Linux                  100%           100%           100%           14%            78%
Free Software              100%           100%           100%            8%            77%
bash                       100%           100%           100%            6%            77%
Multithreading             100%           80%            80%             9%            67%
C                          100%           80%            80%             8%            67%
Vim                        100%           50%            100%           13%            66%
Network Client             50%            100%           90%             5%            61%
ssh                        100%           50%            90%             4%            61%
Marmalade                   0%            100%           100%            1%            50%
Android                    50%            50%            80%             1%            45%
C++                         0%            70%            100%           10%            45%
git                        100%           20%            50%             8%            44%
Scala                      100%           50%            10%             6%            42%
nginx                      100%           50%            10%             4%            41%
Reactive Programming       100%           50%            10%             3%            41%
Functional Programming     100%           50%            10%             3%            41%
JNI                        20%            50%            80%             3%            38%
Imperative OOP             10%            50%            80%             1%            35%
Python                      0%            80%            50%             5%            34%
svn                         0%            80%            50%             3%            33%
```

I didn't expect to see something too surprising, because it's **hard to do constructively**.

But it makes some idea of what I might feel comfortable with.

BTW, instead of industries/activities it's possible to put any concrete job opportunity details to see its rating.
Also this tool can be extended to a powerful job opportunities searching website.
I'll leave it as an idea for some startup company. Go ahead if you want to implement it ;)

### Next step

I figured out what I should **avoid**:

- Enterprise Development (classical Java EE and Finance-related stuff)
- Game Development
- Data Science

Summarizing, for me a **perfect match** would be:

- Client Side Development (particularly for GNU/Linux and maybe Android)
- Modern Technology Stack with new languages (like [Rust](https://rust-lang.org) and [Scala](http://www.scala-lang.org) for instance), partially with Functional Programming
- Free/Libre and Open Source software **development** and **use**
- Office in New Zealand and help with Relocation

But that doesn't look realistic for various reasons.

Or it does?
There's actually [Mozilla](https://www.mozilla.org) with their new [Servo browser engine](https://servo.org) written in Rust by an awesome team distributed around the world (not sure they've got anyone in NZ though).

Wish they had such a full-time opportunity, I would apply right away.

#### Plan B

If I won't find anything related, I'll try something different:

- maybe make some non-profit stuff for awhile to improve my skills
  - [GSoC](https://developers.google.com/open-source/gsoc/)?
    - particulary [Gentoo related stuff](https://wiki.gentoo.org/wiki/Google_Summer_of_Code/2016)
  - write some useful tool in Rust?
    - no idea what even to try; surprisingly there are already so many projects in Rust
  - something Bitcoin-related?
- or some Back-End stuff (I was always curious about distributed computations using things like [Scala](http://www.scala-lang.org) + akka-stream)
  - unless it's about data analysis

Or maybe somebody has a better suggestion?
