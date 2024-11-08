# Software Security with Program Analysis: The New Era

Is the system doing what it is intended to do?
  - How to find vulnerable programme behaviours?
  - How to identify behaviours are indeed vulnerable?

Unexpected input may trigger dangerous output!


### Generate test case to validate the existence of vulnerabilities
Control flow graph

Executed path

Satisfiability Module Theories (SMT) Problem

First-order formula -> SMT solver -> Satisfy/UnSatisfy
example:
  - x*x = 3 UNSAT if x is integer
  - x*x = 3 SAT if x is real

### Symbolic Execution
![symbolic-execution](./symbolic-execution.jpeg)

### How does Symbolic execution find bugs?

### Concolic Execution
Concolic = concrete + symbolic
