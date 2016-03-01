---
bibtex: @article{knuth1992,
  title={Literate programming},
  author={Knuth, Donald E},
  journal={CSLI Lecture Notes, Stanford, CA: Center for the Study of Language and Information (CSLI), 1992},
  volume={1},
  year={1992}
}
---

> One of life's greatest pleasures can be the composition of a computer program that you know will be a pleasure for other people to read, and for yourself to read. p ix

> Programming is best regarded as the process of creating _works of literature_.

> All of the major problems associated with computer programming - issues of reliability, portability learnability, maintainability, and efficiency - are ameliorated when programs and their dialogues with users become more literate.

## Computer Programming as an Art

> Science is knowledge that we understand so well that we can teach it to a computer; and if we don't fully understand something, it is an art to deal with it. p4

> The real problem is that programmers have spent far too much time worrying about efficiency in the wrong places and at the wrong times. Premature optimisation is the root of all evil (or at least most of it) in programming. p10

> Pleasure is significantly enhanced when we accomplish something with limited tools.

> We have seen computer programming as an art, because it applies accumulated knowledge to the world, because it requires skill and ingenuity, and especially because it produces objects of beauty.  Programmers who subconsciously view themselves as artists will enjoy what they do and will do it better. p14

## Literate Programming

> I believe that the time is ripe for significantly better documentation of programs, and that we can best achieve this by considering programs to be _works of literature_. p99

> Instead of imagining that our main task is to instruct a _computer_ what to do, let us concentrate rather on explaining to _human beings_ what we want a computer to do. p99

> The practitioner of literate programming can be regarded as an essayist, whose main concern is with exposition and excellence of style. Such an author, with thesaurus in hand, chooses the names of variables carefully and explains what each variable means. He or she strives for a program that is comprehensible because its concepts have been introduced in an order that is best for human understanding, using a mixture of formal and informal methods that re ̈ınforce each other. p99

WEB is Knuth's literate programming language and is made of 2 parts - weave and tangle.

> A WEB user writes a program that serves as the source language for two different system routines.  One line of processing is called weaving the web; it produces a document that describes the program clearly and that facilitates program maintenance.  The other line of processing is called tangling the web; it produces a machine-executable program. The program and its documentation are both generated from the same source, so they are consistent with each other. p101

The format is essentially substituted macros:

> For example, the angle-bracket notation `< Program to print ::: numbers 2>`  is WEB ’s way of saying the following: “The PASCAL text to be inserted here is called ‘Program to print ::: numbers’, and you can find out all about it by looking at section 2.” p103.

> I have come to realize that there is no need to choose once and for all between top-down and bottom-up, because a program is best thought of as a web instead of a tree.  A hierarchical structure is present, but the most important thing about a program is its structural relationships. A complex piece of software consists of simple parts and simple relations between those parts; the programmer’s task is to state those parts and those relationships, in whatever order is best for human comprehension— not in some rigidly determined order like top-down or bottom-up.

A key advantage of this is that the amount of code in a routine can be commensurate with it's intent.  Large error checking modules can be extracted to better reveal intent.

    procedure update;
    begin if <input data is invalid> then
      <Issue an error message and try to recover>;
    <Update the data structure>;
    end.

> On the other hand when the same task is programmed with WEB, the purpose of update can be shown quite clearly, and the possibility of error recovery can be reduced to a mere mention when update is defined. When another section entitled ‘<Issue an error message and try to recover>’ is subsequently written, the whole point of that section is to do the best error recovery, and it becomes quite natural to write a better program as a result. p126

> Nothing about WEB is really new; I have simply combined a bunch of ideas that have been in the air for a long time. p130

## Mathematical Writing

Each module in literate programming is introduced at the right psychological moment because the compiler orders the code. p236

> There was at all points a natural order of exposition, and it seems that the natural orderings for reading and writing are very much the same. p236

Since compound words are inevitable when naming macros, and camel case is hard to read and looks bad in print, short underscores should be used to conjoin words. p236

> Each module should contain an informal but clear description of what it actually does. We are trying to covey an intuition of what is going on , so a high-level account is much more helpful. p237

> The whole philosophy of WEB is to break a complex thing into tractable part, so the code should reflect this. p237

Kunth favours anthropomorphism of code.

> Why prompt the user with `Name of file to process?` when we can have the computer say `What file should I process?` p237

> Perhaps humans can think of complex processes best in terms of demons in boxes, so why not acknowledge this. p237

Composition of routines allows intent to be communicated. p239
