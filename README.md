# Final Assembler Project (MAMAN 14)  
### The Open University of Israel

This project implements a **full multi-stage assembler in C**, developed as part of the **MAMAN 14** academic assignment in the Computer Science B.Sc. program at The Open University of Israel.

The assembler processes assembly source files, expands macros, performs a two-pass assembly process, and generates standard output files according to the project specification.

The project emphasizes **correctness, modular design, memory awareness**, and a clear **separation of responsibilities** between components.

---

## Features
- **Macro expansion** (pre-assembler stage)
- **Two-pass assembly**
  - First pass: symbol table creation and initial encoding
  - Second pass: address resolution and final encoding
- **Symbol table management**
- **Validation and detailed error handling**
- **Output file generation:**
  - Object file (`.ob`)
  - Entry symbols file (`.ent`)
  - External symbols file (`.ext`)
- Modular and maintainable C codebase

---

## Project Structure
- Pre-assembler (macro processing)
- First pass: symbol table creation and instruction/data counting
- Second pass: address resolution and final encoding
- Output generation

---

## Files Overview
- `assembler.c` – Main program and assembly flow control  
- `pre_assembler.c` – Macro expansion and preprocessing stage  
- `first_pass.c` – Symbol table creation and initial instruction encoding  
- `second_pass.c` – Address resolution and final instruction encoding  
- `symbol_table.c` – Symbol table management  
- `code_image.c` – Machine code image handling  
- `data_image.c` – Data image handling  
- `errors_handler.c` – Centralized error reporting system  
- `*.as` – Example assembly source input files  

---

## Build Instructions
Compile the project using the provided Makefile:

```bash
make
./assembler submit_test1.as submit_test2.as
