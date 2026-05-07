# Slate Compiler

C code generation for the Slate language.

## Modules

- **codegen/** - Emits C from Slate AST
- **loader/** - Module loading and project config

## Pipeline

1. Parse source via `slate` library
2. Build Registry (functions, structs, enums)
3. Walk AST → emit C → compile with clang

## Entry Point

`compiler/source/lib.slt` - exports `codegen` and `loader` modules