# jlox

Java Lox implementation, following the excellent and beautifully crafted book [Crafting Interpreters](https://craftinginterpreters.com) by Robert Nystrom. 

## Usage

Compile first:

```bash
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