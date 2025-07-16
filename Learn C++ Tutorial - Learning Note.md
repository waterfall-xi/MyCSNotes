# Learn C++ Tutorial - Learning Note

[Learn C++ – Skill up with our free tutorials](https://www.learncpp.com/)

LearnCpp.com is a free website devoted to teaching you how to program in modern C++. The lessons on this site will walk you through all the steps needed to write, compile, and debug your C++ programs. No prior programming experience is necessary, but programmers of all levels will benefit from our best practices, tips, and insights.

Becoming an expert won’t happen overnight, but with a bit of patience, you’ll get there. And LearnCpp.com will show you the way.

**My comment account**

Waterfall
waterfall19991115@gmail.com

# 0 Introduction / Getting Started

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

# 2 C++ Basics: Functions and Files

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

## 2.8 — Programs with multiple code files

C++ is designed so that each source file can be compiled independently, with no knowledge of what is in other files. Therefore, the order in which files are actually compiled should not be relevant.
C++ 的设计使每个源文件都可以独立编译，而不知道其他文件中的内容。因此，文件的实际编译顺序应该无关紧要。

```cpp
// main.cpp
#include <iostream>

int add(int x, int y); // needed so main.cpp knows that add() is a function defined elsewhere

int main()
{
    std::cout << "The sum of 3 and 4 is: " << add(3, 4) << '\n';
    return 0;
}
```

```cpp
// add.cpp
int add(int x, int y)
{
    return x + y;
}
```

<div style="border: 2px solid #9caad4; background-color: #dfe7ff; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Tip
    </p>
    <p style="margin: 1;">
        Because the compiler compiles each code file individually (and then forgets what it has seen), each code file that uses <code>std::cout</code> or <code>std::cin</code> needs to <code>#include &lt;iostream&gt;</code>.<br>
        因为编译器单独编译每个代码文件（然后忘记了它所看到的内容），所以每个使用 std：：coutorstd：：cin 的代码文件都需要 #include 。
    </p>
</div>

<div style="border: 2px solid #9caad4; background-color: #dfe7ff; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Key insight
    </p>
    <p style="margin: 1;">
        How linker or compiler connect identifier to its definition?
    </p>
    <p style="margin: 1;">
        If the compiler has seen neither a forward declaration nor a definition for the identifier in the file being compiled, it will error at the point where the identifier is used.<br>
        如果编译器在正在编译的文件中既没有看到 forward 声明，也没有看到 identifier 的定义，它将在使用该 identifier 时出错。
    </p>
    <p style="margin: 1;">
        Otherwise, if a definition exists in the same file, the compiler will connect the use of the identifier to its definition.<br>
        否则，如果定义存在于同一文件中，编译器会将标识符的使用与其定义相关联。
    </p>
    <p style="margin: 1;">
        Otherwise, if a definition exists in a different file (and is visible to the linker), the linker will connect the use of the identifier to its definition.<br>
        否则，如果定义存在于其他文件中（并且对链接器可见），则链接器会将标识符的使用连接到其定义。
    </p>
    <p style="margin: 1;">
        Otherwise (the compiler has seen a forward but no definition exists in any other file), the linker will issue an error indicating that it couldn’t find a definition for the identifier.<br>
        否则（编译器看到 forward 声明但是在其他任何文件都没有定义存在），链接器将发出一个错误，指示它找不到标识符的定义。
    </p>
</div>

## 2.9 — Naming collisions and an introduction to namespaces

C++ requires that all identifiers be non-ambiguous.
C++ 要求所有标识符都是无歧义的。

Two (or more) identically named functions (or global variables) are introduced into separate files belonging to the same program. This will result in a linker error, as shown above.

1. Two (or more) identically named functions (or global variables) are introduced into separate files belonging to the same program. This will result in a linker error.
    两个（或多个）同名函数（或全局变量）被引入**属于同一程序的单独文件**中。这将导致**链接器错误**。
2. Two (or more) identically named functions (or global variables) are introduced into the same file. This will result in a compiler error.
    两个（或多个）同名函数（或全局变量）被引入到**同一个文件**中。这将导致编译器错误。

A **namespace** provides another type of scope region for disambiguation of naming. The names declared in a namespace are isolated from names declared in other scopes, allowing such names to exist without conflict.
namespace提供了另一种类型的范围区域以消除命名歧义。在命名空间中声明的名称与其他范围内声明的名称隔离，从而允许此类名称存在而不会发生冲突。

### std namespace

C++ moved all of the functionality in the standard library into a namespace named `std` (short for “standard”).
C++将标准库中的所有功能移动到名为 `std`（“standard”的缩写）的命名空间中。

```CPP
#include <iostream>

int main()
{
    std::cout << "Hello world!"; // when we say cout, we mean the cout defined in the std namespace
    return 0;
}
```

<div style="border: 2px solid #9cd49c; background-color: #dfffdf; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Best practice
    </p>
    <p style="margin: 1;">
    Use explicit namespace prefixes to access identifiers defined in a namespace.<br>
	使用显式命名空间前缀来访问命名空间中定义的标识符。
	</p>
</div>

### Using namespace std (and why to avoid it)

```CPP
#include <iostream>

using namespace std; // this is a using-directive that allows us to access names in the std namespace with no namespace prefix

int main()
{
    cout << "Hello world!";
    return 0;
}
```

If another cout is defined in the global namespace, the naming conflict will happened.
如果在全局命名空间又定义另一个 cout，则发生命名冲突。

<div style="border: 2px solid #d89696; background-color: #ffd6d6; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Warning
    </p>
    <p style="margin: 1;">
        Avoid using-directives (such as <code>using namespace std;</code>) at the top of your program or in header files. They violate the reason why namespaces were added in the first place.<br>
        避免在程序顶部或头文件中使用 using 指令（例如using namespace std;）。它们违反了最初添加命名空间的原因。
    </p>
</div>

## 2.10 — Introduction to the preprocessor

### Preprocessor directives 预处理器指令

**Preprocessor directives** (often just called *directives*) are instructions that start with a `#` symbol and end with a newline (NOT a semicolon). 预处理器指令（通常简称为指令）是以 a#symbol 开头并以换行符（不是分号）结尾的指令。

#### #include

When *#include* a file, the preprocessor replaces the #include directive with the contents of the included file.

#### Macro defines

In C++, a **macro** is a rule that defines how input text is converted into replacement output text.

```cpp
#define IDENTIFIER substitution_text
// MACRO_NAME ==> substitution_text
```

<div style="border: 2px solid #9cd49c; background-color: #dfffdf; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Best practice
    </p>
    <p style="margin: 1;">
    Macro names should be written in all uppercase letters, with words separated by underscores.<br>
	宏名称应全部使用大写字母书写，单词之间用下划线分隔。
	</p>
</div>

**Object-like macros with substitution text**

```cpp
#include <iostream>

#define MY_NAME "Alex"

int main()
{
    std::cout << "My name is: " << MY_NAME << '\n';
    // preprocessor converts into the following:
    std::cout << "My name is: " << "Alex" << '\n';
    return 0;
}
```

<div style="border: 2px solid #9cd49c; background-color: #dfffdf; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Best practice
    </p>
    <p style="margin: 1;">
    In C++ there are better alternatives than object-like macros with substitution text(see 7.10 -- Sharing global constants across multiple files (using inline variables)). <br>
	C++中有比带替代文本的 object-like 宏更好的替代方案（见 7.10）。
	</p>
</div>

**Object-like macros without substitution text for conditional compilation**

```cpp
#include <iostream>

#define PRINT_JOE

int main()
{
#ifdef PRINT_JOE
    std::cout << "Joe\n"; // will be compiled since PRINT_JOE is defined
#endif

#ifdef PRINT_BOB
    std::cout << "Bob\n"; // will be excluded since PRINT_BOB is not defined
#endif

    return 0;
}
```

```cpp
#include <iostream>

int main()
{
    std::cout << "Joe\n";

#if 0 // Don't compile anything starting here, change to 1 to enable
    std::cout << "Bob\n";
    std::cout << "Steve\n";
#endif // until this point

    return 0;
}
```

## 2.11 — Header files

Conventionally, header files (.h) are used to propagate a bunch of related forward declarations into a code file.
通常，头文件（.h）用于将一组相关的 forward 声明传播到 cpp 文件中。

```
#include <iostream>
```

`#include` a header file make it easy to copy all declarations for using library iostream.

<div style="border: 2px solid #9cd49c; background-color: #dfffdf; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Best practice
    </p>
    <p style="margin: 1;">
    If a header file is paired with a code file (e.g. add.h with add.cpp), they should both have the same base name (add).<br>
	如果头文件与代码文件配对（例如，add.h 与 add.cpp），则它们都应该具有相同的基本名称 （add）。
	</p>
</div>

**Including definitions in a header file will result in a violation of the one-definition rule**

**在头文件中包括定义将导致违反单定义规则**

**Source files should include their paired header** 
**源文件应包含其配对的头文件**

**Do not #include .cpp files**

**不要 #include .cpp 文件**

### Angled brackets vs double quotes

#### Angled brackets

Search only in the directories specified by the `include directories` (come with your compiler, OS, or third-party libraries you’ve installed elsewhere on your system). The preprocessor will not search for the header file in your project’s source code directory.
只在特定的 include 目录（编译器、作系统或已安装在系统其他位置的第三方库附带的）搜索，预处理器不会在项目的源代码目录中搜索头文件。

#### Double quotes

First search in the current directory. If it can’t find, then search the `include directories`.
先在当前目录搜索，如果没有再搜索 include 目录。

| Header type           | Naming convention | Example    | Identifiers placed in namespace                         |
| --------------------- | ----------------- | ---------- | ------------------------------------------------------- |
| C++ specific (new)    | <xxx>             | iostream   | std namespace                                           |
| C compatibility (new) | <cxxx>            | cstddef    | std namespace (required) & global namespace (optional)  |
| C++ specific (old)    | <xxx.h>           | iostream.h | global namespace                                        |
| C compatibility (old) | <xxx.h>           | stddef.h   | global namespace (required) & std  namespace (optional) |

### Including header files from other directories

Bad way (may won’t work after update directory structure):

```
#include "headers/myHeader.h"
#include "../moreHeaders/myOtherHeader.h"
```

A better method is to tell your compiler or IDE that you have a bunch of header files in some other location, so that it will look there when it can’t find them in the current directory. This can generally be done by setting an *include path* or *search directory* in your IDE project settings.
更好的方法是告诉你的编译器或 IDE 在其他位置有一堆头文件，这样当它在当前目录中找不到它们时，它会在那里查找。这通常可以通过在 IDE 项目设置中设置 include pathorsearch directory来完成。

### The order of inclusion for header files

<div style="border: 2px solid #9cd49c; background-color: #dfffdf; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Best practice
    </p>
    <p style="margin: 1;">
    To maximize the chance that missing includes will be flagged by compiler, order your #includes as follows (skipping any that are not relevant):
<br>
	为了最大限度地提高编译器标记缺少的 include 的几率，请按如下方式对 #includes 进行排序（跳过任何不相关的内容）：
	</p>
    <p style="margin: 1;">
        ● The paired header file for this code file (e.g. add.cpp should <code>#include "add.h"</code>)<br>
        ● Other headers from the same project (e.g. <code>#include "mymath.h"</code>)<br>
        ● 3rd party library headers (e.g. <code>#include &lt;boost/tuple/tuple.hpp&gt;</code>)<br>
        ● Standard library headers (e.g. <code>#include &lt;iostream&gt;</code>)
	</p>
</div>


## 2.12 — Header guards

### The duplicate definition problem

```cpp
#ifndef SQUARE_H
#define SQUARE_H

int getSquareSides(); // forward declaration for getSquareSides
int getSquarePerimeter(int sideLength); // forward declaration for getSquarePerimeter

#endif
```

## 2.13 — How to design your first programs

# 3 Debugging C++ Programs



# 4 Fundamental Data Types

## 4.1 — Introduction to fundamental data types

> To be completed

## 4.12 — Introduction to type conversion and static_cast

### Implicit type conversion

```cpp
#include <iostream>

void print(double x) // print takes a double parameter
{
	std::cout << x << '\n';
}

int main()
{
	print(5); // what happens when we pass an int value?
	return 0;
}
```

Implicit type conversion: int => double

```cpp
#include <iostream>

void print(int x) // print now takes an int parameter
{
	std::cout << x << '\n';
}

int main()
{
	print(5.5); // warning: we're passing in a double value
	return 0;
}
```

Implicit type conversion: double => int (possible warning)

**Type conversion of a value produces a new value**

### explicit type conversion via the static_cast operator

**Explicit type conversion** allow us (the programmer) to explicitly tell the compiler to convert a value from one type to another type, and that we take full responsibility for the result of that conversion. If such a conversion results in the loss of value, the compiler will not warn us.
显式类型转换允许我们（程序员）显式告诉编译器将值从一种类型转换为另一种类型，并且我们对该转换的结果负全部责任。如果此类转换导致值丢失，编译器不会警告我们。

```cpp
static_cast<new_type>(expression)
```

#### Sign conversions using static_cast

If the value being converted is in the value scope of destination type.
如果要转换的值在目标类型的取值范围内。

```cpp
    unsigned int u1 { 5 };
    // Convert value of u1 to a signed int
    int s1 { static_cast<int>(u1) };
    std::cout << s1 << '\n'; // prints 5

    int s2 { 5 };
    // Convert value of s2 to an unsigned int
    unsigned int u2 { static_cast<unsigned int>(s2) };
    std::cout << u2 << '\n'; // prints 5
```

Otherwise, something specially happen.

```cpp
    int s { -1 };
    std::cout << static_cast<unsigned int>(s) << '\n'; // prints 4294967295

    unsigned int u { 4294967295 }; // largest 32-bit unsigned int
    std::cout << static_cast<int>(u) << '\n'; // implementation-defined prior to C++20, -1 as of C++20
```

**std::int8_t and std::uint8_t likely behave like chars instead of integers**
std：：int8_t 和 std：：uint8_t 的行为可能类似于 chars 而不是整数

# 5 Constants and Strings

## 5.1 — Constant variables (named constants)

### Named constants

- Constant variables 常量变量
- Object-like macros with substitution text (introducced in 2.10) 带有替换文本的类对象宏 (2.10 中介绍)
- Enumerated constants (see 13.2) 枚举常量

#### Constant variables

Although it is a well-known oxymoron, a variable whose value cannot be changed after initialization is called a **constant variable**.
虽然它是一个众所周知的矛盾修辞法，但初始化后无法更改其值的变量称为 constant 变量。

```cpp
const double gravity { 9.8 };  // preferred use of const before type
int const sidesInSquare { 4 }; // "east const" style, okay but not preferred
```

<div style="border: 2px solid #9cd49c; background-color: #dfffdf; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Best practice
    </p>
    <p style="margin: 1;">
    Place <code>const</code> before the type (because it is more conventional to do so).<br>
	把 <code>const</code> 放在类型前面，因为这样是更规范的做法。
	</p>
</div>

<div style="border: 2px solid #9caad4; background-color: #dfe7ff; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Key insight
    </p>
    <p style="margin: 1;">
    The type of an object includes the const qualifier, so when we define const double gravity { 9.8 }; the type of gravity is const double.<br>
    对象的类型包括 const 限定符，因此当我们定义 const double gravity { 9.8 }; gravity 是 const double 的类型。
    </p>
</div>

**Const variables must be initialized**
**必须初始化 Const 变量**

Const variables naming conventions:

- C: underscored, upper-case, e.g. EARTH_GRAVITY
- some C++: intercapped with a ‘k’ prefix, e.g. kEarthGravity
- normal C++: just follow normal variables

**Const function parameters (do not)**

```cpp
void printInt(const int x)
{
    std::cout << x << '\n';
}
```

In modern C++ we don’t make value parameters `const` because value parameters is just a copy that will be destroyed at the end of the function anyway. The `const` keyword also adds a small amount of unnecessary clutter to the function prototype.

**Const return values (do not)**

```cpp
const int getValue()
{
    return 5;
}
```

For fundamental types, simply ignored (your compiler may generate a warning). 对于基本类型，将被简单地忽略（编译器可能会生成警告）。
For other types, there is typically little point in returning const objects by value, because they are temporary copies that will be destroyed anyway. 对于其他类型，按值返回 const 对象通常没有什么意义，因为它们是临时副本，无论如何都会被销毁。

<div style="border: 2px solid #9cd49c; background-color: #dfffdf; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Best practice
    </p>
    <p style="margin: 1;">
    Make variables constant whenever possible. Exception cases include by-value function parameters and by-value return types, which should generally not be made constant.<br>
	尽可能使变量成为常量。例外情况包括按值函数参数和按值返回类型，它们通常不应成为常量。
	</p>
</div>

<div style="border: 2px solid #9cd49c; background-color: #dfffdf; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Best practice
    </p>
    <p style="margin: 1;">
    Prefer constant variables over object-like macros with substitution text.<br>
	首选常量变量，而不是带有替换文本的类对象宏。
	</p>
</div>

const is a **type qualifiers**

## 5.2 — Literals

```cpp
return 5;                     // 5 is an integer literal
bool myNameIsAlex { true };   // true is a boolean literal
double d { 3.4 };             // 3.4 is a double literal
std::cout << "Hello, world!"; // "Hello, world!" is a C-style string literal
```

type of literal

| Literal value        | Examples             | Default literal type | Note                                                         |
| -------------------- | -------------------- | -------------------- | ------------------------------------------------------------ |
| integer value        | 5, 0, -3             | int                  |                                                              |
| boolean value        | true, false          | bool                 |                                                              |
| floating point value | 1.2, 0.0, 3.4        | double (not float!)  |                                                              |
| character            | ‘a’, ‘\n’ 'a'， '\n' | char                 |                                                              |
| C-style string       | “Hello, world!”      | const char[14]       | see C-style string literals section below<br/>请参阅下面的 C 样式字符串文本部分 |

adding a **literal suffix** to change the type of a literal

| Data type      | Suffix                                 | Meaning                                   |
| -------------- | -------------------------------------- | ----------------------------------------- |
| integral       | u or U                                 | unsigned int                              |
| integral       | l or L                                 | long                                      |
| integral       | ul, uL, Ul, UL, lu, lU, Lu, LU         | unsigned long                             |
| integral       | ll or LL                               | long long                                 |
| integral       | ull, uLL, Ull, ULL, llu, llU, LLu, LLU | unsigned long long                        |
| integral       | z or Z                                 | The signed version of std::size_t (C++23) |
| integral       | uz, uZ, Uz, UZ, zu, zU, Zu, ZU         | std::size_t (C++23)                       |
| floating point | f or F                                 | float                                     |
| floating point | l or L                                 | long double                               |
| string         | s                                      | std::string                               |
| string         | sv                                     | std::string_view                          |

**Scientific notation for floating point literals**

```cpp
double avogadro { 6.02e23 }; // 6.02 x 10^23 is a double literal in scientific notation
double protonCharge { 1.6e-19 }; // charge on a proton is 1.6 x 10^-19
```

### String literals

**For historical reasons, strings are not a fundamental type in C++.**

**C strings** or **C-style strings**

1. implicit null terminator: `"hello"`=`'h'`, `'e'`, `'l`‘, `'l'`, `'o'`, and `'\0'`
2. C-style string literals are const objects that are created at the start of the program and are guaranteed to **exist for the entirety of the program**.

## 5.3 — Numeral systems (decimal, binary, hexadecimal, and octal)

## 5.4 – as-if 规则和编译时优化

## 5.5 — Constant expressions

```cpp
const double x { 1.2 };
const double y { 3.4 };
const double z { x + y }; // x + y may evaluate at runtime or compile-time
```

The expression `x + y` would normally evaluate at runtime, but since the value of `x` and `y` are known at compile-time, the compiler may opt to perform compile-time evaluation instead and initialize `z` with the compile-time calculated value `4.6`.
表达式 x + y 通常会在运行时计算，但由于 x 和 y 的值在编译时是已知的，因此编译器可以选择执行编译时计算，并使用编译时计算值 4.6 初始化 z。

```cpp
constexpr int x { expr }; // Because variable x is constexpr, expr must be evaluatable at compile-time
```

The following most foundational C++ features using compile-time programming both make use of constant expressions:

- Constexpr variables (discussed in upcoming lesson [5.6 -- Constexpr variables](https://www.learncpp.com/cpp-tutorial/constexpr-variables/)).
- Constexpr functions (discussed in upcoming lesson [F.1 -- Constexpr functions](https://www.learncpp.com/cpp-tutorial/constexpr-functions/)).
- Templates (introduced in lesson [11.6 -- Function templates](https://www.learncpp.com/cpp-tutorial/function-templates/)).
- static_assert (discussed in lesson [9.6 -- Assert and static_assert](https://www.learncpp.com/cpp-tutorial/assert-and-static_assert/)).

**constant expression**

Expressions that **can** (not must) be fully evaluated at compile time, and the results remain unchanged throughout the lifetime of the program.

Commonly contain:

- Literals (e.g. ‘5’, ‘1.2’)
- Most operators with constant expression operands (e.g. `3 + 4`, `2 * sizeof(int)`).
- Const integral variables with a constant expression initializer (e.g. `const int x { 5 };`). This is a historical exception -- in modern C++, constexpr variables are preferred.
- Constexpr variables (discussed in upcoming lesson [5.6 -- Constexpr variables](https://www.learncpp.com/cpp-tutorial/constexpr-variables/)).
- Constexpr function calls with constant expression arguments (see [F.1 -- Constexpr functions](https://www.learncpp.com/cpp-tutorial/constexpr-functions/)).

<div style="border: 2px solid #c7c7c7; background-color: #f4f4f4; border-radius: 8px; padding: 14px; margin: 5px">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        For advanced readers
    </p>
    <p style="margin: 1;">
        Constant expressions can also contain:<br>
		Constant expressions 还可以包含：
    </p>
    <p style="margin: 1;">
        ● Non-type template parameters (see 11.9 -- Non-type template parameters).<br>
        ● Enumerators (see 13.2 -- Unscoped enumerations).<br>
        ● Type traits (see the cppreference page for type traits).<br>
        ● Constexpr lambda expressions (see 20.6 -- Introduction to lambdas (anonymous functions)).
    </p>
</div>
<div style="border: 2px solid #9caad4; background-color: #dfe7ff; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Tip
    </p>
    <p style="margin: 1;">
        Constant expressions can not contain:<br>
		Constant expressions 不可以包含：
    </p>
    <p style="margin: 1;">
        ● Non-const variables.<br>
        ● Const non-integral variables, even when they have a constant expression initializer (e.g. const double d { 1.2 };). To use such variables in a constant expression, define them as constexpr variables instead (see lesson 5.6 -- Constexpr variables).<br>
        ● The return values of non-constexpr functions (even when the return expression is a constant expression).<br>
        ● Function parameters (even when the function is constexpr).<br>
        ● Operators with operands that are not constant expressions (e.g. x + y when x or y is not a constant expression, or std::cout << "hello\n" as std::cout is not a constant expression).<br>
        ● Operators new, delete, throw, typeid, and operator, (comma).
    </p>
</div>

```cpp
#include <iostream>

int getNumber()
{
    std::cout << "Enter a number: ";
    int y{};
    std::cin >> y; // can only execute at runtime

    return y;      // this return expression is a runtime expression
}

// The return value of a non-constexpr function is a runtime expression
// even when the return expression is a constant expression
int five()
{
    return 5;      // this return expression is a constant expression
}

int main()
{
    // Literals can be used in constant expressions
    5;                           // constant expression
    1.2;                         // constant expression
    "Hello world!";              // constant expression

    // Most operators that have constant expression operands can be used in constant expressions
    5 + 6;                       // constant expression
    1.2 * 3.4;                   // constant expression
    8 - 5.6;                     // constant expression (even though operands have different types)
    sizeof(int) + 1;             // constant expression (sizeof can be determined at compile-time)

    // The return values of non-constexpr functions can only be used in runtime expressions
    getNumber();                 // runtime expression
    five();                      // runtime expression (even though the return expression is a constant expression)

    // Operators without constant expression operands can only be used in runtime expressions
    std::cout << 5;              // runtime expression (std::cout isn't a constant expression operand)

    return 0;
}
```

```cpp
// Const integral variables with a constant expression initializer can be used in constant expressions:
const int a { 5 };           // a is usable in constant expressions
const int b { a };           // b is usable in constant expressions (a is a constant expression per the prior statement)
const long c { a + 2 };      // c is usable in constant expressions (operator+ has constant expression operands)

// Other variables cannot be used in constant expressions (even when they have a constant expression initializer):
int d { 5 };                 // d is not usable in constant expressions (d is non-const)
const int e { d };           // e is not usable in constant expressions (initializer is not a constant expression)
const double f { 1.2 };      // f is not usable in constant expressions (not a const integral variable)
```

constant expression isn't always evaluated at compile-time

```cpp
const int x { 3 + 4 }; // constant expression 3 + 4 must be evaluated at compile-time
int y { 3 + 4 };       // constant expression 3 + 4 may be evaluated at compile-time or runtime
```

<div style="border: 2px solid #9caad4; background-color: #dfe7ff; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Tip
    </p>
    <p style="margin: 1;">
        The likelihood that an expression is fully evaluated at compile-time can be categorized as follows:<br>
		表达式在编译时被完全计算的可能性分为以下几类：
    </p>
    <p style="margin: 1;">
        ● Never: A non-constant expression where the compiler is not able to determine all values at compile-time.<br>
        ● Possibly: A non-constant expression where the compiler is able to determine all values at compile-time (optimized under the as-if rule).<br>
        ● Likely: A constant expression used in a context that does not require a constant expression.<br>
        ● Always: A constant expression used in a context that requires a constant expression.
    </p>
</div>

<div style="border: 2px solid #c7c7c7; background-color: #f4f4f4; border-radius: 8px; padding: 14px; margin: 5px">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        For advanced readers
    </p>
    <p style="margin: 1;">
        So why doesn’t C++ require all constant expressions to be evaluated at compile-time? There are at least two good reasons:<br>
		那么，为什么 C++ 不要求在编译时计算所有常量表达式呢？至少有两个很好的理由：
    </p>
    <p style="margin: 1;">
        1. Compile-time evaluation makes debugging harder. If our code has a buggy calculation that is evaluated at compile-time, we have limited tools to diagnose the issue. Allowing non-required constant expressions to be evaluated at runtime (typically when optimizations are turned off) enables runtime debugging of our code. Being able to step through and inspect the state of our programs while they are running can make finding bugs easier.<br>
        编译时求值使调试更加困难。如果我们的代码有一个在编译时评估的有缺陷的计算，那么我们诊断该问题的工具有限。允许在运行时（通常在关闭优化时）计算非必需的常量表达式，可以对代码进行运行时调试。能够在程序运行时单步调试并检查程序的状态，可以更轻松地查找 bug。
    </p>
    <p style="margin: 1;">
        2. To provide the compiler with the flexibility to optimize as it sees fit (or as influenced by compiler options). For example, a compiler might want to offer an option that defers all non-required constant expression evaluation to runtime, in order to improve compile times for developers.<br>
        为编译器提供灵活性，使其能够根据需要进行优化 （或受编译器选项的影响）。例如，编译器可能希望提供一个选项，将所有非必需的常量表达式计算推迟到运行时，以便缩短开发人员的编译时间。
    </p>
</div>

## 5.6 — Constexpr variables

### Constexpr keyword

Due to:
由于：

1. const 声明的变量是否可以作为常量表达式不容易判断。
2. const 并不能让编译器知道我们需要一个变量一定可以作为常量表达式。
3. 用 const 创建 compile-time 常量变量没有扩展到非整型变量。

`constexpr` keyword is designed to specifies the value of a variable or function can appear in constant expressions.
'constexpr' 关键字旨在指定一个变量或者函数的值可以出现在常量表达式中。

| keyword     | purpose                                          | initialization                                    | evaluation time                              |
| ----------- | ------------------------------------------------ | ------------------------------------------------- | -------------------------------------------- |
| `const`     | an object cannot be changed after initialization | must, and may be known at compile-time or runtime | can be evaluated at runtime.                 |
| `constexpr` | object can be used in a constant expression      | must, and must be known at compile-time.          | can be evaluated at runtime or compile-time. |

Unlike `const`, `constexpr` is not part of an object’s type. Therefore a variable defined as `constexpr int` actually has type `const int`.
不同于 `const`，`constexpr`不是对象类型的一部分，因此以`constexpr int`定义的变量实际上类型为`const int` 。

<div style="border: 2px solid #9cd49c; background-color: #dfffdf; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Best practice
    </p>
    <p style="margin: 1;">
        Any constant variable whose initializer is a <b>constant expression</b> should be declared as <code>constexpr</code>.<br>
        初始值设定项为<b>常量表达式</b>的任何常量变量都应声明为 <code>constexpr</code>。
	</p>
    <p style="margin: 1;">
        Any constant variable whose initializer is <b>not a constant expression</b> (making it a runtime constant) should be declared as <code>const</code>.<br>
        任何初始值设定项<b>不是常量表达式</b>（使其成为运行时常量）的常量变量都应声明为 <code>const</code>。
	</p>
</div>

<div style="border: 2px solid #c7c7c7; background-color: #f4f4f4; border-radius: 8px; padding: 14px; margin: 5px">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        For advanced readers
    </p>
    <p style="margin: 1;">
        In C and C++, the declaration of an array object (an object can hold multiple values) requires the length of the array (the number of values that it can hold) be known at compile-time (so the compiler can ensure the correct amount of memory is allocated for array objects).<br>
		在 C 和 C++ 中，数组对象的声明（一个对象可以保存多个值）需要在编译时知道数组的长度（它可以保存的值的数量）（以便编译器可以确保为数组对象分配正确的内存量）。
    </p>
    <p style="margin: 1;">
        In C, array length can be declared via a preprocessor macro, or via an enumerator, but not via a const variable. The C++ language standard allowed const integral types with a constant expression initializer to do that. Naturally, the constexpr integral types, which were also const integral types, were allowed too.<br>
        在C中，数组长度可以通过预处理宏、枚举声明，而不能通过常量变量。C++则允许使用常量表达式初始化的 const 整型这么做，自然地，costexpr 整型作为一种 const 整型也可以这么做。
    </p>
</div>

#### const and constexpr function parameters

Normal function parameters:

- If `const`, are treated as runtime constants because the initialization of function parameters happens at runtime;
- if `constexpr`, cannot be compiled.

| Term                  | Definition                                                   |
| --------------------- | ------------------------------------------------------------ |
| Compile-time constant | A value or non-modifiable object whose value must be known at compile time (e.g. literals and constexpr variables). |
| Constexpr             | Keyword that declares objects as compile-time constants (and functions that can be evaluated at compile-time). Informally, shorthand for “constant expression”. |
| Constant expression   | An expression that contains only compile-time constants and operators/functions that support compile-time evaluation. |
| Runtime expression    | An expression that is not a constant expression.             |
| Runtime constant      | A value or non-modifiable object that is not a compile-time constant. |

## 5.7 — Introduction to std::string

C-style string cannot use assignment
C-style string is danger when copy a larger one into the space allocated for a shorter one, undefined behavior will result.

```cpp
#include <string>

int main()
{
    std::string empty {}; // empty string
    std::string name { "Alex" }; // initialize name with string literal "Alex"
    name = "Jay";               // change name to "Jay", and so the length is changed
    std::cout << "My name is: " << name << '\n';
    std::cout << '[' << empty << ']';

    return 0;
}
```

<div style="border: 2px solid #9caad4; background-color: #dfe7ff; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Key insight
    </p>
    <p style="margin: 1;">
        If <code>std::string</code> doesn’t have enough memory to store a string, it will request additional memory (at runtime) using a form of memory allocation known as dynamic memory allocation. This ability to acquire additional memory is part of what makes <code>std::string</code> so flexible, but also comparatively slow.<br>
		如果 <code>std::string</code> 没有足够的内存来存储字符串，它将使用一种称为动态内存分配的内存分配方式（在运行时）请求额外的内存。这种获取额外内存的能力是 <code>std::string</code> 如此灵活但也相对较慢的部分原因。
    </p>
</div>

```cpp
#include <iostream>
#include <string>

int main()
{
    std::cout << "Enter your full name: ";
    std::string name{};
    std::cin >> name; // this won't work as expected since std::cin breaks on whitespace

    std::cout << "Enter your favorite color: ";
    std::string color{};
    std::cin >> color;

    std::cout << "Your name is " << name << " and your favorite color is " << color << '\n';

    return 0;
}
```

```bash
Enter your full name: John Doe
Enter your favorite color: Your name is John and your favorite color is Doe
```

```cpp
#include <iostream>
#include <string> // For std::string and std::getline

int main()
{
    std::cout << "Enter your full name: ";
    std::string name{};
    std::getline(std::cin >> std::ws, name); // read a full line of text into name

    std::cout << "Enter your favorite color: ";
    std::string color{};
    std::getline(std::cin >> std::ws, color); // read a full line of text into color

    std::cout << "Your name is " << name << " and your favorite color is " << color << '\n';

    return 0;
}
```

```
Enter your full name: John Doe
Enter your favorite color: blue
Your name is John Doe and your favorite color is blue
```

### What is `std::ws`?

```cpp
#include <iostream>
#include <string>

int main()
{
    std::cout << "Pick 1 or 2: ";
    int choice{};
    std::cin >> choice;  // get "2\n", '2' to choice as 2, '\n' reserved

    std::cout << "Now enter your name: ";
    std::string name{};
    std::getline(std::cin, name); // note: no std::ws here, just use '\n' above to name and won't wait user's input
    std::getline(std::cin >> std::ws, name); // note: added std::ws here

    std::cout << "Hello, " << name << ", you picked " << choice << '\n';

    return 0;
}
```

```
# no std::ws
Pick 1 or 2: 2
Now enter your name: Hello, , you picked 2
# have std::ws
Pick 1 or 2: 2
Now enter your name: Alex
Hello, Alex, you picked 2
```

<div style="border: 2px solid #9cd49c; background-color: #dfffdf; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Best practice
    </p>
    <p style="margin: 1;">
        If using <code>std::getline()</code> to read strings, use <code>std::cin >> std::ws</code> input manipulator to ignore leading whitespace. This needs to be done for each <code>std::getline()</code> call, as <code>std::ws</code> is not preserved across calls.<br>
        如果使用 <code>std：：getline()</code> 读取字符串，请使用 <code>std：：cin >>std：：ws</code> input 操纵器来忽略前导空格。这需要对每个 <code>std：：getline()</code> 调用完成，因为 <code>std：：ws</code> 不会在调用之间保留。
	</p>
	</p>
</div>

### `std::string.length()`

```cpp
#include <iostream>
#include <string>

int main()
{
    std::string name{ "Alex" };
    std::cout << name << " has " << name.length() << " characters\n";
    int length { static_cast<int>(name.length()) };

    return 0;
}
```

does not include the implicit null-terminator character (although `std::string` is required to be null-terminated since C++11). 不包括隐式 null 终止符字符（尽管自C++11起 `std::string` 以null结尾）。

returns an unsigned integral value (most likely of type `size_t`). 返回一个无符号整型值（很可能是`size_t`）。

### Initializing a `std::string` is expensive

Whenever a std::string is initialized, a copy of the string used to initialize it is made. Making copies of strings is expensive, so care should be taken to minimize the number of copies made.
每当初始化 std：：string 时，都会拷贝用于初始化它的字符串。拷贝字符串的成本很高，因此应注意尽量减少复制的数量。

### Do not pass `std::string` by value

Same to above, function parameter must be initialized with the argument.
同上，函数参数必须用实参初始化。

### Three status can returning a `std::string`

- A local variable of type `std::string`. `std：：string` 的局部变量。
- A `std::string` that has been returned by value from another function call or operator. 已由另一个函数调用或运算符的 value 返回的 `std：：string`。
- A `std::string` temporary that is created as part of the return statement. return 语句中创建的临时 `std：：string`。

上面这些情况可能会直接在调用者的内存空间构造而不用拷贝构造，或者触发移动语义（move semantics）

### `std::string` literals

```cpp
#include <iostream>
#include <string> // for std::string

int main()
{
    using namespace std::string_literals; // easy access to the s suffix

    std::cout << "foo\n";   // no suffix is a C-style string literal
    std::cout << "goo\n"s;  // s suffix is a std::string literal, = std::string { "goo\n", 4 }

    return 0;
}
```

### constexpr string (may not supported)

```cpp
#include <iostream>
#include <string>

int main()
{
    using namespace std::string_literals;
    constexpr std::string name{ "Alex"s }; // compile error

    return 0;
}
```

## 5.8 — Introduction to std::string_view

```cpp
#include <iostream>
#include <string>

void printString(std::string str) // str makes a copy of its initializer
{
    std::cout << str << '\n';
}

int main()
{
    std::string s{ "Hello, world!" }; // s makes a copy of its initializer
    printString(s);

    return 0;
}
```

To address the issue with `std::string` being expensive to initialize (or copy), C++17 introduced `std::string_view` (which lives in the <string_view> header). `std::string_view` provides **read-only access to an *existing* string** (a C-style string, a `std::string`, or another `std::string_view`) without making a copy.

为了解决 `std::string` 初始化（或复制）成本高昂的问题，C++17 引入了 std：：`string_view`（位于<string_view>中）。`std::string_view`提供对现有字符串（C 样式字符串、`std::string` 或另一个 `std::string_view`）的只读访问，而无需制作副本。

### initialization

```cpp
std::string_view s1 { "Hello, world!" }; // initialize with C-style string literal
std::cout << s1 << '\n';

std::string s{ "Hello, world!" };
std::string_view s2 { s };  // initialize with std::string
std::cout << s2 << '\n';

std::string_view s3 { s2 }; // initialize with std::string_view
std::cout << s3 << '\n';
```

### function parameter

```cpp
#include <iostream>
#include <string>
#include <string_view>

void printSV(std::string_view str)
{
    std::cout << str << '\n';
}

int main()
{
    printSV("Hello, world!"); // call with C-style string literal

    std::string s2{ "Hello, world!" };
    printSV(s2); // call with std::string

    std::string_view s3 { s2 };
    printSV(s3); // call with std::string_view

    return 0;
}
```

### `std::string_view` will not implicitly convert to `std::string`

```cpp
#include <iostream>
#include <string>
#include <string_view>

void printString(std::string str)
{
	std::cout << str << '\n';
}

int main()
{
	std::string_view sv{ "Hello, world!" };

	// printString(sv);   // compile error: won't implicitly convert std::string_view to a std::string

	std::string s{ sv }; // okay: we can create std::string using std::string_view initializer
	printString(s);      // and call the function with the std::string

	printString(static_cast<std::string>(sv)); // okay: we can explicitly cast a std::string_view to a std::string

	return 0;
}
```

### Assignment = changes what the `std::string_view` is viewing

Assigning a new string to a `std::string_view` causes the `std::string_view` to view the new string. It does not modify the prior string being viewed in any way.
将新字符串分配给 `std::string_view` 会导致它 view to 新字符串。它不会以任何方式修改正在查看的先前字符串。

### `std::string_view` literals

```cpp
    using namespace std::string_literals;      // access the s suffix
    using namespace std::string_view_literals; // access the sv suffix

    std::cout << "foo\n";   // no suffix is a C-style string literal
    std::cout << "goo\n"s;  // s suffix is a std::string literal
    std::cout << "moo\n"sv; // sv suffix is a std::string_view literal
```

### constexpr string_view (full supported)

```cpp
constexpr std::string_view s{ "Hello, world!" }; // s is a string symbolic constant
std::cout << s << '\n'; // s will be replaced with "Hello, world!" at compile-time
```

## 5.9 — std::string_view (part 2) 

**std::string_view** is a viewer

While viewer (string_view) is destroyed, the viewee is not affected.

While viewee is destroyed, the viewer (string_view), called a **dangling** view now, result unexpected or undefined behavior.

So you should ensure the viewee's outlives the viewer (string_view).
所以你需要确保 viewee 比 viewer (string_view) 存活更久。

<div style="border: 2px solid #d89696; background-color: #ffd6d6; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Warning
    </p>
    <p style="margin: 1;">
        A view is dependent on the object being viewed. If the object being viewed is modified or destroyed while the view is still being used, unexpected or undefined behavior will result.<br>
        视图取决于正在查看的对象。如果正在查看的对象在视图仍在使用时被修改或销毁，则会导致意外或未定义的行为。
    </p>
</div>
### `std::string_view` is best used as a read-only function parameter

- no need copy
    不需要副本
- no risk that the string being viewed (the function argument) will be modified or destroyed
    没有被查看的字符串实参被修改或者销毁的风险

```cpp
#include <iostream>
#include <string>
#include <string_view>

void printSV(std::string_view str) // now a std::string_view, creates a view of the argument
{
    std::cout << str << '\n';
}

int main()
{
    printSV("Hello, world!"); // call with C-style string literal

    std::string s2{ "Hello, world!" };
    printSV(s2); // call with std::string

    std::string_view s3 { s2 };
    printSV(s3); // call with std::string_view

    return 0;
}
```



```cpp
using namespace std::string_literals;
using namespace std::string_view_literals; // access the sv suffix
std::string_view name_1 { "Alex"s }; // DONOT! "Alex"s creates a temporary std::string
std::string_view name_2 { "Alex" }; // OK "Alex"s creates a temporary std::string
std::string_view name_3 { "Alex"sv }; // OK "Alex"s creates a temporary std::string
```



<div style="border: 2px solid #d89696; background-color: #ffd6d6; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Warning
    </p>
    <p style="margin: 1;">
        Do not initialize a <code>std::string_view</code> with a <code>std::string</code> literal, as this will leave the <code>std::string_view</code> dangling.<br>
        不要以<code>std::string</code>字面值初始化一个<code>std::string_view</code>，这会导致<code>std::string_view</code>悬挂。
    </p>
</div>

### Be careful returning a `std::string_view`

Two main safe cases:
两个主要的安全情况

1. return `std::string_view` viewed C-style string literals
2. return `std::string_view` viewed `std::string_view` function parameter

### `remove_prefix()` & `remove_suffix()`

```cpp
	std::string_view str{ "Peach" };	std::cout << str << '\n';	// Remove 1 character from the left side of the view	str.remove_prefix(1);	std::cout << str << '\n';	// Remove 2 characters from the right side of the view	str.remove_suffix(2);	std::cout << str << '\n';	str = "Peach"; // reset the view	std::cout << str << '\n';i
```

once `remove_prefix()` and `remove_suffix()` have been called, the only way to reset the view is by reassigning the source string to it again.
一旦 `remove_prefix()` 和 `remove_suffix()` 被调用，重置视图的唯一方法是再次将源字符串重新分配给它（只能 remove 而不能恢复）。

Due to the `remove_suffix()`, `std::string_view` may or may not be null-terminated.
由于 `remove_suffix()`，`std::string_view` 可能不会以 null 结尾。

### A quick guide on when to use `std::string` vs `std::string_view`

#### Use a `std::string` variable when:

- You need a string that you can modify.
    您需要一个可以修改的字符串。
- You need to store user-inputted text.
    您需要存储用户输入的文本。
- You need to store the return value of a function that returns a `std::string`.
    您需要存储返回 astd：：string 的函数的返回值。

#### Use a `std::string_view` variable when:

- You need read-only access to part or all of a string that already exists elsewhere and will not be modified or destroyed before use of the `std::string_view` is complete.
    您需要对已存在于其他位置的字符串的部分或全部进行只读访问，并且在使用 thestd：：string_viewis 完成之前不会被修改或销毁。
- You need a symbolic constant for a C-style string.
    您需要 C 样式字符串的符号常量。
- In the vast majority of cases, integer exponentiation will overflow the integral type. This is likely why such a function wasn’t included in the standard library in the first place.
    在绝大多数情况下，整数幂运算会使整型溢出。这可能就是为什么 standard 库中最初没有包含这样的函数的原因。
- You need to continue viewing the return value of a function that returns a C-style string or a non-dangling `std::string_view`.
    您需要继续查看返回 C 样式字符串或非 danglingstd：：string_view 的函数的返回值。

#### Use a `std::string` function parameter when:

- The function needs to modify the string passed in as an argument without affecting the caller. This is rare.
    该函数需要修改作为参数传入的字符串，而不会影响调用方。这种情况很少见。
- You are using language standard C++14 or older and aren’t comfortable using references yet.
    您使用的是语言标准 C++14 或更早版本，并且还不习惯使用引用。

#### Use a `std::string_view` function parameter when:

- The function needs a read-only string.
    该函数需要一个只读字符串。
- The function needs to work with non-null-terminated strings.
    该函数需要使用非以 null 结尾的字符串。

#### Use a `const std::string&` function parameter when:

- You are using language standard C++14 or older, and the function needs a read-only string to work with (as `std::string_view` is not available until C++17).
- You are calling other functions that require a `const std::string`, `const std::string&`, or const C-style string (as `std::string_view` may not be null-terminated).

#### Use a `std::string&` function parameter when:

- You are using a `std::string` as an out-parameter (see [12.13 -- In and out parameters](https://www.learncpp.com/cpp-tutorial/in-and-out-parameters/)).
- You are calling other functions that require a `std::string&`, or non-const C-style string.

#### Use a `std::string` return type when:

- The return value is a `std::string` local variable or function parameter.
    返回值为 astd：：stringlocal 变量或函数参数。
- The return value is a function call or operator that returns a `std::string` by value.
    返回值是返回 astd：：stringby 值的函数调用或运算符。

#### Use a `std::string_view` return type when:

- The function returns a C-style string literal or local `std::string_view` that has been initialized with a C-style string literal.
    该函数返回 C 样式字符串文本或 localstd：：string_viewthat 已使用 C 样式字符串文本初始化。
- The function returns a `std::string_view` parameter. 该函数返回 astd：：string_viewparameter。

#### Use a `std::string_view` return type when:

- Writing an accessor for a `std::string_view` member.

#### Use a `std::string&` return type when:

- The function returns a `std::string&` parameter.

#### Use a `const std::string&` return type when:

- The function returns a `const std::string&` parameter.
- Writing an accessor for a `std::string` or `const std::string` member.
- The function returns a static (local or global) `const std::string`.

# 6 Operators

## 6.1 — Operator precedence and associativity

### Operator precedence & associativity

| Prec/Ass | Operator                                                     | Description                                                  | Pattern                                                      |
| :------- | :----------------------------------------------------------- | :----------------------------------------------------------- | :----------------------------------------------------------- |
| 1 L->R   | ::<br />::                                                   | Global scope (unary)<br />Namespace scope (binary)           | ::name<br />class_name::member_name                          |
| 2 L->R   | ()<br />()<br />type()<br />type{}<br />[]<br />.<br />-><br />++<br />––<br />typeid<br />const_cast<br />dynamic_cast<br />reinterpret_cast<br />static_cast<br />sizeof…<br />noexcept<br />alignof | Parentheses<br />Function call<br />Functional cast<br />List init temporary object (C++11)<br />Array subscript<br />Member access from object<br />Member access from object ptr<br />Post-increment<br />Post-decrement<br />Run-time type information<br />Cast away const<br />Run-time type-checked cast<br />Cast one type to another<br />Compile-time type-checked cast<br />Get parameter pack size<br />Compile-time exception check<br />Get type alignment | (expression)<br />function_name(arguments)<br />type(expression)<br />type{expression}<br />pointer[expression]<br />object.member_name<br />object_pointer->member_name<br />lvalue++<br />lvalue––<br />typeid(type)or typeid(expression)<br />const_cast\<type\>(expression)<br /> dynamic_cast\<type\>(expression)<br /> reinterpret_cast\<type\>(expression)<br /> static_cast\<type\>(expression)<br /> sizeof…(expression)<br /> noexcept(expression)<br /> alignof(type) |
| 3 R->L   | +<br />-<br />++<br />––<br />!<br />not<br />~<br />(type)<br />sizeof<br />co_await<br />&<br />*<br />new<br />new[]<br />delete<br />delete[] | Unary plus<br />Unary minus<br />Pre-increment<br />Pre-decrement<br />Logical NOT<br />Logical NOT<br />Bitwise NOT<br />C-style cast<br />Size in bytes<br />Await asynchronous call<br />Address of<br />Dereference<br />Dynamic memory allocation<br />Dynamic array allocation<br />Dynamic memory deletion<br />Dynamic array deletion | +expression<br />-expression<br />++lvalue<br />––lvalue<br />!expression<br />not expression<br />~expression<br />(new_type)expression<br />sizeof(type) or sizeof(expression)<br />co_await expression (C++20)<br />&lvalue<br />*expression<br />new type<br />new type[expression]<br />delete pointer<br />delete[] pointer |
| 4 L->R   | ->*<br />.*                                                  | Member pointer selector<br />Member object selector          | object_pointer->*pointer_to_member<br />object.*pointer_to_member |
| 5 L->R   | *<br />/<br />%                                              | Multiplication<br />Division<br />Remainder                  | expression * expression<br />expression / expression<br />expression % expression |
| 6 L->R   | +<br />-                                                     | Addition<br />Subtraction                                    | expression + expression<br />expression - expression         |
| 7 L->R   | <<<br />>>                                                   | Bitwise shift left / Insertion<br />Bitwise shift right / Extraction | expression << expression<br />expression >> expression       |
| 8 L->R   | <=>                                                          | Three-way comparison (C++20)                                 | expression <=> expression                                    |
| 9 L->R   | <<br /><=<br />><br />>=                                     | Comparison less than <br />Comparison less than or equals<br />Comparison greater than<br />Comparison greater than or equals | expression < expression<br />expression <= expression<br />expression > expression<br />expression >= expression |
| 10 L->R  | ==<br />!=                                                   | Equality<br />Inequality                                     | expression == expression<br />expression != expression       |
| 11 L->R  | &                                                            | Bitwise AND                                                  | expression & expression                                      |
| 12 L->R  | ^                                                            | Bitwise XOR                                                  | expression ^ expression                                      |
| 13 L->R  | \|                                                           | Bitwise OR                                                   | expression \| expression                                     |
| 14 L->R  | &&<br />and                                                  | Logical AND<br />Logical AND                                 | expression && expression<br />expression and expression      |
| 15 L->R  | \|\|<br />or                                                 | Logical OR<br />Logical OR                                   | expression \|\| expression<br />expression or expression     |
| 16 R->L  | throw<br />co_yield<br />? :<br />=<br />*=<br />/=<br />%=<br />+=<br />-=<br /><<=<br />>>=<br />&=<br />\|=<br />^= | Throw expression<br />Yield expression (C++20)<br />Conditional<br />Assignment<br />Multiplication assignment<br />Division assignment<br />Remainder assignment<br />Addition assignment<br />Subtraction assignment<br />Bitwise shift left assignment<br />Bitwise shift right assignment<br />Bitwise AND assignment<br />Bitwise OR assignment<br />Bitwise XOR assignment | throw expression<br />co_yield expression<br />expression ? expression: expression<br />lvalue = expression<br />lvalue *= expression<br />lvalue /= expression<br /> lvalue %= expression<br /> lvalue += expression<br /> lvalue -= expression<br /> lvalue <<= expression<br /> lvalue >>= expression<br /> lvalue &= expression<br /> lvalue \|= expression<br /> lvalue ^= expression |
| 17 L->R  | ,                                                            | Comma operator                                               | expression, expression                                       |

<div style="border: 2px solid #9caad4; background-color: #dfe7ff; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Q: Where is the exponent operator?
    </p>
    <p style="margin: 1;">
        C++ doesn’t include exponentiation operator. Discuss exponentiation in lesson [6.3 -- Remainder and Exponentiation](https://www.learncpp.com/cpp-tutorial/remainder-and-exponentiation/).<br>
		C++没有幂运算的运算符，在6.3将讨论幂运算。
    </p>
</div>

<div style="border: 2px solid #9cd49c; background-color: #dfffdf; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Best practice
    </p>
    <p style="margin: 1;">
        Use parentheses to make it clear how a non-trivial compound expression should evaluate (even if they are technically unnecessary).<br>
        使用括号来明确组合表达式应该如何计算（即使它们在技术上是不必要的）。
	</p>
    <p style="margin: 1;">
        A good rule of thumb is: Parenthesize everything, except addition, subtraction, multiplication, and division. Expressions that have a single assignment operator (and no comma operator) do not need to have the right operand of the assignment wrapped in parenthesis.<br>
        一个好的经验法则是：将所有内容都括起来，除了加法、减法、乘法和除法。具有单个赋值运算符（且没有逗号运算符）的表达式不需要将赋值的正确作数括在括号中。
	</p>
</div>

#### The order of evaluation of operands (including function arguments) is mostly unspecified

```c++
a * b + c * d
# same to
(a * b) + (c * d)
# may (a * b) first or may (c * d) first
```

```cpp
int getValue()
{
    std::cout << "Enter an integer: ";

    int x{};
    std::cin >> x;
    return x;
}

void printCalculation(int x, int y, int z)
{
    std::cout << x + (y * z);
}

int main()
{
    printCalculation(getValue(), getValue(), getValue()); // this line is ambiguous

    return 0;
}
```

<div style="border: 2px solid #9caad4; background-color: #dfe7ff; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Tip
    </p>
    <p style="margin: 1;">
        The Clang compiler evaluates arguments in left-to-right order. The GCC compiler evaluates arguments in right-to-left order.<br>
		Clang 编译器按从左到右的顺序计算参数。GCC 编译器按从右到左的顺序计算参数。
    </p>
</div>
## 6.2 — Arithmetic operators

### Integer and floating point division 整数和浮点除法

If either (or both) of the operands are floating, `%` performs floating point division that returns a floating point value. 如果其中一个（或两个）操作数是浮点值，则 `%` 将执行浮点除法返回浮点值。

If both of the operands are integers, `%` performs integer division instead. It drops any fractions (rounded down while it is greater than 0, rounded up while it is less than 0) and returns an integer value. 如果两个操作数都是整数，则 `%` 将改为执行整数除法。会丢弃任何分数（大于0时候向下取整，小于0时候向上取整）并返回一个整数值。

#### Using static_cast<> to do floating point division with integers

```c++
constexpr int x{ 7 };
constexpr int y{ 4 };

std::cout << "int / int = " << x / y << '\n';
std::cout << "double / int = " << static_cast<double>(x) / y << '\n';
std::cout << "int / double = " << x / static_cast<double>(y) << '\n';
std::cout << "double / double = " << static_cast<double>(x) / static_cast<double>(y) << '\n';
```

```
int / int = 1
double / int = 1.75
int / double = 1.75
double / double = 1.75
```

### Dividing by 0 and 0.0

1. Dividing by 0: undefined behavior
2. Dividing by 0.0: `NaN`,`Inf`, or undefined behavior

## 6.3 — Remainder and Exponentiation

### The remainder operator (**`operator%`**)

```c++
if ((x % y) == 0)
    // x is evenly divisible by y
```

#### Remainder with negative numbers

`x % y` always returns results with the sign of *x*.

#### write a function that returns whether a number is odd

```cpp
bool isOdd(int x)
{
    return (x % 2) == 1; // fails when x is -5
}
```

Above can't work when x is negative.

```cpp
bool isOdd(int x)
{
    return (x % 2) != 0; // could also write return (x % 2)
}
```

### Exponents in C++

```c++
#include <cmath>

double x{ std::pow(3.0, 4.0) }; // 3 to the 4th power
```

```c++
float       pow ( float base, float exp );
double      pow ( double base, double exp );
float       pow ( float base, int exp );
double      pow ( double base, int exp );
```

Note that `pow()` must return floating type. 注意 `pow()` 一定会返回浮点类型

If you want to do integer exponentiation, you’re best off using your own function to do so. 如果想要整型幂运算，最好自己实现

```cpp
#include <cassert> // for assert
#include <cstdint> // for std::int64_t
#include <iostream>

// note: exp must be non-negative
// note: does not perform range/overflow checking, use with caution
constexpr std::int64_t powint(std::int64_t base, int exp)
{
	assert(exp >= 0 && "powint: exp parameter has negative value");

	// Handle 0 case
	if (base == 0)
		return (exp == 0) ? 1 : 0;

	std::int64_t result{ 1 };
	while (exp > 0)
	{
		if (exp & 1)  // if exp is odd
			result *= base;
		exp /= 2;
		base *= base;
	}

	return result;
}

int main()
{
	std::cout << powint(7, 12) << '\n'; // 7 to the 12th power
i
	return 0;
}
```

<div style="border: 2px solid #d89696; background-color: #ffd6d6; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Warning
    </p>
    <p style="margin: 1;">
        In the vast majority of cases, integer exponentiation will overflow the integral type. This is likely why such a function wasn’t included in the standard library in the first place.<br>
        在绝大多数情况下，整数幂运算会使整型溢出。这可能就是为什么标准库中最初没有包含这样的函数的原因。
    </p>
</div>
A safer version that checks for overflow:
一个会检查溢出的更安全版本：

```cpp
#include <cassert> // for assert
#include <cstdint> // for std::int64_t
#include <iostream>
#include <limits> // for std::numeric_limits

// A safer (but slower) version of powint() that checks for overflow
// note: exp must be non-negative
// Returns std::numeric_limits<std::int64_t>::max() if overflow occurs
constexpr std::int64_t powint_safe(std::int64_t base, int exp)
{
    assert(exp >= 0 && "powint_safe: exp parameter has negative value");

    // Handle 0 case
    if (base == 0)
        return (exp == 0) ? 1 : 0;

    std::int64_t result { 1 };

    // To make the range checks easier, we'll ensure base is positive
    // We'll flip the result at the end if needed
    bool negativeResult{ false };

    if (base < 0)
    {
        base = -base;
        negativeResult = (exp & 1);
    }

    while (exp > 0)
    {
        if (exp & 1) // if exp is odd
        {
            // Check if result will overflow when multiplied by base
            if (result > std::numeric_limits<std::int64_t>::max() / base)
            {
                std::cerr << "powint_safe(): result overflowed\n";
                return std::numeric_limits<std::int64_t>::max();
            }

            result *= base;
        }

        exp /= 2;

        // If we're done, get out here
        if (exp <= 0)
            break;

        // The following only needs to execute if we're going to iterate again

        // Check if base will overflow when multiplied by base
        if (base > std::numeric_limits<std::int64_t>::max() / base)
        {
            std::cerr << "powint_safe(): base overflowed\n";
            return std::numeric_limits<std::int64_t>::max();
        }

        base *= base;
    }

    if (negativeResult)
        return -result;

    return result;
}

int main()
{
	std::cout << powint_safe(7, 12) << '\n'; // 7 to the 12th power
	std::cout << powint_safe(70, 12) << '\n'; // 70 to the 12th power (will return the max 64-bit int value)

	return 0;
}
```

## 6.4 — Increment/decrement operators, and side effects

| Operator                                    | Symbol | Form | Operation                                                    |
| :------------------------------------------ | :----- | :--- | :----------------------------------------------------------- |
| Prefix increment (pre-increment) 前缀递增   | ++     | ++x  | Increment x, then return x 递增 x，然后返回 x                |
| Prefix decrement (pre-decrement) 前缀递减   | ––     | ––x  | Decrement x, then return x 递减 x，然后返回 x                |
| Postfix increment (post-increment) 后缀递增 | ++     | x++  | Copy x, then increment x, then return the copy<br />复制 x，然后递增 x，然后返回副本 |
| Postfix decrement (post-decrement) 后缀递减 | ––     | x––  | Copy x, then decrement x, then return the copy<br />复制 x，然后递减 x，然后返回副本 |

Note that the postfix version takes a lot more steps, and thus may not be as performant as the prefix version.

<div style="border: 2px solid #9cd49c; background-color: #dfffdf; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Best practice
    </p>
    <p style="margin: 1;">
        Favor the prefix versions, as they are more performant and less likely to cause surprises. e.g. <code>for(int i = 0; i <10; ++i)</code> is preferred over <code>for(int i = 0; i <10; ++i)</code>.<br>
        首选前缀版本，因为它们的性能更高，不太可能引起意外。例如，<code>for(int i = 0; i <10; ++i)</code> 相比 <code>for(int i = 0; i <10; ++i)</code>来说更好。
	</p>
</div>

**Side effects can cause order of evaluation issues**

```cpp
#include <iostream>

int add(int x, int y)
{
    return x + y;
}

int main()
{
    int x { 5 };
    int value{ add(x, ++x) }; // undefined behavior: is this 5 + 6, or 6 + 6?
    // It depends on what order your compiler evaluates the function arguments in
    std::cout << value << '\n'; // value could be 11 or 12, depending on how the above line evaluates!
    return 0;
}
```

## 6.5 — The comma operator

| Operator | Symbol | Form | Operation                             |
| :------- | :----- | :--- | :------------------------------------ |
| Comma    | ,      | x, y | Evaluate x then y, returns value of y |

Note that comma has the lowest precedence of all the operators, even lower than assignment. Because of this, the following two lines of code do different things:

```cpp
z = (a, b); // evaluate (a, b) first to get result of b, then assign that value to variable z.
z = a, b; // evaluates as "(z = a), b", so z gets assigned the value of a, and b is evaluated and discarded.
```

## 6.6 — The conditional operator

| Operator    | Symbol | Form      | Meaning                                                      |
| :---------- | :----- | :-------- | :----------------------------------------------------------- |
| Conditional | ?:     | c ? x : y | If conditional `c` is `true` then evaluate `x`, otherwise evaluate `y` |

<div style="border: 2px solid #9cd49c; background-color: #dfffdf; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Best practice
    </p>
    <p style="margin: 1;">
        Parenthesize the entire conditional operation (including operands) when used in a compound expression.<br>
        在复合表达式中使用时，将整个条件运算（包括操作数）括起来。。
	</p>
    <p style="margin: 1;">
        For readability, consider parenthesizing the condition if it contains any operators (other than the function call operator).<br>
        为了提高可读性，如果条件包含任何运算符（函数调用运算符除外），请考虑将条件括起来。
	</p>
</div>

**The type of the expressions must match or be convertible**

```cpp
std::cout << (true ? 1 : 2) << '\n';    // okay: both operands have matching type int
std::cout << (false ? 1 : 2.2) << '\n'; // okay: int value 1 converted to double
std::cout << (true ? -1 : 2u) << '\n';  // surprising result: -1 converted to unsigned int, result out of range
/*
1
2.2
4294967295
*/
```

## 6.7 — Relational operators and floating point comparisons

| Operator               | Symbol | Form   | Operation                                                |
| :--------------------- | :----- | :----- | :------------------------------------------------------- |
| Greater than           | >      | x > y  | true if x is greater than y, false otherwise             |
| Less than              | <      | x < y  | true if x is less than y, false otherwise                |
| Greater than or equals | >=     | x >= y | true if x is greater than or equal to y, false otherwise |
| Less than or equals    | <=     | x <= y | true if x is less than or equal to y, false otherwise    |
| Equality               | ==     | x == y | true if x equals y, false otherwise                      |
| Inequality             | !=     | x != y | true if x does not equal y, false otherwise              |

### Comparison of calculated floating point values can be problematic

```cpp
constexpr double d1{ 100.0 - 99.99 }; // should equal 0.01 mathematically
constexpr double d2{ 10.0 - 9.99 }; // should equal 0.01 mathematically

if (d1 == d2)
    std::cout << "d1 == d2" << '\n';
else if (d1 > d2)
    std::cout << "d1 > d2" << '\n'; // actually d1 = 0.010000000000005116 and d2 = 0.0099999999999997868
else if (d1 < d2)
    std::cout << "d1 < d2" << '\n';
```

Due to the floating point values are not precise, comparing floating point values using any of the relational operators can be dangerous!
由于浮点值是不精确的，用任何关系操作符比较浮点值都可能是危险的！

### Floating point equality and inequality

The equality operators  (== and !=) is the most dangerous operators in the relational operators between two floating point value.
相等操作符（==和!=）是两个浮点值之间的关系操作符中最危险的操作符。

<div style="border: 2px solid #d89696; background-color: #ffd6d6; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Warning
    </p>
    <p style="margin: 1;">
        Avoid using operator== and operator!= to compare floating point values if there is any chance those values have been calculated.<br>
        避免使用 == 和 != 来比较浮点值（如果有可能已计算这些值）。
    </p>
</div>

One exception case to the above: It is safe to compare a floating point literal with a variable of the same type that has been initialized with a literal of the same type, so long as the number of significant digits in each literal does not exceed the minimum precision for that type. Float has a minimum precision of 6 significant digits, and double has a minimum precision of 15 significant digits.
一个例外情况：将浮点 Literals 与已使用相同类型的 Literal 初始化的相同类型的变量进行比较是安全的，只要每个 Literals 中的有效位数不超过该类型的最小精度。Float 的最小精度为 6 位有效数字，double 的最小精度为 15 位有效数字。

It is mostly not safe to compare floating point literals of different types. For example, comparing `9.8f` to `9.8` will return false.
比较不同类型的浮点 Literals 通常是不安全的。例如，比较`9.8f`和`9.8`将返回 false。

<div style="border: 2px solid #9caad4; background-color: #dfe7ff; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Tip
    </p>
    <p style="margin: 1;">
        One exception case to the above: It is safe to compare a floating point literal with a variable of the same type that has been initialized with a literal of the same type, so long as the number of significant digits in each literal does not exceed the minimum precision for that type. Float has a minimum precision of 6 significant digits, and double has a minimum precision of 15 significant digits.<br>
		一个例外情况：将浮点 Literals 与已使用相同类型的 Literal 初始化的相同类型的变量进行比较是安全的，只要每个 Literals 中的有效位数不超过该类型的最小精度。Float 的最小精度为 6 位有效数字，double 的最小精度为 15 位有效数字。
    </p>
    <p style="margin: 1;">
        It is mostly not safe to compare floating point literals of different types. For example, comparing <code>9.8f</code> to <code>9.8</code> will return false.<br>
		比较不同类型的浮点 Literals 通常是不安全的。例如，比较<code>9.8f</code>和<code>9.8</code>将返回 false。
    </p>
</div>

### Comparing floating point numbers (advanced / optional reading)

A inconvenient solution:

```cpp
#include <cmath> // for std::abs()

// absEpsilon is an absolute value
bool approximatelyEqualAbs(double a, double b, double absEpsilon)
{
    // if the distance between a and b is less than or equal to absEpsilon, then a and b are "close enough"
    return std::abs(a - b) <= absEpsilon;
}
```

[Donald Knuth](https://en.wikipedia.org/wiki/Donald_Knuth), a famous computer scientist, suggested the following method in his book “The Art of Computer Programming, Volume II: Seminumerical Algorithms (Addison-Wesley, 1969)”:
[Donald Knuth](https://en.wikipedia.org/wiki/Donald_Knuth)著名计算机科学家在他的著作《计算机编程的艺术，第二卷：半数值算法》（Addison-Wesley，1969 年）中提出了以下方法：

```cpp
#include <algorithm> // for std::max
#include <cmath>     // for std::abs

// Return true if the difference between a and b is within epsilon percent of the larger of a and b
bool approximatelyEqualRel(double a, double b, double relEpsilon)
{
	return (std::abs(a - b) <= (std::max(std::abs(a), std::abs(b)) * relEpsilon));
}
```

But `approximatelyEqualRel()` will be invalidated while the input floating point value are mathematical zero.
但是当两个浮点值输入是数学上的0时，`approximatelyEqualRel()`会失效。

A compositive solution:

```cpp
// Return true if the difference between a and b is less than or equal to absEpsilon, or within relEpsilon percent of the larger of a and b
bool approximatelyEqualAbsRel(double a, double b, double absEpsilon, double relEpsilon)
{
    // Check if the numbers are really close -- needed when comparing numbers near zero.
    if (std::abs(a - b) <= absEpsilon)
        return true;
    // Otherwise fall back to Knuth's algorithm
    return approximatelyEqualRel(a, b, relEpsilon);
}
```

## 6.8 — Logical operators

| Operator    | Symbol | Example Usage | Operation                                                    |
| :---------- | :----- | :------------ | :----------------------------------------------------------- |
| Logical NOT | !      | !x            | true if x is false, or false if x is true<br />如果 x 为 false，则为 true，如果 x 为 true，则为 false。 |
| Logical AND | &&     | x && y        | true if x and y are both true, false otherwise<br />如果 x 和 y 都为 true，则为 true，否则为 false |
| Logical OR  | \|\|   | x \|\| y      | true if either (or both) x or y are true, false otherwise<br />如果 x 和 y 都为 true，则为 true，否则为 false |

**Short circuit evaluation**

```cpp
x == 1 && y == 2
z == 1 || z == 2
```

If `x==1` is false, the expression must return false. Then `y == 2` won't be evaluated for optimization purposes.
如果`x==1`为false表达式结果一定是false，于是`y == 2`不会被计算以优化效率。

Similarly, if `z == 1`, the `z == 2` won't be evaluated.
同样地，如果`z == 1`为真，`z == 2` 不会被计算。

<div style="border: 2px solid #d89696; background-color: #ffd6d6; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Warning
    </p>
    <p style="margin: 1;">
        Short circuit evaluation may cause Logical OR and Logical AND to not evaluate the right operand. Avoid using expressions with side effects in conjunction with these operators.<br>
        短路计算可能会导致 Logical ORandLogical AND 不计算正确的作数。避免将具有副作用的表达式与这些运算符结合使用。
    </p>
</div>

<div style="border: 2px solid #c7c7c7; background-color: #f4f4f4; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        For advanced readers
    </p>
    <p style="margin: 1;">
    Only the built-in versions of these operators perform short-circuit evaluation. If you overload these operators to make them work with your own types, those overloaded operators will not perform short-circuit evaluation.<br>
    只有这些运算符的内置版本才会执行短路计算。如果重载这些运算符以使它们与您自己的类型一起使用，则这些重载运算符将不会执行短路计算。
    </p>
</div>

### Mixing ANDs and ORs

*logical AND* has higher precedence than *logical OR* !
逻辑AND比逻辑OR的优先级更高！

<div style="border: 2px solid #9cd49c; background-color: #dfffdf; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Best practice
    </p>
    <p style="margin: 1;">
        Explicitly parenthesizing When mixing logical AND and logical OR in a single expression!<br>
        在复合表达式中使用时，将整个条件运算（包括操作数）括起来。。
	</p>
</div>

**De Morgan’s laws**

`!(x && y)` is equivalent to `!x || !y`

| x     | y     | !x    | !y    | !(x && y) | !x \|\| !y |
| :---- | :---- | :---- | :---- | :-------- | :--------- |
| false | false | true  | true  | true      | true       |
| false | true  | true  | false | true      | true       |
| true  | false | false | true  | true      | true       |
| true  | true  | false | false | false     | false      |

`!(x || y)` is equivalent to `!x && !y`

| x     | y     | !x    | !y    | !(x \|\| y) | !x && !y |
| :---- | :---- | :---- | :---- | :---------- | :------- |
| false | false | true  | true  | true        | true     |
| false | true  | true  | false | false       | false    |
| true  | false | false | true  | false       | false    |
| true  | true  | false | false | false       | false    |

### No logical exclusive or (XOR) but `!=`

| Left operand | Right operand | logical XOR | operator!= |
| :----------- | :------------ | :---------- | :--------- |
| false        | false         | false       | false      |
| false        | true          | true        | true       |
| true         | false         | true        | true       |
| true         | true          | false       | false      |

# 7 Scope, Duration, and Linkage

## 7.1 — Compound statements (blocks)

<div style="border: 2px solid #9cd49c; background-color: #dfffdf; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Best practice
    </p>
    <p style="margin: 1;">
        Keep the nesting level of your functions to 3 or less. If your function has a need for more nested levels, consider refactoring your function into sub-functions.<br>
        将函数的嵌套级别保持为 3 或更低。如果您的函数需要更多嵌套级别，请考虑将函数重构为子函数。
	</p>
</div>

## 7.2 — User-defined namespaces and the scope resolution operator

```cpp
// main.cpp
#include "foo.h"
#include "goo.h"

int main()
{
    int x{doSomething(1, 2)};
    return 0;
}
```

```cpp
// foo.h
#ifndef FOO_H
#define FOO_H
int doSomething(int x, int y);
#endif
```

```cpp
// foo.cpp
#include "foo.h"

int doSomething(int x, int y)
{
    return x + y;
}
```

```cpp
// goo.h
#ifndef GOO_H
#define GOO_H
int doSomething(int x, int y);
#endif
```

```cpp
// goo.cpp
#include "goo.h"

int doSomething(int x, int y)
{
    return x - y;
}
```

Get a linker error:
得到链接错误：

```
goo.cpp:3: multiple definition of `doSomething(int, int)'; foo.cpp:3: first defined here
```

Using **user-defined namespaces** / **program-defined namespaces** to fix that:
使用 **user-defined namespaces** / **program-defined namespaces** 来修改：

```cpp
// main.cpp
#include "foo.h"
#include "goo.h"

int main()
{
    int x{Foo::doSomething(1, 2)};
    int y{Goo::doSomething(1, 2)};
    return 0;
}
```

```cpp
// foo.h
#ifndef FOO_H
#define FOO_H
namespace Foo {
    int doSomething(int x, int y);
}
#endif
```

```cpp
// foo.cpp
#include "foo.h"

namespace Foo // define a namespace named Foo
{
    int doSomething(int x, int y)
    {
        return x + y;
    }
}
```

```cpp
// goo.h
#ifndef GOO_H
#define GOO_H
namespace Goo {
    int doSomething(int x, int y);
}
#endif
```

```cpp
// goo.cpp
#include "goo.h"

namespace Goo // define a namespace named Foo
{
    int doSomething(int x, int y)
    {
        return x - y;
    }
}
```

Prefer namespace names starting with a capital letter
首选用大写字母开头为命名空间名称命名

**Using the scope resolution operator with no name prefix**

`UserNameSpace::doSomething` vs `::doSomething`

`::doSomething`=>`globalNamespace::doSomething`

```cpp
#include <iostream>

void print() // this print() lives in the global namespace
{
	std::cout << " there\n";
}

namespace Foo
{
	void print() // this print() lives in the Foo namespace
	{
		std::cout << "Hello";
	}
}

int main()
{
	Foo::print(); // call print() in Foo namespace
	::print();    // call print() in global namespace (same as just calling print() in this case)
	return 0;
}
```

**Identifier resolution from within a namespace**

`doSomething` vs `::doSomething`

`doSomething`=>`currentNamespcae::doSomething` no found =>`previousNamespcae::doSomething`=>`globalNamespace::doSomething`

```cpp
#include <iostream>

void print() // this print() lives in the global namespace
{
	std::cout << " there\n";
}

namespace Foo
{
	void print() // this print() lives in the Foo namespace
	{
		std::cout << "Hello";
	}
	void printHelloThere()
	{
		print();   // calls print() in Foo namespace
		::print(); // calls print() in global namespace
	}
}

int main()
{
	Foo::printHelloThere();
	return 0;
}
```

**Multiple namespace blocks in multiple locations are allowed**
**在多个位置的多个命名空间块是合法的**

### How to use namespaces

1. Any code that will be distributed should definitely be namespaced.
    任何将被分发的代码应该被空间命名

2. In multi-team organizations, two-level or even three-level namespaces
    在多团队组织中，二级甚至三级命名空间

- Project or library :: module (e.g. `Foologger::Lang`)
- Company or org :: project or library (e.g. `Foosoft::Foologger`)
- Company or org :: project or library :: module (e.g. `Foosoft::Foologger::Lang`)

## 7.3 — Local variables

**1. Local variables have block scope**

From their point of definition to the end of the block

**2. All variable names within a scope must be unique**

**3. Local variables have automatic storage duration**

Local variables are automatically created at the point of definition and automatically destroyed at the end of the block

**4. Local variables have no linkage**

An identifier’s **linkage** determines whether a declaration of that same identifier in a different scope refers to the same object (or function).
标识符的**linkage**属性确定不同范围内相同标识符的声明是否引用同一对象（或函数）。

```cpp
    int x { 2 }; // local variable, no linkage
    {
        int x { 3 }; // this declaration of x refers to a different object than the previous x
    }
```

## 7.4 — Introduction to global variables

### Declaring global variables and its scope

```cpp
#include <iostream>

// Variables declared outside of a function are global variables
int g_x {}; // global variable g_x

void doSomething()
{
    // ...
}

int main()
{
    //...
    return 0;
}
// g_x goes out of scope here
```

<div style="border: 2px solid #9cd49c; background-color: #dfffdf; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Best practice
    </p>
    <p style="margin: 1;">
        Prefer defining global variables inside a namespace rather than in the global namespace.<br>
        首选在命名空间内定义全局变量，而不是在全局命名空间中。
	</p>
</div>

**Global variables have static duration**

Global variables are created when the program starts (before `main()` begins execution), and destroyed when it ends. This is called **static duration**. Variables with *static duration* are sometimes called **static variables**.
全局变量在程序启动时创建 （`main()`开始执行之前），并在程序结束时销毁。这称为静态持续时间。具有静态持续时间的变量有时称为静态变量。

<div style="border: 2px solid #9cd49c; background-color: #dfffdf; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Best practice
    </p>
    <p style="margin: 1;">
        Consider using a “g” or “g_” prefix when naming global variables (especially those defined in the global namespace).<br>
        在命名全局变量（尤其是在全局命名空间中定义的变量）时，请考虑使用“g”或“g_”前缀。
	</p>
</div>
## 7.5 — Variable shadowing (name hiding)

```cpp
int main()
{ // outer block
    int apples { 5 }; // here's the outer block apples
    { // nested block
        // apples refers to outer block apples here
        std::cout << apples << '\n'; // print value of outer block apples

        int apples{ 0 }; // define apples in the scope of the nested block

        // apples now refers to the nested block apples
        // the outer block apples is temporarily hidden

        apples = 10; // this assigns value 10 to nested block apples, not outer block apples

        std::cout << apples << '\n'; // print value of nested block apples
    } // nested block apples destroyed
    std::cout << apples << '\n'; // prints value of outer block apples
    return 0;
} // outer block apples destroyed
```

```bash
5
10
5
```

```cpp
int value { 5 }; // global variable

void foo()
{
    std::cout << "global variable value: " << value << '\n'; // value is not shadowed here, so this refers to the global value
}

int main()
{
    int value { 7 }; // hides the global variable value (wherever local variable value is in scope)
    ++value; // increments local value, not global value
    std::cout << "local variable value: " << value << '\n';
    foo();
    return 0;
} // local value is destroyed
```

```
local variable value: 8
global variable value: 5
```

<div style="border: 2px solid #9cd49c; background-color: #dfffdf; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Best practice
    </p>
    <p style="margin: 1;">
        Avoid variable shadowing.<br>
        避免变量阴影。
	</p>
</div>
## 7.6 — Internal linkage

An identifier with **internal linkage** can be seen and used within a single translation unit, but it is not accessible from other translation units. This means that if two source files have identically named identifiers with internal linkage, those identifiers will be treated as independent (and do not result in an ODR violation for having duplicate definitions).
具有内部链接的标识符可以在单个翻译单元中查看和使用，但无法从其他翻译单元访问。这意味着，如果两个源文件具有具有内部链接的同名标识符，则这些标识符将被视为独立标识符（并且不会因具有重复定义而导致 ODR 违规）。

- Global variables identifiers: internal linkage while `static`, external linkage by default.
- `const`/`constexpr` global variables identifiers: internal linkage by default, external linkage while `extern`.
- Function identifiers: internal linkage while `static`, external linkage by default.
- Local variables identifiers: no linkage

### Global variables with internal linkage

```cpp
// a.cpp
[[maybe_unused]] constexpr int g_x { 2 }; // this internal g_x is only accessible within a.cpp
```

```cpp
// main.cpp
static int g_x { 3 }; // this separate internal g_x is only accessible within main.cpp

int main()
{
    std::cout << g_x << '\n'; // uses main.cpp's g_x, prints 3
    return 0;
}
```

### Const variables have internal linkage by default

The C++11 standard (appendix C) provides the rationale for why const variables have internal linkage by default: “Because const objects can be used as compile-time values in C++, this feature urges programmers to provide explicit initializer values for each const. This feature allows the user to put const objects in header files that are included in many compilation units.”
C++11 标准（附录 C）提供了 const 变量默认具有内部链接的基本原理：“由于 const 对象可以用作 C++ 中的编译时值，因此此功能敦促程序员为每个 const 提供显式初始值设定项值。此功能允许用户将 const 对象放在包含在许多编译单元中的头文件中。

The designers of C++ intended two things:
C++ 的设计者打算做两件事：

- Const objects should be usable in constant expressions. In order to be usable in a constant expression, the compiler must have seen a definition (not a declaration) so it be evaluated at compile-time.
    const 对象应该可以在常量表达式中使用。为了在常量表达式中可用，编译器必须看到定义（而不是声明），以便在编译时对其进行评估。
- Const objects should be able to be propagated via header files.
    Const 对象应该能够通过头文件传播。

Objects with external linkage can only be defined in a single translation unit without violating the ODR -- other translation units must access those objects via a forward declaration. If const objects had external linkage by default, they would only be usable in constant expressions in the single translation unit containing the definition, and they could not be effectively propagated via header files, as #including the header into more than one source file would result in an ODR violation.
具有外部链接的对象只能在单个翻译单元中定义，而不会违反 ODR —— 其他翻译单元必须通过正向声明访问这些对象。如果 const 对象默认具有外部链接，则它们只能在包含定义的单个翻译单元中的常量表达式中使用，并且无法通过头文件有效地传播，因为将头文件 #including 到多个源文件中将导致 ODR 冲突。

Objects with internal linkage can have a definition in each translation unit where they are needed without violating the ODR. This allows const objects to be placed in a header file and #included into as many translation units as desired without violating the ODR. And since each translation unit has a definition rather than a declaration, this ensures that those constants can be used in constant expressions within the translation unit.
具有内部链接的对象可以在每个需要它们的转换单元中有一个定义，而不会违反 ODR。这允许将 const 对象放置在头文件中，并根据需要 #included 到任意数量的转换单元中，而不会违反 ODR。由于每个翻译单元都有一个定义而不是声明，这确保了这些常量可以在翻译单元内的常量表达式中使用。

Inline variables (which can have external linkage without causing ODR violations) weren’t introduced until C++17.
内联变量（可以具有外部链接而不导致 ODR 冲突）直到 C++17 才被引入。

### Functions with internal linkage

```cpp
// add.cpp
// This function is declared as static, and can now be used only within this file
// Attempts to access it from another file via a function forward declaration will fail
[[maybe_unused]] static int add(int x, int y)
{
    return x + y;
}
```

```cpp
// main.cpp
int add(int x, int y); // forward declaration for function add

int main()
{
    std::cout << add(3, 4) << '\n';
    return 0;
}
```

### The one-definition rule and internal linkage

ODR: an object or function can’t have more than one definition, either within a file or a program. 一个对象或函数不能有多个定义，无论是在文件还是程序中。

internal objects (and functions) that are defined in different files are considered to be independent entities (even if their names and types are identical). 在不同文件中定义的内部对象（和函数）被视为独立实体（即使它们的名称和类型相同）。

## 7.7 — External linkage and variable forward declarations

An identifier with **external linkage** can be used both from the file in which it is defined, and from other code files (via a forward declaration).
具有外部链接的标识符既可以从定义它的文件中查看和使用，也可以从其他代码文件（通过前向声明）中使用。

| Type            | Definition        | Forward declaration                             |
| --------------- | ----------------- | ----------------------------------------------- |
| Function        | implicit external | implicit external                               |
| Global variable | implicit external | explicit external (otherwise become definition) |

Note that the **const globals** have *internal links* by default, while the **non-const globals** have *external links* by default.

```cpp
// Global variable forward declarations (extern w/ no initializer):
extern int g_y;                 // forward declaration for non-constant global variable
extern const int g_y;           // forward declaration for const global variable
extern constexpr int g_y;       // not allowed: constexpr variables can't be forward declared

// External global variable definitions (no extern)
int g_x;                        // defines non-initialized external global variable (zero initialized by default)
int g_x { 1 };                  // defines initialized external global variable
// External const global variable definitions (extern w/ initializer)
extern const int g_x { 2 };     // defines initialized const external global variable
extern constexpr int g_x { 3 }; // defines initialized constexpr external global variable
```

<div style="border: 2px solid #9cd49c; background-color: #dfffdf; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Best practice
    </p>
    <p style="margin: 1;">
        Only use <code>extern</code> for global variable forward declarations or const global variable definitions.<br>
        只在全局变量前向声明或全局 const 定义中使用<code>extern</code>。
	</p>
    <p style="margin: 1;">
        Do not use <code>extern</code> for non-const global variable definitions (they are implicitly <code>extern</code>).<br>
        不要对全局非 const 变量定义使用<code>extern</code>（他们是隐式<code>extern</code>的）。
	</p>
</div>

**Whether to use `extern` explicitly**

Definition:

| Type                      | `extern` explicitly ? |
| ------------------------- | --------------------- |
| Function                  | No                    |
| Non-const global variable | No                    |
| Const global variable     | Yes                   |

Forward declaration:

| Type                      | `extern` explicitly ? |
| ------------------------- | --------------------- |
| Function                  | No                    |
| Non-const global variable | Yes                   |
| Const global variable     | Yes                   |

## 7.8 — Why (non-const) global variables are evil

<div style="border: 2px solid #9cd49c; background-color: #dfffdf; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Best practice
    </p>
    <p style="margin: 1;">
        Use local variables instead of global variables whenever possible.<br>
        尽可能使用局部变量而不是全局变量。
	</p>
    <p style="margin: 1;">
        Do not use non-const variableswhenever possible.<br>
        尽可能不要使用非 const 全局变量。
	</p>
</div>

## 7.9 — Inline functions and variables

```cpp
int min(int x, int y)
{
    return (x < y) ? x : y;
}

int main()
{
    std::cout << min(5, 6) << '\n';
    std::cout << min(3, 2) << '\n';
    return 0;
}
```

For small functions (such as `min()` above), the overhead costs can be larger than the time needed to actually execute the function’s code!
对于小型函数（例如上面的`min()`），overhead开销成本可能大于实际执行函数代码所需的时间！

### C++ compiler Inline expansion

<div style="border: 2px solid #9caad4; background-color: #dfe7ff; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Tip
    </p>
    <p style="margin: 1;">
        Modern optimizing compilers make the decision about when functions should be expanded inline.<br>
		现代优化编译器决定何时应内联扩展函数。
    </p>
</div>

```cpp
#include <iostream>

int main()
{
    std::cout << ((5 < 6) ? 5 : 6) << '\n';
    std::cout << ((3 < 2) ? 3 : 2) << '\n';
    return 0;
}
```

### The historical inline keyword

Historically, C++ provided the keyword `inline` to be used as a hint to the compiler that a function would (probably) benefit from being expanded inline.
历史上的C++ 提供关键字`inline`用作对编译器的提示，即函数（可能）会从内联扩展中受益。

Modern optimizing compilers are typically good at determining which function calls should be made inline -- better than humans in most cases. As a result, the compiler will likely ignore or devalue any use of `inline` to request inline expansion for your functions.
现代优化编译器通常擅长确定哪些函数调用应该内联 —— 在大多数情况下，它比人类更好。因此，编译器可能会忽略或贬低任何请求对函数的内联扩展的`inline`使用。

<div style="border: 2px solid #9cd49c; background-color: #dfffdf; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Best practice
    </p>
    <p style="margin: 1;">
        Do not use the <code>inline</code> keyword to request inline expansion for your functions.<br>
        不要使用<code>inline</code>关键字为您的函数请求内联扩展。
	</p>
</div>

### The modern inline keyword

In modern C++, the term `inline` has evolved to mean “multiple definitions are allowed”. Thus, an inline function is one that is allowed to be defined in multiple translation units (without violating the ODR).
在现代 C++ 中，术语`inline`已演变为“允许多个定义”。因此，内联函数是允许在多个翻译单元中定义的函数（不违反 ODR）。

The inline function is particularly useful for **header-only libraries**. 内联函数对于仅头文件库非常有用。

<div style="border: 2px solid #c7c7c7; background-color: #f4f4f4; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        For advanced readers
    </p>
    <p style="margin: 1;">
        Implicitly inline functions 隐式内联函数:<br>
        <ul>
            <li>Functions defined inside a class, struct, or union type definition (14.3 -- Member functions).</li>
        	<li>Constexpr / consteval functions (F.1 -- Constexpr functions).</li>
        	<li>Functions implicitly instantiated from function templates (11.7 -- Function template instantiation).</li>
    	</ul>
    </p>
</div>

Note that making functions inline and defined in a header file increase compile times significantly. 注意将函数内联并在头文件中定义会显著增加编译时间。

<div style="border: 2px solid #9cd49c; background-color: #dfffdf; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Best practice
    </p>
    <p style="margin: 1;">
        Avoid the use of the <code>inline</code> keyword unless you have a specific, compelling reason to do so (e.g. you’re defining those functions or variables in a header file).<br>
        避免使用<code>inline</code>关键字，除非你有具体的、令人信服的理由（例如，你在头文件中定义这些函数或变量）。
	</p>
</div>

### Inline variables (C++17) 

C++17 introduces **inline variables**, which are variables that are allowed to be defined in multiple files.
C++17 引入了内联变量，这些变量是允许在多个文件中定义的变量。

<div style="border: 2px solid #c7c7c7; background-color: #f4f4f4; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        For advanced readers
    </p>
    <p style="margin: 1;">
        Implicitly inline variables 隐式内联变量:<br>
        <ul>
            <li>Static constexpr data members 15.6 -- Static member variables.</li>
    	</ul>
    </p>
</div>

## 7.10 — Sharing global constants across multiple files (using inline variables)

### Global constants as internal variables (before C++17)

constants.h:

```cpp
#ifndef CONSTANTS_H
#define CONSTANTS_H
namespace constants
{
    // Global constants have internal linkage by default
    constexpr double pi { 3.14159 };
    constexpr double avogadro { 6.0221413e23 };
    constexpr double myGravity { 9.2 }; // m/s^2 -- gravity is light on this planet\
}
#endif
```

main.cpp:

```cpp
#include "constants.h" // include a copy of each constant in this file
#include <iostream>
int main()
{
    double radius{};
    std::cin >> radius;
    std::cout << "The circumference is: " << 2 * radius * constants::pi << '\n';
    return 0;
}
```

Each .cpp file gets an independent version of the global variable due to const globals have internal linkage by default!
由于 const 全局变量具有内部链接，因此每个源文件都会获得全局变量的独立版本！

**Advantages:**

- Works prior to C++17.
    适用于 C++17 之前的版本。
- Can be used in constant expressions in any translation unit that includes them.
    可以在包含它们的任何翻译单元的常量表达式中使用。

**Downsides:**

- Changing anything in the header file requires recompiling files including the header.
    更改定义所在头文件中的任何内容都需要重新编译所有包括了那个头文件的文件。
- Each translation unit including the header gets its own copy of the variable (use much memory).
    每个翻译单元（包括 header）都会获得自己的变量副本（使用很多内存）。

### Global constants as external variables (before C++17)

constants.h:

```cpp
#ifndef CONSTANTS_H
#define CONSTANTS_H
namespace constants
{
    // Since the actual variables are inside a namespace, the forward declarations need to be inside a namespace as well
    // We can't forward declare variables as constexpr, but we can forward declare them as (runtime) const
    extern const double pi;
    extern const double avogadro;
    extern const double myGravity;
}
#endif
```

constants.cpp:

```cpp
#include "constants.h"
namespace constants
{
    // We use extern to ensure these have external linkage
    extern constexpr double pi { 3.14159 };
    extern constexpr double avogadro { 6.0221413e23 };
    extern constexpr double myGravity { 9.2 }; // m/s^2 -- gravity is light on this planet
}
```

Now the symbolic constants will get instantiated only once (in *constants.cpp*), and all uses of these constants will be linked to the version instantiated in *constants.cpp*.
现在，符号常量将只实例化一次 （在constants.cpp），并且这些常量的所有使用都将链接到constants.cpp中实例化的版本。

However, Each .cpp file include constants.h only gets the forward declarations instead of the variable definitions, this means these variables can’t be used in a constant expression and the compiler may not be able to optimize these as much.
但是，每个包括constants.h的源文件只得到了前向声明而没有变量定义，这意味着这些变量不能在常量表达式中使用，并且编译器可能无法对这些表达式进行尽可能多的优化。

**Advantages:**

- Works prior to C++17.
    适用于 C++17 之前的版本。
- Only one copy of each variable is required.
    每个变量只需要一个副本。
- Only requires recompilation of one file if the value of a constant changes.
    当常量的值发生变化时，只需要重新编译定义常量那一个文件。

**Disadvantages:**

- Forward declarations and variable definitions are in separate files, and must be kept in sync.
    前向声明和变量定义位于单独的文件中，必须保持同步。
- Variables not usable in constant expressions outside of the file in which they are defined.
    变量在定义它们的文件之外的常量表达式中不可用。

### Global constants as inline variables (after C++17)

Using global constexpr as inline variables to to avoid the disadvantages of both above ways.

<div style="border: 2px solid #c7c7c7; background-color: #f4f4f4; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        A reminder
    </p>
    <p style="margin: 1;">
        Constexpr functions are implicitly inline, but constexpr variables are not implicitly inline. If you want an inline constexpr variable, you must explicitly mark it as <code>inline</code>.<br>
        constexpr 函数是隐式内联的，但 constexpr 变量不是隐式内联的。如果你想要一个内联的 constexpr 变量，你必须显式地将其标记为 <code>inline</code>。
    </p>
</div>

<div style="border: 2px solid #9caad4; background-color: #dfe7ff; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Key insight
    </p>
    <p style="margin: 1;">
        Inline variables have external linkage by default to be visible to the linker. This is necessary so the linker can de-duplicate the definitions.<br>
        默认情况下，内联变量具有外部链接以使它们对链接器可见。这是必需的，以便链接器可以删除重复的定义。
    </p>
    <p style="margin: 1;">
        Non-inline constexpr variables have internal linkage. If included into multiple translation units, each translation unit will get its own copy of the variable. This is not an ODR violation because they are not exposed to the linker.<br>
        非内联 constexpr 变量具有内部链接。如果包含在多个翻译单元中，则每个翻译单元都将获得自己的变量副本。这不是 ODR 冲突，因为它们不会向链接器公开。
    </p>
</div>

constants.h:

```cpp
#ifndef CONSTANTS_H
#define CONSTANTS_H
namespace constants
{
    inline constexpr double pi { 3.14159 }; // note: now inline constexpr
    inline constexpr double avogadro { 6.0221413e23 };
    inline constexpr double myGravity { 9.2 }; // m/s^2 -- gravity is light on this planet
}
#endif
```

**Advantages:**

- Can be used in constant expressions in any translation unit that includes them.
    可以在包含它们的任何翻译单元的常量表达式中使用。
- Only one copy of each variable is required.
    每个变量只需要一个副本。

**Disadvantages:**

- Only works in C++17 onward.
    仅适用于 C++17 及更高版本。
- Changing anything in the header file requires recompiling files including the header.
    更改constants.h中的任何内容都需要重新编译所有包括头文件该的文件。

## 7.11 — Static local variables

### Static local (non-const) variables

Automatic duration (default):

```cpp
void incrementAndPrint()
{
    int value{ 1 }; // automatic duration by default
    ++value;
    std::cout << value << '\n';
} // value is destroyed here

int main()
{
    incrementAndPrint();
    incrementAndPrint();
    incrementAndPrint();
    return 0;
}
```

```
2
2
2
```

Static duration (using static keyword):

```cpp
void incrementAndPrint()
{
    static int s_value{ 1 }; // static duration via static keyword.  This initializer is only executed once.
    ++s_value;
    std::cout << s_value << '\n';
} // s_value is not destroyed here, but becomes inaccessible because it goes out of scope

int main()
{
    incrementAndPrint();
    incrementAndPrint();
    incrementAndPrint();
    return 0;
}
```

```
2
3
4
```

**Initialization time:**

- zero-initialized or constexpr initializer:
    program start 程序开始时
- no initializer or non-constexpr initializer:
    zero-initialized at program start. 程序开始时，零-初始化
    reinitialized the first time the variable definition is encountered (if non-constexpr initializer). 首次变量定义时再次初始化（如果 non-constexpr 初始化）
    skipped on subsequent calls. 跳过随后的定义

<div style="border: 2px solid #9cd49c; background-color: #dfffdf; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Best practice
    </p>
    <p style="margin: 1;">
        Initialize your static local variables.<br>
        初始化静态局部变量。
	</p>
</div>

<div style="border: 2px solid #9caad4; background-color: #dfe7ff; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Tip
    </p>
    <p style="margin: 1;">
        Use “s_” to prefix static (static duration) local variables.<br>
        使用 “s_” 来给静态 （静态持续时间） 局部变量添加前缀。
    </p>
</div>

The typical uses of static local variables is for unique ID generators. 典型的 static local variables 用途是唯一ID生成器。

```cpp
int generateID()
{
    static int s_itemID{ 0 };
    return s_itemID++; // makes copy of s_itemID, increments the real s_itemID, then returns the value in the copy
}
```

Static variables offer some of the benefit of global variables (they don’t get destroyed until the end of the program) while limiting their visibility to block scope. This makes them easier to understand and safer to use.
静态变量提供了全局变量的一些好处（它们在程序结束之前不会被销毁），同时将它们的可见性限制在块范围内。这使它们更易于理解且使用更安全。

<div style="border: 2px solid #9caad4; background-color: #dfe7ff; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Key insight
    </p>
    <p style="margin: 1;">
        A static local variable has block scope like a local variable, but its lifetime is until the end of the program like a global variable.<br>
        静态局部变量与局部变量一样具有块范围，但其生命周期与全局变量一样直到程序结束。
    </p>
</div>

### Static local const variables

**Advantages:**

When initialization is expensive, you only need to pay once. 当初始化成本昂贵时，只需付出一次。

<div style="border: 2px solid #9caad4; background-color: #dfe7ff; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Key insight
    </p>
    <p style="margin: 1;">
        Static local variables are best used to avoid expensive local object initialization each time a function is called.<br>
        静态局部变量最好用于避免每次调用函数时进行昂贵的本地对象初始化。
    </p>
</div>

**Don’t use static local variables to alter flow**

<div style="border: 2px solid #9cd49c; background-color: #dfffdf; border-radius: 8px; padding: 14px; margin: 5px;">
    <p style="font-weight: bold; font-size: 1.1em; margin: 0 0 8px 0;">
        Best practice
    </p>
    <p style="margin: 1;">
        Const static local variables are generally okay.<br>
        const static 局部变量通常是没问题。
	</p>
    <p style="margin: 1;">
        Non-const static local variables should generally be avoided. If you do use them, ensure the variable never needs to be reset, and isn’t used to alter program flow.<br>
        通常应避免使用 non-const 静态局部变量。如果您确实使用它们，请确保该变量永远不需要重置，并且不用于更改程序流。
	</p>
</div>

## 7.12 — Scope, duration, and linkage summary

### Scope summary

about where can see, and declaration

**block (local) scope**: can only be accessed from the point of declaration until the end of the block.

**global scope**: can be accessed from the point of declaration until the end of the file.

### Duration summary

about when the entity created and destroyed

**automatic duration**: created at the point of definition, and destroyed when the block they are part of is exited.

**static duration**: created when the program begins and destroyed when the program ends.

**dynamic duration**: created and destroyed by programmer request.

### Linkage summary

**no linkage**: another declaration of the same identifier refers to a unique entity.

**internal linkage**: a declaration of the same identifier within the same translation unit refers to the same object or function.

**external linkage**: a declaration of the same identifier within the entire program refers to the same object or function.

**Variable summary table**

| Type                                     | Example                         | Scope  | Duration  | Linkage  | Notes                        |
| :--------------------------------------- | :------------------------------ | :----- | :-------- | :------- | :--------------------------- |
| Local variable                           | int x;                          | Block  | Automatic | None     |                              |
| Static local variable                    | static int s_x;                 | Block  | Static    | None     |                              |
| Dynamic local variable                   | int* x { new int{} };           | Block  | Dynamic   | None     |                              |
| Function parameter                       | void foo(int x)                 | Block  | Automatic | None     |                              |
| Internal non-const global variable       | static int g_x;                 | Global | Static    | Internal | Initialized or uninitialized |
| External non-const global variable       | int g_x;                        | Global | Static    | External | Initialized or uninitialized |
| Inline non-const global variable (C++17) | inline int g_x;                 | Global | Static    | External | Initialized or uninitialized |
| Internal constant global variable        | constexpr int g_x { 1 };        | Global | Static    | Internal | Must be initialized          |
| External constant global variable        | extern const int g_x { 1 };     | Global | Static    | External | Must be initialized          |
| Inline constant global variable (C++17)  | inline constexpr int g_x { 1 }; | Global | Static    | External | Must be initialized          |

**Forward declaration summary table**

| Type                                      | Example                   | Notes                                             |
| :---------------------------------------- | :------------------------ | :------------------------------------------------ |
| Function forward declaration              | void foo(int x);          | Prototype only, no function body                  |
| Non-constant variable forward declaration | extern int g_x;           | Must be uninitialized                             |
| Const variable forward declaration        | extern const int g_x;     | Must be uninitialized                             |
| Constexpr variable forward declaration    | extern constexpr int g_x; | Not allowed, constexpr cannot be forward declared |



| Specifier    | Meaning                                                      | Note                |
| :----------- | :----------------------------------------------------------- | :------------------ |
| extern       | static (or thread_local) storage duration and external linkage |                     |
| static       | static (or thread_local) storage duration and internal linkage |                     |
| thread_local | thread storage duration                                      |                     |
| mutable      | object allowed to be modified even if containing class is const |                     |
| auto         | automatic storage duration                                   | Deprecated in C++11 |
| register     | automatic storage duration and hint to the compiler to place in a register | Deprecated in C++17 |

### My summary

