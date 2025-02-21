# Learn C++ Tutorial - Learning Note

[Learn C++ – Skill up with our free tutorials](https://www.learncpp.com/)

LearnCpp.com is a free website devoted to teaching you how to program in modern C++. The lessons on this site will walk you through all the steps needed to write, compile, and debug your C++ programs. No prior programming experience is necessary, but programmers of all levels will benefit from our best practices, tips, and insights.

Becoming an expert won’t happen overnight, but with a bit of patience, you’ll get there. And LearnCpp.com will show you the way.

# Introduction / Getting Started

<div style="border: 2px solid #c7c7c7; background-color: #f4f4f4; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Nomenclature
    </p>
    <p style="margin: 0;">
        Although C++ is technically considered a high-level language, newer programming languages (e.g. scripting languages) provide an even higher level of abstraction. As such, C++ is sometimes inaccurately called a “low-level language” in comparison.
    </p>
</div>
<<<<<<< HEAD

<div style="border: 2px solid #c7c7c7; background-color: #f4f4f4; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Nomenclature
    </p>
    <p style="margin: 0;">
        Although C++ is technically considered a high-level language, newer programming languages (e.g. scripting languages) provide an even higher level of abstraction. As such, C++ is sometimes inaccurately called a “low-level language” in comparison.
    </p>
</div>

=======
<div style="border: 2px solid #c7c7c7; background-color: #f4f4f4; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Author’s note
    </p>
    <p style="margin: 0;">
        Today, C++ would probably be more accurately described as a mid-level language. However, this also highlights one of C++’s key strengths: it often provides the ability to work at different levels of abstraction. You can choose to operate at a lower level for better performance and precision, or at a higher level for greater convenience and simplicity.
    </p>
</div>


>>>>>>> d98288d... 20250221-1353 update README.md
<div style="border: 2px solid #c1acff; background-color: #e7dfff; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Rule
    </p>
    <p style="margin: 0;">
        Rules are instructions that you <i>must</i> do, as required by the language. Failure to abide by a rule will generally result in your program not working.
    </p>
</div>

<div style="border: 2px solid #9cd49c; background-color: #dfffdf; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Best practice
    </p>
    <p style="margin: 0;">
        Best practices are things that you <i>should</i> do, because that way of doing things is either conventional (idiomatic) or recommended. That is, either everybody does it that way (and if you do otherwise, you’ll be doing something people don’t expect), or it is generally superior to the alternatives.
    </p>
</div>

<div style="border: 2px solid #d89696; background-color: #ffd6d6; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Warning
    </p>
    <p style="margin: 0;">
        Warnings are things that you <i>should not</i> do, because they will generally lead to unexpected results.
    </p>
</div>

## 0.2 — Introduction to programs and programming languages

<div style="border: 2px solid #c7c7c7; background-color: #f4f4f4; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Platform
    </p>
    <p style="margin: 0;">
        The term <b>platform</b> refers to a compatible set of hardware and software (OS, browser, etc…) that provides an environment for software to run. For example, the term “PC” is used colloquially to mean the platform consisting of a Windows OS running on an x86-family CPU.
    </p>
</div>

<div style="border: 2px solid #c7c7c7; background-color: #f4f4f4; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Portable
    </p>
    <p style="margin: 0;">
        If a program uses capabilities or services provided by the platform, it becomes dependent on that platform, and cannot be run on other platforms without modification. An program that can be easily transferred from one platform to another is said to be <b>portable</b>. The act of modifying a program so that it runs on a different platform is called <b>porting</b>.
    </p>
</div>

<div style="border: 2px solid #c7c7c7; background-color: #f4f4f4; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        CPU family
    </p>
    <p style="margin: 0;">
        A “CPU family” is formally called an “instruction set architecture” (“ISA” for short).
    </p>
</div>



assembly code -[assembler]-> machine code --pack--> executable file

C++ code  -[C++ compiler]-> machine code / assembly code --pack--> executable file

<div style="border: 2px solid #c7c7c7; background-color: #f4f4f4; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        cross-platform
    </p>
    <p style="margin: 0;">
        If we’re careful, we can write a single C++ that will compile on every platform that has a C++ compiler! A program that is designed to run on multiple platforms is said to be <b>cross-platform</b>.
    </p>
</div>

### factors  inhibit the portability

- Operating system: such as Microsoft Windows, offer platform-specific capabilities that easier to use but depend on OS.
- Third-party libraries: those are only available on certain platforms.
- Compilers-specific extensions from compilers: which are capabilities that are only available in that compiler.
- Compilers defined behavior: eg. theme “implementation-defined behavior”

## 0.3 — Introduction to C/C++

## 0.4 — Introduction to C++ development

<div style="border: 2px solid #9cd49c; background-color: #dfffdf; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Best practice
    </p>
    <p style="margin: 0;">
        Name the first/primary source code file in each program <code>main.cpp</code>. This makes it easy to determine which source code file is the primary one.
    </p>
</div>

## 0.5 — Introduction to the compiler, linker, and libraries

Coding -> Compile (`filename.0`) -> Link (`executablefilename.exe`)

Build / Make = Compile + Link

## 0.6 — Installing an Integrated Development Environment (IDE)

## 0.7 — Compiling your first program

## 0.8 — A few common C++ problems

## 0.9 — Configuring your compiler: Build configurations

## 0.10 — Configuring your compiler: Compiler extensions



## 1.1 — Statements and the structure of a program

### C++ statements

Most (but not all) statements in C++ end in a semicolon. If you see a line that ends in a semicolon, it’s probably a statement.

- Declaration statements
- Jump statements
- Expression statements
- Compound statements
- Selection statements (conditionals)
- Iteration statements (loops)
- Try blocks

### C++ functions

A **function** is a collection of statements that get executed sequentially (in order, from top to bottom).

## 1.2 — Comments

*123*