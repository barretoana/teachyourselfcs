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
