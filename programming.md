# Structure and Interpretation of Computer Programs 
[Available online here](https://mitpress.mit.edu/sites/default/files/sicp/full-text/book/book.html)

> *“If art interprets our dreams, the computer executes them in the guise of programs.”*

## About 

This document is for note-taking and expanding on the main subject of the book. The organization follows the chapters. 

## Notes 

### Foreword 

**Three foci(or focuses, if you prefer)**: 
- The Human Mind 
- Collections of Computer Programs
- The Computer

 » Develop an arsenal of standard program structures, and learn to combine them into more complex ones;  
 
 » The understanding of powerful organization techniques aids that ^;  
 
 » Programmers should ask themselves "TOWARD WHAT END?" frequently;   

» **Algorithms**: precise mathematical function;  
    └ Optimal behavior: time & data storage requirements;  
    └ It's the responsibility of the programmer to estimate and try to improve their performance;   

### Preface 

» A computer language is not just a way of getting a computer to perform operations but rather that is a novel formal medium for expressing ideas about methodology;  

» **Programs must be written for people to read and only incidentally for machines to execute**;   

» This books adresses the techniques used to control intellectual complexity of large software systems;  

» The computer revolution is a revolution in the way we **think** and in the way we **express** what we think;  

» **Procedutal Epistemology**: The study of the structure of knowledge from an imperative point of view.   
└ = a framework of **HOW TO**;  
└ "becoming aware of our nuanced logical and problem-solving thought processes and reducing them to elegant algorithms" [[source]](https://boundlessrationality.wordpress.com/2011/07/23/computer-science-and-philosophy-procedural-epistemology/
)

## Chapter 1: Building Abstractions with Procedures 

» Computational process: 
  - Manipulates data;
  - The evolution of one is directed by a program;
  
» People create programsto direct processes;  

» Lisp: invented in the late 50s, based on a paper about Recursive Functions;  
└ Evolved to a family of dialects, Scheme is the on used in the book;  
└ Why? Unique features tha make it a good language for learning, Procedures (description of processes) and It's fun!  

### 1.1 The elements of Programming 

» A programming language mechanisms:  
└ Primitive expression: represent the simplest entities;  
└ Means of combination: compound elements are built from simpler ones;  
└ Means of abstraction: compound elements can be named and manipulated as units; 

» **Procedures**: descriptions of rules for manipulating data;  
» **Data**: *stuff* we want to manipulate; 

### 1.1.1 Expressions 

» An expression is a combination of one or more constants, variables, operators and functions that the programming language interprets and computes to produce another value ([Wikipedia](https://en.wikipedia.org/wiki/Expression_(computer_science))).  

» **Evaluation**: this process for mathematical expressions ^   

» **Prefix Notation**    
```
(- 13 1)
```  
Combination:  (- 13 1)   
Operator: -   
Operands: 13 1  
Arguments: 13, 1  
└ Advantages: less ambiguity, allows straight foward nesting;   
└ Pretty printing (aka indentation) can help with legibility;   

» The Interpreer runs a read-eval-print loop;   

### 1.1.2 Naming the Environment   

» **Variables**   
```
(define size 2)
``` 
Name-Object pair: size, 2   
└ Simplest means of abstraction   

» Complex programs are constructed by building step by step computational objects of increasing complexity;    

» **Environment**: memory that keeps track o the name-object pairs;    

### 1.1.3 Evaluating Combinations  

» **Evaluation Process**:   
1. Evaluate the subexpressions of the combination   
2. Apply the procedure to the arguments    

└ recursive in nature    

» Tree accumulation: filter values upwards;   

» Special Forms: exceptions of the general evaluation rule (such as define);   

### 1.1.4 Compund Procedures 

» **Procedure definitions**: a compound operation can be given a name and then refered to as a unit;  
```
(define (square x) (* x x))
```  

### 1.1.5 The Substitution Model for Procedure Application

» The interpreter evaluates the elements of the combination and applier the procedure to the arguments;   

» **Substitution Model**: The process of evaluating the body of the procedure with the parameter replaced by the corresponding argument (not how typical interpreters work);   

» **Normal Order Evalutaion**: fully expand the expression then reduce;   

» **Applicative Order evaluation**: evaluatee the arguments and then apply;   
└ Used by Lisp's interpreter because of efficiency and normal order is more complicated; 

### 1.1.6 Conditional Expressions and Predicates

» **Case Analysis**: perform different operations depending on the result of a test. 
``` 
(cond (p1 e1)
      (p2 e2) 
      ...
      (pn en))
          
          
 (if <predicate> <consequent> <alternative>)
 ```

Predicate: the value to be interpreted as true or false; 
Expression or Consequent: if the predicate is true, returns the value of the expression; 
Alternative: if the predicate is false, returns the alternative; 

» **Logic composition operations**: 
└ AND: true when all true;   
└ OR: true when at least one true;   
└ NOT: negates the value;   

```
(and <e1> ... <en>) 
(or <e1> <e2> ... <en>)
(not <e>) 
```






















