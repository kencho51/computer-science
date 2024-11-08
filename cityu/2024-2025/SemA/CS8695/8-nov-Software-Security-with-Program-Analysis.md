# Software Security with Program Analysis: The New Era
HUANG, Heqing
https://5hadowblad3.github.io/

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

### How does Symbolic execution find bugs?

### Concolic Execution
Concolic = concrete + symbolic

### Hybrid concolic testing
Concolic + random testing

### Explosive software code size
  - Linux kernal: 17 million lines
  - Chrome: 78 million lines
  - Tesla Model S: 100 million lines 

### NP-HARD problems

### key insight: minimize the search space with approximation

### State of the art solution: Fuzz testing

### What is fuzzing?

### Precise and Effectiveness

### Problems1: Existing mechanisms are not incremental
Random mutation is fast but not precise
Constraint solving is expensive, low efficiency

### 1st contribution
Interpret the input search space


### Problem II: Infeasible path explosion

### 2nd contribution
Directed fuzzing with provable path pruning
How to infer the precondition precisely which allows filtering more irrelevant paths?
Solution: Interval anstraction with precision enhancement

### Tremendous targets exist in software industry nowadays
  - bug discovery
  - bug location
  - bug fixing

### Problem III: existing works do not distinguish the synergy among targets

Differentiate bug correlations through reducing the seach space

Solution: concurrently fuzz multiple 


tools:
pangolin
beacon
titan

Summary: make fuzzing more efficient

Future goal: effectively fuzz all the things

Identifying bugs are difficult/challenging

Insight: Search space could be represented with rich semantics




