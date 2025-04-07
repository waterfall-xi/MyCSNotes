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
    <p>Prefer <code>\n</code> over <code>std::endl</code> when outputting text to the console.<br>
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
