# Hydra is a "Computable Oriented Design" Abstract Language Interpreter

## All Hydra Computables are made up of the following core elements:
<img align="right" height="500" width="600" src="https://github.com/ItsZeusBro/Hydra/blob/822433adcf0249ccff8811fe67f70eb1bb2c4f65/Computable2.jpg">

1. Data
2. Data Management
3. Routine
4. Machine
5. Result
6. Medium or Network



### Things to Note about the diagram:
- The Routine of a Computable can only be run on a Machine capable of carrying out its exact instructions in the routine's exact order.
    - So imagine in the example that the directed graph is capable of computing each step of the routine faithfully
- Lets assume that all Hydra Computables are sequential in the execution of their Routines
    - When Hydra speaks of concurrency, we call these Meta-Computables or Orchastrations (more on this later). But a Meta-Computable would not fall under a mere "Computable Element" for communication purposes.
    - A Meta-Computable uses the same 6 core principles as a normal computable. 

#### However, these should be thought of a bit differently for a Meta-Computable

1. Results of Computables
2. Storage of those Results
3. Routine based on those Results
4. A Machine capable of performing that Routine
5. A Composite Result
6. A place and method to send it to

##### Why do we not add "Display" to the list?
- This is an important question. The result is a form of display when it is shared! So Network encapsulates the logic of Display. To network is to communicate. That is a form of display, and we wont really delve too much into this distinction because it's not relevant here (even though it is at the end).
- Suffice it to say that even your display on your phone is just some "Result" of some "Computable" shared over a Medium


##### What does this mean for Hydra?
- It means, we can focus on these abstract elements for all Hydra Computables from a high level, and not worry about the implementations underneath it.
- What this means for our purposes is that we nail down a descriptive syntax that is very formal, and very easy to reason about. Each Hydra File is basically a composite of these 6 principles. Each Hydra File describes a Syncronous Routine. Even Meta-Computable Hydra Files. 
- Meta-Computable Hydra Files represent concurrency through syncronicity. And we will touch on this soon.




### Does this abstraction help me build my app?
- That is exactly what Hydra is needed for. It aims to remove all of the complexity from implementation, and allow you to implement the design of your application and have more complex features and experiences.


## Concurrency through Syncronicity:
Just because each Hydra File is Syncronous, and just because we only care about Hydra Files, does not mean that we can't compute things in parallel!
- Higher Order Hydra Files are the same as Lower order Hydra Files, with the exception that Higher Order ones reason about lower order ones. 
- While a Meta-Computable is kicking off a Hydra Process, that Hydra Computable is concurrently executed with the next Hydra Computable. 
- The results of those steps can be stored after their Machine's have closed off the Computable with a result. 
    - Evaluation of a step is not the same as steping into it and steping out of it.
        - So every abstract step can be "Completed" without being "Evaluated", all while remaining "Syncronous" within the Hydra File. 
        - So syncronicity for Hydra's purposes just means we "Complete" each step without looking underneath us until that is a part of the next step itself.
