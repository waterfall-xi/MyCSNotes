# Learn C++ Tutorial - Learning Note

[Learn C++ – Skill up with our free tutorials](https://www.learncpp.com/)

LearnCpp.com is a free website devoted to teaching you how to program in modern C++. The lessons on this site will walk you through all the steps needed to write, compile, and debug your C++ programs. No prior programming experience is necessary, but programmers of all levels will benefit from our best practices, tips, and insights.

Becoming an expert won’t happen overnight, but with a bit of patience, you’ll get there. And LearnCpp.com will show you the way.

# Introduction / Getting Started

<div style="border: 2px solid #c7c7c7; background-color: #f4f4f4; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Nomenclature
    </p>
    <p style="margin: 1;">
        Although C++ is technically considered a high-level language, newer programming languages (e.g. scripting languages) provide an even higher level of abstraction. As such, C++ is sometimes inaccurately called a “low-level language” in comparison.
    </p>
</div>

<div style="border: 2px solid #c7c7c7; background-color: #f4f4f4; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Author’s note
    </p>
    <p style="margin: 1;">
        Today, C++ would probably be more accurately described as a mid-level language. However, this also highlights one of C++’s key strengths: it often provides the ability to work at different levels of abstraction. You can choose to operate at a lower level for better performance and precision, or at a higher level for greater convenience and simplicity.
    </p>
</div>

<div style="border: 2px solid #c1acff; background-color: #e7dfff; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Rule
    </p>
    <p style="margin: 1;">
        Rules are instructions that you <i>must</i> do, as required by the language. Failure to abide by a rule will generally result in your program not working.
    </p>
</div>

<div style="border: 2px solid #9cd49c; background-color: #dfffdf; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Best practice
    </p>
    <p style="margin: 1;">
        Best practices are things that you <i>should</i> do, because that way of doing things is either conventional (idiomatic) or recommended. That is, either everybody does it that way (and if you do otherwise, you’ll be doing something people don’t expect), or it is generally superior to the alternatives.
    </p>
</div>

<div style="border: 2px solid #d89696; background-color: #ffd6d6; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Warning
    </p>
    <p style="margin: 1;">
        Warnings are things that you <i>should not</i> do, because they will generally lead to unexpected results.
    </p>
</div>

<div style="border: 2px solid #dad591; background-color: #ffffdf; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Otehrs
    </p>
    <p style="margin: 1;">
        Otehrs
    </p>
</div>


## 0.2 — Introduction to programs and programming languages

<div style="border: 2px solid #c7c7c7; background-color: #f4f4f4; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Platform
    </p>
    <p style="margin: 1;">
        The term <b>platform</b> refers to a compatible set of hardware and software (OS, browser, etc…) that provides an environment for software to run. For example, the term “PC” is used colloquially to mean the platform consisting of a Windows OS running on an x86-family CPU.
    </p>
</div>

<div style="border: 2px solid #c7c7c7; background-color: #f4f4f4; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Portable
    </p>
    <p style="margin: 1;">
        If a program uses capabilities or services provided by the platform, it becomes dependent on that platform, and cannot be run on other platforms without modification. An program that can be easily transferred from one platform to another is said to be <b>portable</b>. The act of modifying a program so that it runs on a different platform is called <b>porting</b>.
    </p>
</div>

<div style="border: 2px solid #c7c7c7; background-color: #f4f4f4; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        CPU family
    </p>
    <p style="margin: 1;">
        A “CPU family” is formally called an “instruction set architecture” (“ISA” for short).
    </p>
</div>



assembly code -[assembler]-> machine code --pack--> executable file

C++ code  -[C++ compiler]-> machine code / assembly code --pack--> executable file

<div style="border: 2px solid #c7c7c7; background-color: #f4f4f4; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        cross-platform
    </p>
    <p style="margin: 1;">
        If we’re careful, we can write a single C++ that will compile on every platform that has a C++ compiler! A program that is designed to run on multiple platforms is said to be <b>cross-platform</b>.
    </p>
</div>

### factors  inhibit the portability

- Operating system: such as Microsoft Windows, offer platform-specific capabilities that easier to use but depend on OS.
- Third-party libraries: those are only available on certain platforms.
- Compilers-specific extensions from compilers: which are capabilities that are only available in that compiler.
- Compilers defined behavior: eg. theme “implementation-defined behavior”

## 0.3 — Introduction to C/C++

**Object-oriented Programming**

- Video games
- Real-time systems (e.g. for transportation, manufacturing, etc…)
- High-performance financial applications (e.g. high frequency trading)
- Graphical applications and simulations
- Productivity / office applications
- Embedded software
- Audio and video processing
- Artificial intelligence and neural networks

## 0.4 — Introduction to C++ development

<div style="border: 2px solid #9cd49c; background-color: #dfffdf; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Best practice
    </p>
    <p style="margin: 1;">
        Name the first/primary source code file in each program <code>main.cpp</code>. This makes it easy to determine which source code file is the primary one.
    </p>
</div>

## 0.5 — Introduction to the compiler, linker, and libraries

Coding -> Compile (`filename.0`) -> Link (`executablefilename.exe`)

Build / Make = Compile + Link

## 0.6 — Installing an Integrated Development Environment (IDE)

## 0.7 — Compiling your first program

### Creating a project in VS Code

1. Open Folder
2. New File `main.cpp`
3. Typing code
4. Run C/C++ File / Debug C/C++ File
5. Choose the *g++ build and debug active file* option (at the first time)

### Nomenclature differentiation: compile, build, run...

- **Build** compiles all *modified* code files in the project or workspace/solution, and then links the object files into an executable. If no code files have been modified since the last build, this option does nothing.
- **Clean** removes all cached objects and executables so the next time the project is built, all files will be recompiled and a new executable produced.
- **Rebuild** does a “clean”, followed by a “build”.
- **Compile** recompiles a single code file (regardless of whether it has been cached previously). This option does not invoke the linker or produce an executable.
- **Run/start** executes the executable from a prior build. Some IDEs (e.g. Visual Studio) will invoke a “build” before doing a “run” to ensure you are running the latest version of your code. Otherwise (e.g. Code::Blocks) will just execute the prior executable.

## 0.8 — A few common C++ problems

### General run-time issues

#### Q: When executing a program, the console window blinks and then closes immediately.

#### Q: I ran my program and get a window but no output.

### General compile-time issues

#### Q: When I compile my program, I get an error about unresolved external symbol _main or _WinMain@16

#### Q: When I compile my program, I get an error that main is already defined, or about multiple definitions for main

#### Q: I’m trying to use C++11/14/17/XX functionality and it doesn’t work

#### Q: When I compile my program, I get an error that it cannot open the .exe for writing

#### Q: When trying to use cin, cout, or endl, the compiler says cin, cout, or endl is an ‘undeclared identifier’

```
#include <iostream>
std::cout << "make sure each use of cin, cout, and endl are prefixed by std::" << std::endl;
```

### Visual Studio issues

#### Q: When compiling with Microsoft Visual C++, you get a C1010 fatal error, with an error message like "c:\vcprojects\test.cpp(263) :fatal error C1010: unexpected end of file while looking for precompiled header directive"

#### Q: Visual Studio gives an error like: "1MSVCRTD.lib(exe_winmain.obj) : error LNK2022: unresolved external symbol _WinMain@16 referenced in function "int __cdecl invoke_main(void)" (?invoke_main@@YAHXZ)"

#### Q: When I compile my program, I get a warning about "Cannot find or open the PDB file"

### Something else

#### Q: I have some other problem that I can’t figure out. How can I get an answer quickly?

## 0.9 — Configuring your compiler: Build configurations

**build configuration**

- Executable name
- Code and library files directories
- Compiler optimizing level
- etc.

**debug configuration**

- Turns off all optimizations
- Includes debugging information, which makes your programs larger and slower
- Easier to debug

**release configuration**

- Typically optimized for size and performance
- No extra debugging information
- Ready to release or test performance

<div style="border: 2px solid #dad591; background-color: #ffffdf; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        For gcc and Clang users
    </p>
    <p style="margin: 1;">
        For GCC and Clang, the <code>-0#</code> option is used to control optimization settings. The most common options are as follows:
    </p>
    <ul>
        <li><code>-O0</code> is the recommended optimization level for <b>debug builds</b>, as it disables optimization. This is the default setting.</li>
        <li><code>-O2</code> is the recommended optimization level for <b>release builds</b>, as it applies optimizations that should be beneficial for all programs.</li>
        <li><code>-O3</code> adds additional optimizations that may or may not perform better than <code>-O2</code> depending on the specific program. Once your program is written, you can try compiling your release build with <code>-O3</code> instead of <code>-O2</code> and measure to see which is faster.</li>
	</ul>
    <p style="margin: 1;">
        See <a href="https://gcc.gnu.org/onlinedocs/gcc/Optimize-Options.html">https://gcc.gnu.org/onlinedocs/gcc/Optimize-Options.html</a>  for information on optimization options.
    </p>
</div>

<div style="border: 2px solid #dad591; background-color: #ffffdf; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        For VS Code users
    </p>
    <p style="margin: 1;">
        When you first ran your program, a new file called <code>tasks.json</code> was created under the .vscode folder in the explorer pane. Open the tasks.json file, find <code>"args"</code>, and then locate the line <code>"${file}"</code> within that section.
    </p>
    <p style="margin: 1;">
        Above the <code>"${file}"</code> line, add a new line containing the following command (one per line) when debugging:<br />
<code>"-ggdb",</code>
    </p>
    <p style="margin: 1;">
    	Above the <code>"${file}"</code> line, add new lines containing the following commands (one per line) for release builds:<br />
<code>"-O2",</code><br />
<code>"-DNDEBUG",</code>
    </p>
</div>

**Debugging option**

- `-g`: extra debugging information in the operating system’s native format.
- `-ggdb`: extra debugging information for use by GDB.
- `-g0` `-ggdb0`: no debug information at all.

- `-g1 ` `-ggdb1`: minimal information, enough for making backtraces in parts of the program that you don’t plan to debug. This includes descriptions of functions and external variables, and line number tables, but no information about local variables.
- `-g2` `-ggdb2`: default level information.
- `-g3` `-ggdb3`: extra information, such as all the macro definitions present in the program.

The last `-g` is effective while multiple `-g` options are used.

**Use `-Og`instead of `-O0`**

`-Og` make compiler passes some information useful for debugging but `-O0` not.

See https://gcc.gnu.org/onlinedocs/gcc/Debugging-Options.html.

**`-DNDEBUG`**

Means *Define No Debug*, it will define macro `NDEBUG`, make `assert` ineffective (be ignored in compiling).

More about gcc is here: https://gcc.gnu.org/onlinedocs/gcc/index.html#SEC_Contents.

<div style="border: 2px solid #9cd49c; background-color: #dfffdf; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Best practice
    </p>
    <p style="margin: 1;">
        Whenever you update your project settings, make the change for all build configurations (unless it’s not appropriate for some reason).
    </p>
</div>


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

