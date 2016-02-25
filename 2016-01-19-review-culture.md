---
layout: post
title: Review Culture - The Forgotten Contribution
date: 2016-01-19 20:19:21
author: Christopher Pisano - The Advisory Board Company
tags:
- Contributing
guest_post: true
excerpt: |
  Everyone wants to contribute but most do not know where to start and others
  are unable to write code. How can you start contrbuting without writing a
  single line of code and still have an impact on the code base?
---

###Overview

Review culture is often something that is overlooked and you do not realize how
important it is usually until it is too late. Most projects and companies fall
into the trap of encouraging users, developers, admins and anyone else capable to
contribute to their code base by either submitting feature/bug requests and code
for patches or something that does not exist yet. This is a great start and is
most definitely necessary to be successful. However when it comes to promoting
these patches and code contributions from development to productions is when you
find that nobody ever said anything about code reviews. Code reviews might be
the most important part of contributing to something and is definitely the most
overlooked. I know some people will say automated deployments with CI/CD tools
and writing tests etc will negate the need for code reviews, but the reality is
a fully automated pipeline with no human intervention from local development to
 production is a pipe dream for most. So what is your contigency plan?

###Reviewing Code - Who, What. . . Why?

From my experience in most organizations there is an incorrect perception of
code reviews. Everyone seems to agree that they are important, however very few
tend to agree on what exactly you are reviewing and who exactly needs to review.
My goal here is to try and simplify this a bit and even though there really is
no right answer, maybe my opinions can guide you in a direction.

####Who Reviews Code

It almost always seems that the perception is you need to know how to code in
order to review code. This perception in my opinion is incorrect and one of the
main reasons a strong review culture is hard to adopt. Code review is about more
than just knowing the code and that it executes correctly; it is how you learn. You can
gain a deeper understanding of how things work just by reviewing a pull request
without having any prior knowledge. The questions you will have will lead you
down a path of inquiry where you will hopefully continue to learn more.

I guess the short answer to who should review code is anyone and everyone who
wants to contribute. Those that know how to code can review based on
functionality from a technical standpoint while others can review based on
structure and other standards you have put in place. For those that want to make
the jump into doing more technical code reviews a "mentor program" can be put
in place. Pair an inexperienced reviewer with someone who knows the ropes. Let
them benefit from each others knowledge and perspectives. Before you know it
you will have more people capable of doing code reviews than you ever thought
you would need.

###What to Review

The easy answer here is to review everything, in detail and be nit picky over
everything. The better answer is to figure out what your automated tests will be
checking for and then fill in the gaps with human code reviews. Code
functionality is usually the top priority for automated testing so it should not
necessarily be the most important part of your human code review. What you
should focus on is more of the structure and syntax of what you are reviewing.
Ensuring there is a style guide that is being followed and that things like
commit messages and documentation meets a standard. You most definitely have the
right to reject a pull request, or at least push back, if it does not conform to
the style guide you put forth and especially if the commit message does not meet
your standards. Many people thing documentation is a no brainer but you would be
surprised how often there is little to no documentation. This is where I am most
stringent because I want people to be able to read a doc and understand what the
code is meant to do, what requirements it has and what dependencies it has in
order to function.

###Results

If you put the time in and foster a culture of code reviews and good practices
you will be pleasently surprised with what your code base ends up looking like.
You need to start at the beginning though. Define standards for commit messages,
documentation, structure etc. Make these well known and documented and then
start enforcing them. Enforce them in the lowest environments possible so it is
known what to expect when going to production. The cleaner your code base and
the more structured it is the easier it will be to find issues and recover.
