# Learn C++ Tutorial - Learning Note

[Learn C++ – Skill up with our free tutorials](https://www.learncpp.com/)

LearnCpp.com is a free website devoted to teaching you how to program in modern C++. The lessons on this site will walk you through all the steps needed to write, compile, and debug your C++ programs. No prior programming experience is necessary, but programmers of all levels will benefit from our best practices, tips, and insights.

Becoming an expert won’t happen overnight, but with a bit of patience, you’ll get there. And LearnCpp.com will show you the way.

# Introduction / Getting Started

<div style="border: 2px solid #c7c7c7; background-color: #f4f4f4; border-radius: 8px; padding: 14px; margin: 5px">
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

<div style="border: 2px solid #9caad4; background-color: #dfe7ff; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Key insight
    </p>
    <p style="margin: 1;">
        Key insight
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

# 1 C++ Basics

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

**Every C++ program must have a special function named main (all lower case letters)!**

## 1.2 — Comments

### Single-line comments

```cpp
std::cout << "Hello world!\n"; // std::cout lives in the iostream library
std::cout << "It is very nice to meet you!\n"; // these comments make the code hard to read
std::cout << "Yeah!\n"; // especially when lines are different lengths
```

Comments for following code:

```cpp
// std::cout lives in the iostream library
std::cout << "Hello world!\n";
```

### Multi-line comments

```cpp
/* This is a multi-line comment.
   This line will be ignored.
   So will this one. */
/* This is a multi-line comment.
 * the matching asterisks to the left
 * can make this easier to read
 */
```

Attention: Multi-line style comments can not be nested.

```cpp
/* This is a multi-line /* comment */ this is not inside the comment */
// The above comment ends at the first */, not the second */
```

## 1.3 — Introduction to objects and variables

### Data and value

- Numbers (e.g. `5` or `-6.7`).
- Characters, which are placed between single-quotes (e.g. `'H'` or `'$'`). Only a single symbol may be used.
- Text, which must be placed between double-quotes (e.g. `"Hello"` or `"H"`). Text can contain 0 or more characters.

#### literals

Data values that are placed directly into the source code. see 5.2 — Literals

### Random Access Memory

The hardcoded data and data generating while the program is running are (usually, possible CPU register) stored in RAM.

### Objects and variables

An **object** represents a region of storage (typically RAM or a CPU register) that can hold a value.

Although objects in C++ can be unnamed (anonymous), more often we name our objects using an identifier. An object with a name is called a **variable**.

### Variable definition

### Data types

The decoding or interpretation mode for bit data in RAM.

<div style="border: 2px solid #9caad4; background-color: #dfe7ff; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Key insight
    </p>
    <p style="margin: 1;">
        The data type of an object must be known at compile-time (so the compiler knows how much memory that object requires).
    </p>
</div>

## 1.4 — Variable assignment and initialization

### Variable assignment

#### copy assignment

```cpp
int width; // define an integer variable named width
width = 5; // assignment of value 5 into variable width
```

### Variable initialization

```cpp
int a;         // default-initialization (no initializer)

// Traditional initialization forms:
int b = 5;     // copy-initialization (initial value after equals sign)
int c ( 6 );   // direct-initialization (initial value in parenthesis)

// Modern initialization forms (preferred):
int d { 7 };   // direct-list-initialization (initial value in braces)
int e = { 7 }; // copy-list-initialization of initial value 6 into variable height (rarely used)
int f {};      // value-initialization / zero-initialization to value 0 (empty braces)
```

#### Default-initialization

In many cases, default-initialization performs no initialization, and leaves the variable with an *indeterminate* value (a value that is not predictable, sometimes called a “garbage value”).
See 1.6 -- Uninitialized variables and undefined behavior

#### Copy-initialization

Copy-initialization is less efficient than other forms of initialization for some complex types. However, C++17 remedied the bulk of these issues.

<div style="border: 2px solid #c7c7c7; background-color: #f4f4f4; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        For advanced readers
    </p>
    <p style="margin: 1;">
    <p>Copy-initialization is also used whenever values are implicitly copied, such as when passing arguments to a function by value, returning from a function by value, or catching exceptions by value.</p>
    <p>每当隐式复制值时，也会使用复制初始化，例如按值将参数传递给函数、按值从函数返回或按值捕获异常时。</p>
    </p>
</div>

#### Direct-initialization

Direct-initialization was initially introduced to allow for more efficient initialization of complex objects (those with class types, which we’ll cover in a future chapter). Just like copy-initialization, direct-initialization had fallen out of favor in modern C++, largely due to being superseded by direct-list-initialization. However, direct-list-initialization has a few quirks of its own, and so direct-initialization is once again finding use in certain cases.
引入直接初始化最初是为了允许更高效地初始化复杂对象（具有 Class 类型的对象，我们将在下一章中介绍）。就像复制初始化一样，直接初始化在现代 C++ 中已经失宠，主要是由于被直接列表初始化所取代。但是，direct-list-initialization 也有一些自己的怪癖，因此直接初始化在某些情况下再次得到使用。

<div style="border: 2px solid #c7c7c7; background-color: #f4f4f4; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        For advanced readers
    </p>
    <p style="margin: 1;">
    <p>Direct-initialization is also used when values are explicitly cast to another type (e.g. via <code>static_cast</code>).</p>
    <p>每当隐式复制值时，也会使用复制初始化，例如按值将参数传递给函数、按值从函数返回或按值捕获异常时。</p>
    </p>
</div>

#### List-initialization

```cpp
int width { 5 };    // direct-list-initialization of initial value 5 into variable width (preferred)
int height = { 6 }; // copy-list-initialization of initial value 6 into variable height (rarely used)
```

<div style="border: 2px solid #9caad4; background-color: #dfe7ff; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Key insight
    </p>
    <p style="margin: 1;">
            <p>List-initialization purport: When we see curly braces, we know we’re list-initializing an object.</p>
    <p>列表初始化的意义：当我们看到大括号时，我们知道我们正在对对象进行列表初始化。
</p>
    </p>
</div>

Another benefit: **List-initialization disallows narrowing conversions**

```cpp
    // An integer can only hold non-fractional values.
    // Initializing an int with fractional value 4.5 requires the compiler to convert 4.5 to a value an int can hold.
    // Such a conversion is a narrowing conversion, since the fractional part of the value will be lost.
    int w1 { 4.5 }; // compile error: list-init does not allow narrowing conversion

    int w2 = 4.5;   // compiles: w2 copy-initialized to value 4
    int w3 (4.5);   // compiles: w3 direct-initialized to value 4
```

#### Value-initialization and zero-initialization

In most cases, value-initialization will implicitly initialize the variable to zero (or whatever value is closest to zero for a given type). In cases where zeroing occurs, this is called **zero-initialization**.

<div style="border: 2px solid #c7c7c7; background-color: #f4f4f4; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        For advanced readers
    </p>
    <p style="margin: 1;">
    <p>For class types, value-initialization (and default-initialization) may instead initialize the object to predefined default values, which may be non-zero.</p>
    <p>对于 Class 类型，value-initialization（和 default-initialization）可能会将对象初始化为预定义的默认值，该值可以是非零的。</p>
    </p>
</div>



<div style="border: 2px solid #9cd49c; background-color: #dfffdf; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Best practice
    </p>
    <p style="margin: 1;">
    <p>Prefer direct-list-initialization or value-initialization to initialize your variables.<br>
       首选 direct-list-initialization 或 value-initialization 来初始化变量。</p>
</div>

<div style="border: 2px solid #9cd49c; background-color: #dfffdf; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Best practice
    </p>
    <p style="margin: 1;">
    <p>Use direct-list-initialization when you’re actually using the initial value:<br>
       当你实际使用初始值时，请使用 direct-list-initialization：</p>
    <code>int x { 0 };    // direct-list-initialization with initial value 0<br>
          std::cout << x; // we're using that 0 value here</code>
    <p>Use value-initialization when the object’s value is temporary and will be replaced:<br>
       当对象的值是临时的并且将被替换时，请使用 value-initialization：</p>
    <code>int x {};      // value initialization<br>
	      std::cin >> x; // we're immediately replacing that value so an explicit 0 would be meaningless</code>
    </p>
</div>

<div style="border: 2px solid #9cd49c; background-color: #dfffdf; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Best practice
    </p>
    <p style="margin: 1;">
    <p>Initialize your variables upon creation. Unless for a specific reason<br>
       除非有特别的原因，在创建时就初始化变量。</p>
</div>

<div style="border: 2px solid #c7c7c7; background-color: #f4f4f4; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Related content
    </p>
    <p style="margin: 1;">
        For more discussion on this topic, Bjarne Stroustrup (creator of C++) and Herb Sutter (C++ expert) make this recommendation themselves here: https://github.com/isocpp/CppCoreGuidelines/blob/master/CppCoreGuidelines.md#es20-always-initialize-an-object.<br>
		有关此主题的更多讨论，Bjarne Stroustrup（C++ 的创建者）和 Herb Sutter（C++ 专家）自己提出了此建议：https://github.com/isocpp/CppCoreGuidelines/blob/master/CppCoreGuidelines.md#es20-always-initialize-an-object。
    </p>
</div>

 [here](https://github.com/isocpp/CppCoreGuidelines/blob/master/CppCoreGuidelines.md#es20-always-initialize-an-object).

### Unused initialized variables warnings and  `[[maybe_unused]]` attribute (C++17)

Modern compilers will typically generate warnings if a variable is initialized but not used.

```cpp
    // Here's some math/physics values that we copy-pasted from elsewhere
    double pi { 3.14159 };
    double gravity { 9.8 };
    double phi { 1.61803 };
    std::cout << pi << '\n';  // pi is used
    std::cout << phi << '\n'; // phi is used

    // The compiler will likely complain about gravity being defined but unused
```

For case that you does use the variable but want to reserve it and hope no warnings for it:

```cpp

    [[maybe_unused]] double pi { 3.14159 };  // Don't complain if pi is unused
    [[maybe_unused]] double gravity { 9.8 }; // Don't complain if gravity is unused
    [[maybe_unused]] double phi { 1.61803 }; // Don't complain if phi is unused
    std::cout << pi << '\n';
    std::cout << phi << '\n';

    // The compiler will no longer warn about gravity not being used
```

Additionally, the compiler will likely optimize these variables out of the program, so they have no performance impact.

## 1.5 — Introduction to iostream: cout, cin, and endl

### The input/output library

The **input/output library** (io library) is part of the C++ standard library that deals with basic input and output.

```cpp
#include <iostream>
```

<div style="border: 2px solid #9cd49c; background-color: #dfffdf; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Best practice
    </p>
    <p style="margin: 1;">
    Prefer <code>\n</code> over <code>std::endl</code> when outputting text to the console.<br>
	在将文本输出到控制台时尽量用 <code>\n</code> 而不是 <code>std::endl</code>。</p>
</div>


## 1.6 — Uninitialized variables and undefined behavior

When a variable is created/defined but not initialized, and it is given a memory address to use to store data, the default value of that variable is whatever (garbage) value happens to already be in that memory address! That is called an **uninitialized variable**.

当未初始化的变量被赋予用于存储数据的内存地址时，该变量的默认值是该内存地址中已经存在的任何（垃圾）值！这被称为未初始化的变量。

```cpp
#include <iostream>
int main()
{
    // define an integer variable named x
    int x; // this variable is uninitialized because we haven't given it a value
    std::cout << x << '\n'; // who knows what we'll get, because x is uninitialized
    return 0;
}
```

<div style="border: 2px solid #d89696; background-color: #ffd6d6; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Warning
    </p>
    <p style="margin: 1;">Some compilers, such as Visual Studio, will initialize the contents of memory to some preset value when you’re using a debug build configuration. This will not happen when using a release build configuration. Therefore, if you want to run the above program yourself, make sure you’re using a release build configuration (see lesson 0.9 -- Configuring your compiler: Build configurations for a reminder on how to do that).<br
>
    某些编译器（例如 Visual Studio）会在您使用 debug build configuration 时将 memory 内容初始化为某个预设值。使用 release build 配置时不会发生这种情况。因此，如果您想自己运行上述程序，请确保您使用的是 release build configuration（有关如何执行此作的提醒，请参阅 lesson0.9 -- Configuring your compiler: Build configurations）。</p>
    <p style="margin: 1;">For example, if you run the above program in a Visual Studio debug configuration, it will consistently print -858993460, because that’s the value (interpreted as an integer) that Visual Studio initializes memory with in debug configurations.<br>
	例如，如果在 Visual Studio 调试配置中运行上述程序，它将始终打印 -858993460，因为这是 Visual Studio 在调试配置中初始化内存时使用的值（解释为整数）。</p>
</div>

Using uninitialized variables is one of the most common mistakes that novice programmers make, and unfortunately, it can also be one of the most challenging to debug (because the program may run fine anyway if the uninitialized variable happened to get assigned to a spot of memory that had a reasonable value in it, like 0). This is the primary reason for the “always initialize your variables” best practice.
使用未初始化的变量是新手程序员最常犯的错误之一，不幸的是，它也可能是最具挑战性的调试错误之一（因为如果未初始化的变量碰巧被分配到具有合理值的内存点，例如 0），程序无论如何都可能运行良好。这是 “always initialize your variables” 最佳实践的主要原因。

## 1.7 — Keywords and naming identifiers

### Identifier naming rules

- Can not be a keyword.
    不能是关键字。
- Can only be composed of letters (lower or upper case), numbers, and the underscore character.
    标识符只能由字母（小写或大写）、数字和下划线字符组成。
- Can not start with a number.
    不能以数字开头。
- Case sensitive.
    区分大小写。

### Identifier naming best practices

A too long strong... Only a portion of the content is captured.

#### variable names

- Begin with a lowercase letter.
- See acronym to all lowercase word.

#### function names

- Begin with a lowercase letter.
- See acronym to all lowercase word.

#### structs, class, and enumerations names

- Begin with a capital letter.
- See acronym to all lowercase word.

<div style="border: 2px solid #9cd49c; background-color: #dfffdf; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Best practice
    </p>
    <p style="margin: 1;">
    When working in an existing program, use the conventions of that program (even if they don’t conform to modern best practices). Use modern best practices when you’re writing new programs.<br>
	在现有程序中工作时，请使用该程序的约定（即使它们不符合现代最佳实践）。在编写新程序时，请使用现代最佳实践。</p>
</div>

## 1.8 — Whitespace and basic formatting

### Style guides

A **style guide** is a concise, opinionated document containing (sometimes arbitrary) programming conventions, formatting guidelines, and best practices. The goal of a style guide is to ensure that all developers on a project are programming in a consistent manner.
Astyle guide 是一个简洁、有主见的文档，包含（有时是任意的）编程约定、格式指南和最佳实践。样式指南的目标是确保项目中的所有开发人员都以一致的方式进行编程。

Some commonly referenced C++ style guides include:
一些常用的 C++ 样式指南包括：

- [C++ Core Guidelines](http://isocpp.github.io/CppCoreGuidelines/CppCoreGuidelines), maintained by Bjarne Stroustrup and Herb Sutter. 由 Bjarne Stroustrup 和 Herb Sutter 维护。
- [Google](https://google.github.io/styleguide/cppguide.html).
- [LLVM](https://llvm.org/docs/CodingStandards.html)
- [GCC/GNU GCC/GNU](https://gcc.gnu.org/codingconventions.html)

We generally favor the C++ Core Guidelines, as they are up to date and widely applicable.
我们通常支持 C++ 核心指南，因为它们是最新的并且广泛适用。

## 1.9 — Introduction to literals and operators

### Literals

A **literal** (also known as a **literal constant**) is a fixed value that has been inserted directly into the source code.

一个字面值（也称为 aliteral constant）是一个直接插入源代码的固定值。

### Operators

An **operation** is a process involving zero or more input values (called **operands**) that produces a new value (called an *output value*). An **operator** is a symbol used to denoted that perform a specific operation.
运算是涉及零个或多个输入值（称为作数）的过程，它产生一个新值（称为输出值）。运算符是被用来表示要执行某个特定运算的符号。

- **Unary**
- **Binary**
- **Ternary**
- **Nullary**

### Return values and side effect

## 1.10 — Introduction to expressions

In general programming, an **expression** is a non-empty sequence of literals, variables, operators, and function calls that calculates a value. The process of executing an expression is called **evaluation**, and the resulting value produced is called the **result** of the expression (also sometimes called the **return value**).
在一般编程中，anexpression 是计算值的文本、变量、运算符和函数调用的非空序列。执行表达式的过程称为 evaluation，生成的结果值称为表达式的结果（有时也称为返回值）。

<div style="border: 2px solid #c7c7c7; background-color: #f4f4f4; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        For advanced readers
    </p>
    <p style="margin: 1;">
        In C++, the result of an expression is one of the following:<br>
		A value (most commonly) 值（最常见）<br>
		An object or a function. We discuss expressions that return objects in lesson 12.2 -- Value categories (lvalues and rvalues). 对象或函数。我们在 lesson12.2 -- Value categories (lvalues and rvalues) 中讨论返回对象的表达式。<br>
		Nothing. These are the result of non-value returning function calls (covered in lesson 2.3 -- Void functions (non-value returning functions)) that are called only for their side effects 无。 这些是非值返回函数调用的结果（在 lesson2.3 -- Void functions (non-value returning functions) 中介绍），这些调用仅用于其副作用
    </p>
</div>

## 1.11 — Developing your first program

# C++ Basics: Functions and Files

## 2.1 — Introduction to functions

A **function** is a reusable sequence of statements designed to do a particular job.

```cpp
returnType functionName() // This is the function header (tells the compiler about the existence of the function)
{
    // This is the function body (tells the compiler what the function does)
}
```

### Nested functions are not supported

## 2.2 — Function return values (value-returning functions)

```cpp
#include <iostream>
// int is the return type
// A return type of int means the function will return some integer value to the caller (the specific value is not specified here)
int returnFive()
{
    // the return statement provides the value that will be returned
    return 5; // return the value 5 back to the caller
}

int main()
{
    std::cout << returnFive() << '\n'; // prints 5
    std::cout << returnFive() + 2 << '\n'; // prints 7

    returnFive(); // okay: the value 5 is returned, but is ignored since main() doesn't do anything with it

    return 0;
}
```

<div style="border: 2px solid #c7c7c7; background-color: #f4f4f4; border-radius: 8px; padding: 14px; margin: 5px">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Nomenclature
    </p>
    <p style="margin: 1;">
        The return expression produces the value to be returned. The return value is a copy of that value.<br>
		return 表达式生成要返回的值。返回值是该值的副本。
    </p>
</div>

<div style="border: 2px solid #9caad4; background-color: #dfe7ff; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Key insight
    </p>
    <p style="margin: 1;">
        C does allow <code>main()</code> to be called explicitly, so some C++ compilers will allow this for compatibility reasons.<br>
        C 语言允许显式调用 <code>main()</code>，因此出于兼容性原因，一些 C++ 编译器将允许这样做。
    </p>
</div>

<div style="border: 2px solid #9cd49c; background-color: #dfffdf; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Best practice
    </p>
    <p style="margin: 1;">
    Make sure your functions with non-void return types return a value in all cases.<br>
	确保具有非 void 返回类型的函数在所有情况下都返回值。<br>
	Failure to return a value from a value-returning function will cause undefined behavior.<br>
    未能从值返回函数返回值将导致未定义的行为。</p>
</div>

## 2.3 — Void functions (non-value returning functions)

```cpp
void printHi() // This function is non-value returning
{
    std::cout << "In printHi()" << '\n';
    return; // OK, return in advance and do not execute subsequent statements
    std::cout << "Hi!" << '\n';
    return 5; // compile error: we're trying to return a value
}
```

**Void function can use return statement to return to the caller at the point where the return statement is executed**

**Void functions can’t be used in expression that require a value**

## 2.4 — Introduction to function parameters and arguments

```cpp
#include <iostream>

int getValueFromUser()
{
 	std::cout << "Enter an integer: ";
	int input{};
	std::cin >> input;
	return input;
}

void printDouble(int value)
{
	std::cout << value << " doubled is: " << value * 2 << '\n';
}

int main()
{
	printDouble(getValueFromUser());
	return 0;
}
```

### Unreferenced parameters and unnamed parameters

In certain cases, you will encounter functions that have parameters that are not used in the body of the function. These are called **unreferenced parameters**.
在某些情况下，您会遇到具有函数体中未使用的参数的函数。这些参数称为 unreferenced 参数。

In a function definition, the name of a function parameter is optional. Therefore, in cases where a function parameter needs to exist but is not used in the body of the function, you can simply omit the name. A parameter without a name is called an **unnamed parameter**.
在函数定义中，函数参数的名称是可选的。因此，如果函数参数需要存在但未在函数主体中使用，则只需省略该名称即可。没有名称的参数称为 anunnamed 参数。

<div style="border: 2px solid #c7c7c7; background-color: #f4f4f4; border-radius: 8px; padding: 14px; margin: 5px">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Author’s note
    </p>
    <p style="margin: 1;">
        Why we’d write a function that has a parameter whose value isn’t used? 为什么我们要编写一个具有 value 未使用的参数的函数？<br>
		Let’s say we have a function with a single parameter. Later, the function is updated in some way, and the value of the parameter is no longer needed. If the now-unused function parameter were simply removed, then every existing call to the function would break (because the function call would be supplying more arguments than the function could accept). This would require us to find every call to the function and remove the unneeded argument. This might be a lot of work (and require a lot of retesting). It also might not even be possible (in cases where we did not control all of the code calling the function). So instead, we might leave the parameter as it is, and just have it do nothing. 假设我们有一个带有单个参数的函数。稍后，该函数以某种方式更新，并且不再需要参数的值。如果简单地删除了现在未使用的函数参数，那么对该函数的每个现有调用都会中断（因为函数调用将提供比函数可以接受的更多的参数）。这将要求我们找到对函数的每个调用并删除不需要的参数。这可能是大量的工作（并且需要大量的重新测试）。它甚至可能是不可能的（在我们没有控制调用该函数的所有代码的情况下）。因此，相反，我们可能会保持参数不变，让它什么都不做。
    </p>
</div>

<div style="border: 2px solid #c7c7c7; background-color: #f4f4f4; border-radius: 8px; padding: 14px; margin: 5px">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        For advanced readers
    </p>
    <p style="margin: 1;">
        Other cases where this occurs: 发生这种情况的其他情况：<br>
		Operators ++ and -- have prefix and postfix variants (e.g. ++foo vs foo++). An unreferenced function parameter is used to differentiate whether an overload of such an operator is for the prefix or postfix case. We cover this in lesson 21.8 -- Overloading the increment and decrement operators.
运算符++和--具有前缀和后缀变体（例如++foovsfoo++）。未引用的函数参数用于区分此类运算符的重载是针对前缀还是后缀大小写。我们将在课程中21.8 -- Overloading the increment and decrement operators介绍这一点。<br>
When we need to determine something from the type (rather than the value) of a type template parameter.
当我们需要从类型模板参数的类型（而不是值）中确定某些内容时。
    </p>
</div>

<div style="border: 2px solid #9cd49c; background-color: #dfffdf; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Best practice
    </p>
    <p style="margin: 1;">
    When a function parameter exists but is not used in the body of the function, do not give it a name. You can optionally put a name inside a comment.<br>
	当函数参数存在但未在函数正文中使用时，请勿为其命名。您可以选择在注释中放置名称。</p>
</div>
## 2.5 — Introduction to local scope

### local variables

1. defined inside the body of a function
2. function parameters

### local variable lifetime

Determine if local variable exist in memory. 决定局部变量是否存在于内存空间。

for local variable inside the function body:

- Begin at the point of definition, end at the end of curly braces. 在定义处开始，大括号末尾结束。
- Destroyed in the opposite order of creation. 以和创建顺序相反的顺序销毁。

for function parameter:

- Begin at the enter point of function, and at the end of the function. 在进入函数处开始，函数末尾结束。
- Destroyed in the opposite order of creation. 以和创建顺序相反的顺序销毁。

<div style="border: 2px solid #c7c7c7; background-color: #f4f4f4; border-radius: 8px; padding: 14px; margin: 5px">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        For advanced readers
    </p>
    <p style="margin: 1;">
        In actuality, objects may be created earlier, or destroyed later for optimization purposes.<br>
		实际上，对象可以提前创建，也可以稍后销毁以进行优化。
    </p>
</div>

**lifetime is a runtime property.**
The variable creation and destruction happen when the program is running. 变量创建和销毁发生在运行时。

### local scope (block scope)

Determine if local variable identifier can be used. 决定局部变量标识符是否可以使用。

for local variable identifier inside the function body:

- Begin at the point of definition, end at the end of curly braces. 在定义处开始，大括号末尾结束。

for function parameter identifier:

- Begin at the point of definition, end at the end of curly braces. 在定义处开始，大括号末尾结束。

**Scope is a compile-time property.**
Trying to use an identifier when it is not in scope will result in a compile error. 尝试在作用域外使用标识符会导致编译错误。

<div style="border: 2px solid #9cd49c; background-color: #dfffdf; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Best practice
    </p>
    <p style="margin: 1;">
    Define your local variables as close to their first use as reasonable.<br>
	尽可能接近其首次使用的位置进行局部变量定义。</p>
</div>

## 2.6 — Why functions are useful, and how to use them effectively

- Groups of statements that appear more than once in a program should generally be made into a function. For example, if we’re reading input from the user multiple times in the same way, that’s a great candidate for a function. If we output something in the same way in multiple places, that’s also a great candidate for a function.
    在程序中多次出现的语句组通常应组成函数。例如，如果我们以相同的方式多次读取用户的输入，那么这就是函数的一个很好的候选者。如果我们在多个地方以相同的方式输出一些东西，那也是一个很好的函数候选者。
- Code that has a well-defined set of inputs and outputs is a good candidate for a function, (particularly if it is complicated). For example, if we have a list of items that we want to sort, the code to do the sorting would make a great function, even if it’s only done once. The input is the unsorted list, and the output is the sorted list. Another good prospective function would be code that simulates the roll of a 6-sided dice. Your current program might only use that in one place, but if you turn it into a function, it’s ready to be reused if you later extend your program or in a future program.
    具有一组明确定义的输入和输出的代码是函数的良好候选者（尤其是在函数很复杂的情况下）。例如，如果我们有一个要排序的项目列表，那么进行排序的代码将成为一个很棒的功能，即使它只执行一次。input 是未排序的列表，output 是排序列表。另一个很好的 Prospective 函数是模拟 6 面骰子掷骰子的代码。您当前的程序可能只在一个地方使用它，但是如果您将其转换为函数，则当您以后扩展程序或将来的程序时，它就可以重用。
- A function should generally perform one (and only one) task.
    一个函数通常应该执行一个（且只有一个）任务。
- When a function becomes too long, too complicated, or hard to understand, it can be split into multiple sub-functions. This is called **refactoring**. We talk more about refactoring in lesson [3.10 -- Finding issues before they become problems](https://www.learncpp.com/cpp-tutorial/finding-issues-before-they-become-problems/).
    当一个函数变得太长、太复杂或难以理解时，它可以被拆分为多个子函数。这称为重构。我们在 lesson[3.10 -- Finding issues before they become problems](https://www.learncpp.com/cpp-tutorial/finding-issues-before-they-become-problems/) 中更多地讨论 refactoring。

## 2.7 — Forward declarations and definitions

### Use a forward declaration

A **forward declaration** allows us to tell the compiler about the existence of an identifier *before* actually defining the identifier.
Aforward 声明允许我们在实际定义标识符之前告诉编译器标识符的存在。

```cpp
#include <iostream>

int add(int x, int y); // forward declaration of add() (function declaration). Compile error is produced without this.

int main()
{
    std::cout << "The sum of 3 and 4 is: " << add(3, 4) << '\n'; // this works because we forward declared add() above
    return 0;
}

int add(int x, int y) // even though the body of add() isn't defined until here
{
    return x + y;
}
```

<div style="border: 2px solid #9cd49c; background-color: #dfffdf; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Best practice
    </p>
    <p style="margin: 1;">
    Keep the parameter names in your function declarations.<br>
	将参数名称保留在函数声明中。</p>
</div>

### The one definition rule (ODR)

1. Within a *file*, each function, variable, type, or template in a given scope can only have one definition. Definitions occurring in different scopes (e.g. local variables defined inside different functions, or functions defined inside different namespaces) do not violate this rule.
    在一个文件中，给定范围内的每个函数、变量、类型或模板只能有一个定义。出现在不同作用域中的定义（例如，在不同函数内定义的局部变量，或在不同命名空间内定义的函数）不违反此规则。
2. Within a *program*, each function or variable in a given scope can only have one definition. This rule exists because programs can have more than one file (we’ll cover this in the next lesson). Functions and variables not visible to the linker are excluded from this rule (discussed further in lesson [7.6 -- Internal linkage](https://www.learncpp.com/cpp-tutorial/internal-linkage/)).
    在一个程序中，给定作用域中的每个函数或变量只能有一个定义。这条规则之所以存在，是因为程序可以有多个文件（我们将在下一课中介绍这一点）。对链接器不可见的函数和变量被排除在此规则之外（将在 lesson[7.6 -- Internal linkage](https://www.learncpp.com/cpp-tutorial/internal-linkage/) 中进一步讨论）。
3. Types, templates, inline functions, and inline variables are allowed to have duplicate definitions in different files, so long as each definition is identical. We haven’t covered what most of these things are yet, so don’t worry about this for now -- we’ll bring it back up when it’s relevant.
    类型、模板、内联函数和内联变量允许在不同的文件中具有重复的定义，只要每个定义都相同即可。我们还没有介绍其中的大部分内容，所以现在不用担心 - 我们会在相关时重新提出来。

Violating part 1 of the ODR will cause the compiler to issue a redefinition error. Violating ODR part 2 will cause the linker to issue a redefinition error. Violating ODR part 3 will cause undefined behavior.
违反 ODR 的第 1 部分将导致编译器发出重新定义错误。违反 ODR 第 2 部分将导致链接器发出重新定义错误。违反 ODR 第 3 部分将导致未定义的行为。
