# FunctionCraft Compiler Projects

A Java/ANTLR coursework collection for the FunctionCraft language, covering parsing, abstract syntax trees, semantic analysis, and JVM-oriented code generation.

## Project map

| Directory | Focus |
| --- | --- |
| `CA1/` | Grammar, generated parsers, and sample programs |
| `CA3/` | Type checking and diagnostic reporting |
| `CA4/` | Type checking and Jasmin-based code generation |

The repository retains the original coursework layout, including nested source directories and generated files.

## Explore and run

Use a JDK and the ANTLR 4.13.1 JAR bundled with the relevant assignment. There is no shared Maven or Gradle build at the root.

1. Open one assignment in a Java IDE.
2. Mark its `src` directory as a source root and add its ANTLR JAR to the classpath.
3. Generate the grammar into the `parsers` package if the generated parser classes are missing.
4. Run `main.FunctionCraft` from that assignment's working directory.

For CA3, pass a FunctionCraft file path as the first argument. The entry point writes diagnostics to `samples/out11.txt`.

CA4 currently reads `samples/sample1.fl`, writes type-checking diagnostics under `samples/`, and assembles output through the bundled Jasmin JAR. Its process invocation and paths may require adjustments on a different operating system. Review `CA4/src/main/FunctionCraft.java` before running it.

## Validation

The assignment sample programs and expected-output files provide the existing checks. No reproducible command-line build or complete automated test suite is documented for this snapshot.

## Project credits

This is Sobhan Alaeddini's portfolio fork of [AryanBastany/Programming-Languages-and-Compiler-Course-Projects](https://github.com/AryanBastany/Programming-Languages-and-Compiler-Course-Projects). The project was developed collaboratively; the upstream repository and Git history retain the original contributor credits. Documentation in this fork is maintained independently.
