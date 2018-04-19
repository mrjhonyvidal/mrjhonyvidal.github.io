---
title: "Debugging Javascript as a Ninja"
categories:
  - Debugging
tags:
  - javascript
  - eslint
  - atom
---

## Prepare your Environment

Mistakes happen and by no chance you will write down code without make small tiny mistakes that were not a mistake initially. So why not have a automated way to catch them all and display before even save/compile your code? 

Well that is the first step on debugging your code, pre debug automatically using linters, a linters are tools with bunch of rules pre-defined using code standards, and is quite easy to set linters inside our favorite editor(sublime, atom, visual studio code, etc), but the linters can be runned in our command-line console, which is fantastic because we can set these bunch of rules that we want to be followed everytime the whole code is built and deployed to a QA environment, and is fantastic because we assure that not only our code is being "linted" to check mistakes, inconsistences but everyone that colaborate to the project. 

I also would like to mention that debugg smartly is part of a test-driven environment, because if you think write down tests, whether they are functional, acceptance, smokey, end-to-end whatever, the mindset is what counts, think the scenario, figure out what could be an expected error, make the famous Green-red-Green cycle, make it pass with minimal solution, then make it fails intentionally/expectedly, then refactor the code make it pass. Which reduce the time debugging the error in the long run. And a last think, debugging is not google the error, but think the error, rollback to a safe point where everything is working, try to expect the result, code in small pieces. 

Here I share some secret techniquees by [Marek Kirejczyk (VP of Engineering at DaftCode)](http://qr.ae/TU16Nn) where he says:
    -Debug using binary search on your code. You can also do binary search your repository history (see git bisect). This technique can be very helpful when looking for bugs in the code.
    
    -Undo the last change if you brake something. Because you make small steps and you keep app covered wit tests, you should be able quickly notice if you break something. Just undo the recent change and start step from scratch.

## Setting Atom and EsLint

Here is quick video by Harry Wolff, 
https://www.youtube.com/watch?v=qhuFviJn-es

[https://hackernoon.com/what-is-eslint-how-do-i-set-it-up-on-atom-70f270f57296](What is ESLint? How do I set it up on Atom?)

