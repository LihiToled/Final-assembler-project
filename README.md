**Final Assembler Project (MAMAN 14) - The Open University of Israel** 

This project implements a full multi-stage assembler in C, developed as part of an academic assignment (MAMAN 14).
The assembler processes assembly source files, expands macros, performs a two-pass assembly process, and generates standard output files.

The project emphasizes correctness, modular design, memory awareness, and a clear separation of responsibilities between components.

**Features**
* Macro expansion (pre-assembler stage)
* Two-pass assembly (first and second pass)
* Symbol table management
* Validation and detailed error handling
* Output file generation:

  * Object file (`.ob`)
  * Entry symbols file (`.ent`)
  * External symbols file (`.ext`)
* Modular and maintainable C codebase

**Project Structure
**
* Pre-assembler (macro processing)
* First pass: symbol table creation and initial encoding
* Second pass: address resolution and final encoding
* Output generation

**Build Instructions**
Compile the project using:
```bash
make
```

**Usage**
Run the assembler with one or more assembly source files:

```bash
./assembler file1.as file2.as
```

**Technologies**
* C (ANSI C90)
* Makefile
* Linux / Unix development environment
* Modular design principles

Notes
The project was developed with strict compilation flags and careful memory management, with a strong focus on code readability and maintainability.

**Authors**
Lihi Toledano & Yuval Tal
Computer Science B.Sc. students
