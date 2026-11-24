## 1. Introduction

Hello! So happy to have you here. This is my first specification and language and my first attempt at designing a language at this scale. I would be extremely happy if you gave me any feedback on literally anything. These are also my first LaTeX documents.

  

> **The goal:?**
> Create a language that will make native applications great again.

## 2. How AI is Used in This Project

**It isn’t.** I have used AI in the past, but most everything in this document is hand written. It might be used on occasion when I’m learning a new LaTeX syntax or feature.


AI is a great tool when you need to get something done. But this? This I care about. I want to do it right.

  

## 3. About Cinnabar

Cinnabar is a **statically typed, compiled, general-purpose programming language** with a focus on **applications and games**. It supports low-level operations such as direct pointer manipulation and raw memory allocation.

  

### Fixing C++’s Decades of Baggage

|**Area**|**C++ Default**|**Cinnabar Design**|
|---|---|---|
|**Initialization**|Multiple competing syntaxes & the _most vexing parse_|**A single way** to initialize a variable — no most vexing parse|
|**Return Values**|Ignored silently unless marked `[[nodiscard]]`|**`nodiscard` by default**|
|**Conversions**|Implicit unless marked `explicit`|**Explicit by default** — requires an `implicit` keyword|
|**Copies & References**|Implicit copying and referencing|**No implicit copying or referencing** unless explicitly defined|
|**Destructor Control**|Relies on compiler optimizations (NRVO, etc.)|Direct language control via **`abandon $foo;`**|

### Direct Destructor Suppression (`abandon`)

Cinnabar gives you access to language facilities that are genuinely missing from C++, such as `abandon $foo;`.

  

This syntax allows for the suppression of the destructor, turning behaviors that C++ only achieves through compiler optimizations into direct, predictable language features.

  

### Compiler Architecture

My compiler follows a **front-end / middle-end / back-end** architecture (`Front-End` -> `Middle-End` -> `Back-End`). By default, the back-end is **LLVM**, although this may be customizable in the future.

  

## 4. Planned (Not Yet Designed) Features

> [!NOTE]
> 
> **Persistent Compiler** — I read about this in another language proposal, the [kov language](https://github.com/wube/kov). In these documents, Kovarex proposes having a persistent compiler. I fell in love with this idea and have been thinking about it a ton—though until now, I haven't yet figured out how to write such a compiler.
> 
>   

## 5. Contents of This Repository

This repository contains the specification and source files for the **front-end** and **middle-end** of Cinnabar.

|**Path**|**Description**|
|---|---|
|`/docs/spec/`|The full language specification written as a collection of LaTeX documents|
|`/docs/readme/`|Source files and assets (including `logo.svg`) for this `README.md`|