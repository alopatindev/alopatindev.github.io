---
layout: post
title: "How to Take Notes Like a Programmer"
date: 2018-01-14 23:00:00 +0300
categories: learning productivity workbook synopsis summary abstract conspectus epitome
---

When I was a kid I used to make pretty awful notes:
dirty hand-written copybooks with poor structure.
Almost unusable.

Later, when I discovered [MOOC](https://en.wikipedia.org/wiki/Massive_open_online_course) video courses,
I kept using the same antipatterns I used in classrooms but in a clearer way,
with [VimWiki](https://vimwiki.github.io) and later with [**Jupyter**](https://jupyter.org).

The notes were still poorly structured.
Take a look at this—I'm **not even motivated** to open and figure out what's in it:

![minipic](/pictures/how-to-take-notes-like-a-programmer/weeks.png)

Eventually I found what works best for me and I want to share it with you.

The main idea is to **projéct <u>our</u> mind into notes** (rather than a lecturer's mind)
using computer **programming principles**:

![](/pictures/how-to-take-notes-like-a-programmer/reflect-ideas.svg)

### Prerequisites
I assume you are already [aware of basic suggestions](https://www.google.com/search?q=take+notes) like
expressing ideas with **your own words** (own vocabulary, simpler terminology)
or focusing on questions, answers, **conclusions** and evidence.

I also assume you're [familiar with **chunking** technique](https://www.coursera.org/learn/learning-how-to-learn/lecture/nUOhG/2-1-introduction-to-chunking)
from [Learning How To Learn](https://www.coursera.org/learn/learning-how-to-learn) course
or from [A Mind for Numbers](https://www.amazon.com/Mind-Numbers-Science-Flunked-Algebra/dp/039916524X/) book.

### Make It Easier to Read
We, software developers, are very serious about code quality.
We don't like when [**code smells**](https://en.wikipedia.org/wiki/Code_smell#Common_code_smells).

We communicate with code and **invest extra time** and energy **in writing** elegant code,
so it could be read effectively in the future by **other developers**.
Including **ourselves**: in the future **we** literally **become different people**.

I found this approach useful for personal notes as well:
you can **optimize notes for effective lookups and reads** by applying extra effort in writing.

#### Raw Draft
Right down a **title** and **sources** (books, articles, papers, videos, whatever you use)
in a particular chunk of information.
Start analysis of the first source, add some **key points** during the analysis.

<video autoplay="" loop="" width="100%" playsinline="" onclick="this.play()">
  <source src="/pictures/how-to-take-notes-like-a-programmer/raw-draft.mp4" type="video/mp4">
</video>

#### Refactoring
So far, so good.
**Outline** key words, **split** long sentences, use **more complex bullet hierarchy**, add **subtitles**.
Use Occam's razor: **reduce your notes several times** without losing the original meaning.

<video autoplay="" loop="" width="100%" playsinline="" onclick="this.play()">
  <source src="/pictures/how-to-take-notes-like-a-programmer/refactoring.mp4" type="video/mp4">
</video>

Keep studying other sources and update **corresponding notes**:
add new information
and **clarify** the old one.

As the note becomes bigger—**separate it into files** or even **a directory structure**:

<video autoplay="" loop="" width="100%" playsinline="" onclick="this.play()">
  <source src="/pictures/how-to-take-notes-like-a-programmer/navigation.mp4" type="video/mp4">
</video>

How do I choose the structure?
Make it the way **you** feel comfortable: imagine you're looking for something in your own notes.
**How** exactly would you make a lookup?
What would be the **shortest path** to the note you need?

#### Add Hints for Future Changes
Are you bored of learning stuff and want to start doing things?
It's good to be pragmatic.
Add **assumptions** you might want to investigate in the future with **TODO comment**.

Did you find a cool resource about the topic you've already held over?
Find the **corresponding note**, add a **source** and keep doing your current work.

![](/pictures/how-to-take-notes-like-a-programmer/todo-receiver.png)

TODO comments are [considered as antipattern](http://wiki.c2.com/?TodoCommentsConsideredHarmful) by some developers,
though I still find them useful for personal projects and notes.

You **don't have to continue** your research in the future note review,
TODO comment is just a sign there's something you don't know well
and you might would like to improve knowledge in a particular area, **if you encounter it** in practice.

### Review and Improve
Suppose that some time has passed and you decided to use your notes.
You're **solving a particular problem** and you want to find something specific quickly.
Ability to find information quickly is important:
it **decreases probability to lose focus** on a problem you're trying to solve.

Try to **search in files**:

![](/pictures/how-to-take-notes-like-a-programmer/git-grep.png)

Couldn't find anything?
Possible reasons:
- a **typo** in the search **input**—check the spelling of your input first
- wrong keyword—a **synonym** was used to describe the same idea
- there's a **typo in your note**

Now it's time to improve.
Find your note **manually** and fix the problem by
- fixing the **typo**
- adding a **keyword**

So next time you'll find the same note quickly.

In some weird cases you'll fail to find the note again.
For instance, recently I tried to find some stuff about **statistics**:

![](/pictures/how-to-take-notes-like-a-programmer/git-grep-quantil.png)

Not found. A spelling issue?

![](/pictures/how-to-take-notes-like-a-programmer/google-quantil.png)

Nope.
I Googled something but WTF did I find?

As I'm not a native English speaker, it took extra time to figure it out: that was an **input typo** after all.

Misspelling of rarely used words is normal, even if you are a native speaker.
Possible solution is to **add misspelled** words as **keywords** so next time you'll find the note quickly.

![](/pictures/how-to-take-notes-like-a-programmer/keyword-quantil.png)

Another approach could be a use of some tricky **fuzzy search** engine.

**UPDATE**: Actually the problem was my confusion about
the [terminology](https://en.wikipedia.org/wiki/Quantile#Specialized_quantiles).
So in *this* case the right solution is to add «quantile» keyword.

#### Update Structure According to Your Mind Image
Suppose you ain't able to find your note quickly, **even manually**. Possible reasons:
- the note is in the **wrong place**
- the right place is **not well defined**
    - where would you put notes about Big-O notation: into Calculus or Algorithms?

How to fix it?
- **move** a section or a file to a proper place
- **add a link** from one note to another

![](/pictures/how-to-take-notes-like-a-programmer/reference-code.png)

![](/pictures/how-to-take-notes-like-a-programmer/reference.png)

#### Refactor Again
Suppose you've found what you've been looking for
but your **brain struggles to understand** something you've written in the past—just **simplify** it once again.

Another typical issue is finding **several notes** that actually should be **a single one**.
Just **merge** such fragments together and put in a proper place.

#### Find a Balance
How to not overdo this?
If you catch yourself **wasting time on finding** notes
in a **wrong place**—that's a sign it still has a poor structure.
Just improve it every time you run into this issue.

If it feels hard for you or too time-consuming—use something similar to "the rule of three":
if you've been looking for this particular note **two times** in the wrong place—**leave it untouched**.
For the **third** time—**refactor**.

### What's the Point?
You may say I didn't convince you that investing extra time in writing quality notes is so important:
doing that way is **too boring**, or it's **not applicable** to an area of your work/study.
This might be true, might be not.

Remember the time you've been doing a creative work, being ["in the zone"](https://en.wikipedia.org/wiki/Flow_(psychology)).
Sometimes you need to grab some information and **continue** your work, without losing a focus.
You may grab this information via Google but sometimes it's very specific,
like your own conclusions about a particular topic or maybe project-specific stuff.

As you can't find it in the Web—you use your notes.
Now it's a defining moment: if you are able to find the note quickly—you **won't lose a focus** on your work.
If you can't—you will interrupt and waste your time on finding this thing anyway.
Technically it's the same issue as **being interrupted** by somebody.

[![](/pictures/how-to-take-notes-like-a-programmer/programmer-interrupted.png)](http://heeris.id.au/2013/this-is-why-you-shouldnt-interrupt-a-programmer/)

After that you need to restore your **creative state** of mind again and continue your work.
Just think how much **energy it takes** from you.

Still feels taking notes that way is too time-consuming?
But you have time for **practice**, right?
Think twice.
Interruptions usually **steal our practice time** a lot.

Anyway it's just a strategy: that's true it **could** be inapplicable for some areas of work, so use it wisely.

### Checklist
- [x] Write a **raw draft** with **sources** and poor structure
- [x] **Refactor** your note once in a while:
    - [x] **Outline** key words
    - [x] **Split** long sentences
    - [x] Improve **bullet hierarchy**
    - [x] Use **subtitles**
    - [x] Simplify text, **reduce** it
    - [x] Too **long** documents?—Make **separate files**
    - [x] Too **many** files?—Improve **directory structure**
- [x] Add TODO **hints**
- [x] **Enjoy your creative work** without losing a focus! **Grab notes** when you need them:
    - [x] **Can't find** a note quickly?
        - [x] Fix **typos**
        - [x] Add **keywords** (sometimes **misspelled** keywords)
        - [x] **Wrong place**?—**Move** a section/file to a proper place
        - [x] Place is **ambiguous**?—**Add links** from other places
    - [x] **Can't understand**?—**Refactor** again
    - [x] **Duplicates/fragments** of a single note in several places?—**Merge** them

It's not that hard, right?

**UPDATE:** This post is also available in [Russian](https://habrahabr.ru/post/346876/) on Habrahabr.
