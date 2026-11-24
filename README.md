<figure data-latex-placement="h">
<img src="logo.svg" style="width:50.0%" />
<figcaption>Cinnabar logo</figcaption>
</figure>

**Cinnabar Language**

*lefloysi*

------------------------------------------------------------------------

# Introduction

Hello! So happy to have you here. This is my first specification and
language and my first attempt at designing a language at this scale. I
would be extremely happy if you gave me any feedback on literally
anything. These are also my first LaTeX documents.

The goal is to create a language that will make native applications
great again.

# How AI is used in this project

It isn’t. I have used AI in the past, but most everything in this
document is hand written. It might be used on occasion when I’m learning
a new LaTeX syntax or feature.

AI is a great tool when you need to get something done. But this? This I
care about. I want to do it right.

To make an example of what I would use AI for. My company logo. Now
don’t be upset, I came up with the full idea of the logo. I used AI to
generate me an SVG of the logo idea. I gave it the gradient, the braces,
the rounded corners. Entirely my own idea, just transformed into SVG
with AI as I have no interest in learning SVG.

# About Cinnabar

Cinnabar is a statically typed language compiled, general purpose
programming language with a focus on applications and games. It supports
low level operation such as direct pointer manipulation and raw memory
allocation.

The goal with Cinnabar is to fix C++’s decades of baggage. There should
be a single way to initialize a variable. There should not be a most
vexing parse. I aim to improve the bad defaults by making functions
nodiscard by default, and requiring an implicit keyword, instead of
explicit.

There is also no implicit copying, implicit referencing unless you
define it. Cinnabar also gives you access to some language facilities
that are genuinely missing from C++. Such as `abandon $foo;`

This syntax allows for the suppression of the destructor, which allows
for some things C++ only gets through optimization to be direct language
features.

My compiler follows a front-end/middle-end/back-end architecture. By
default the back-end is LLVM, although this may be customizable in the
future.

# Planned but not designed bits of the language

I read about this in another language proposal, which is the [kov
language](https://github.com/wube/kov). In these documents Kovarex
proposes having a persistent compiler. I fell in love with this idea and
have been thinking about it a ton. But until now, I can’t figure out how
to write such a compiler.

# Contents of this repository

This repository contains the specification and source files for the
front-end and middle-end of Cinnabar.

You will find the specification as a bunch of LaTeX documents inside of
/docs/spec/. You can find this README.md inside of /docs/readme.
