# jlox

Java Lox implementation, following the excellent and beautifully crafted book [Crafting Interpreters](https://craftinginterpreters.com) by Robert Nystrom. 

## Usage

Generate the AST and compile first:

```bash
javac com/craftinginterpreters/tool/GenerateAst.java
java com/craftinginterpreters/tool/GenerateAst com/craftinginterpreters/lox
javac com/craftinginterpreters/lox/*.java
```

Then, to use the interactive interpreter:

```bash
java com.craftinginterpreters.lox.Lox
```

(The interactive interpreter doesn't allow code blocks over multiple lines.)

To run script files:

```bash
java com.craftinginterpreters.lox.Lox tests/hello-world.lox
```

## Gotcha's 

I never took out the AST printer functionality from one of the early chapters. This required me as a result to add a printer method each time I added to the AST in subsequent chapters. For that I simply looked up the reference implementation at https://github.com/munificent/craftinginterpreters/.