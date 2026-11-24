# Cinnabar Language

<img align="left" src="https://github.com/kilnware-dev/kilnware/blob/main/assets/logo.svg?raw=true" alt="Cinnabar Language Logo" width="240" hspace="20" vspace="6">Hello! So happy to have you here. This is my first specification and language and my first attempt at designing a language at this scale. I would be extremely happy if you gave me any feedback on literally anything. The spec is also my first LaTeX document.
<br clear="both" />
## Overview
Cinnabar is a statically typed language compiled, general purpose programming language with a focus on applications and games. It supports low level operation such as direct pointer manipulation and raw memory allocation.

The goal with Cinnabar is to fix C++'s decades of baggage. There should be a single way to initialize a variable. There should not be a most vexing parse. I aim to improve the bad defaults by making functions nodiscard by default, and requiring an implicit keyword, instead of explicit.

There is also no implicit copying, implicit referencing unless you define it. Cinnabar also gives you access to some language facilities that are genuinely missing from C++. Such as `abandon $foo`

This syntax allows for the suppression of the destructor, which allows for some things C++ only gets through optimization to be direct language features.


My compiler follows a front-end/middle-end/back-end architecture. By default the back-end is LLVM, although this may be customizable in the future.


## Highlights
- explicit relocate operator $
- everything implicit is always opt-in, rather than opt-out
- everything is \[\[nodiscard\]\]
- suppress operators with `abandon $foo`
- "simple code oriented" rather than object or data oriented

## Contents

| Path         | Description                                    |
| ------------ | ---------------------------------------------- |
| /src         | the compiler front- and middle-end             |
| /docs/readme | the old readme (its so pretty :3)              |
| /docs/spec   | the entire LaTeX Specification, run `main.tex` |

## Planned but not designed bits of the language
I read about this in another language proposal, which is the [kov](https://github.com/wube/kov}{kov) language. In these documents Kovarex proposes having a persistent compiler. I fell in love with this idea and have been thinking about it a ton. But until now, I can't figure out how to write such a compiler.

## How AI is used in this project
It isn't. I have used AI in the past, but most everything in this document is hand written. It might be used on occasion when I'm learning a new LaTeX syntax or feature. (god i hate i cant make this readme in latex because evil github wont render it :<, if youd like to read it open the old readme)

This project is about the journey, not the destination

To make an example of what I would use AI for. My company logo. Now don't be upset, I came up with the full idea of the logo. I used AI to generate me an SVG of the logo idea. I gave it the gradient, the braces, the rounded corners. Entirely my own idea, just transformed into SVG with AI as I have no interest in learning SVG.
