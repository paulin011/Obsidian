testing every Path is impossible relevant errors only occur on exceptional nieche branches in the code

Types of Static Analysis 
[[Statistik/Softwaretechnik/Structural Analysis]]
[[Statistik/Softwaretechnik/Bug Finding]]



A static analysis tool analyzes the source code wether it satisfies a spesific property (Phi)

Examples of Static Analysis 
• P never accesses a variable that is null. • P never uses inputs that are not validated. 
• P never executes a division by zero.
• P will always close the DB connection. 
• P will always return a value.

Basic Concepts of Static Analysis Abstraction: The possible state space of a program (i.e., the possible values of its variables) is reduced.

Programs as structures: Code is represented by basic structures such as trees or graphs.

Static analysis systematically checks whether some property holds in an abstraction of the state space of a program

Summary
• Analysis of token streams (text) or code structures. 
• Suitable for finding patterns. 
• Checks local and structural properties that are independent from any execution path

Tools for Java 
Checkstyle: Checks coding style and conventions 
PMD: Identifies bad practices • Complicated statements • Inefficient code • … 
Findbugs: Specialized on bug patterns


2nd Summary 
• Static analysis: systematic automated analysis of the code, without executing the program 
• Structural analysis: looking for patterns in code 
• Control Flow Analysis: Analyze all possible paths (global property) 
• Data Flow Analysis: Analyzing possible (abstract) values of variables on all paths 
• All static analyses are unsound or incomplete or both
Page 22 to End
![[Statistik/Softwaretechnik/Lectures/19_QA+Testing IV.pdf]]