Lifecycle of a Program
In Java, the program lifecycle consists of several distinct phases that work together to execute code. The process begins with developers writing Java source code in .java files using an IDE or text editor. This code is then compiled by the Java compiler (javac) into bytecode stored in .class files, with syntax and type checking performed during compilation. When the program runs, the Java Virtual Machine (JVM) loads these compiled class files into memory through a process involving loading of binary data, linking for verification and preparation, and initialization of class elements. The JVM then verifies the bytecode's security compliance, performs Just-In-Time (JIT) compilation to translate bytecode into native machine code for better performance, and executes the program instructions while managing system resources. Throughout execution, the JVM handles garbage collection by reclaiming memory from unused objects, and finally releases all resources upon program termination. This architecture enables Java's "write once, run anywhere" capability since the bytecode can execute on any device with a compatible JVM.

☕ The Java Life Cycle: From Code to Execution
The journey of a Java program follows the "Write Once, Run Anywhere" (WORA) philosophy, facilitated by the Java Virtual Machine (JVM).
1. Source Code Creation
The process begins with the developer writing human-readable code in a text editor or IDE (like IntelliJ IDEA or Eclipse).
File Extension: The source file must be saved with a .java extension (e.g., Main.java).
2. Compilation (Build Time)
The Java Compiler (javac), included in the JDK, translates the source code into an intermediate format.
Output: A .class file containing Bytecode.
Platform Independence: This bytecode is not specific to any OS, allowing it to run on any device with a compatible JVM.
3. Class Loading & Linking
When the program is run (using the java command), the JVM prepares the code:
Loading: The ClassLoader brings the .class files into memory.
Verification: The Bytecode Verifier checks for security violations or illegal instructions.
Linking: The JVM resolves symbolic references and prepares static variables.
4. Execution (Run Time)
The JVM’s Execution Engine converts the platform-neutral bytecode into machine-specific instructions (binary) for the local CPU.
Interpreter: Reads and executes bytecode line-by-line for a quick start.
Just-In-Time (JIT) Compiler: Identifies "hot" (frequently used) code and compiles it into native machine code to significantly boost performance.
5. Garbage Collection & Termination
Memory Management: The Garbage Collector automatically identifies and removes objects no longer in use to free up heap memory.
Exit: The program terminates once all non-daemon threads finish or a manual exit command (like System.exit()) is called.
