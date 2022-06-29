# Hydra is a "Computable Object Model"

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

## What is in a Hydra File?
1. A Data Source
2. A Data Management Structure and Interface
3. An Abstract Routine Syntax (a bit like pseudo code)
4. A Reference to a Machine that is capable of executing it
5. A Result or "Artifact" Destination
6. A Reference to a Medium or Network to Send the results to

## It Should look something like this (but is not limited to this because there are many ways to describe a Computable Object):
    {
        source:{},
        structure:{},
        routine:{},
        machine: ref_to_some_machine,
        artifact: ref_to_some_structure_somewhere 
        display: ref_to_some_medium
    
    }
    
### Notes on High Level Scheme:
- The artifact destination in the way of some structure somewhere is not strictly necessary
    - For example, it could be stored in the local structure, some other hydra structure, or sent straight to some network or display (same thing)
- The routine can be written in a high level or low level language depending on plugin support
- The machine can be any computational machine, so long as it is able to complete the result
- The data source can be a simple path to a file, a socket, IPC, or a database handler

### Hydra has a Plugin Enabled Environment:
- Every single Hydra Computable Object utilizes its own plugins. If you want to Display the results of a State Machine for your Sub-Routine that searches a Red-Black Tree filled with nodes of strings coming from a file stream, on a simple web page; a single Hydra Computable Object should suffice.

### Benefits:
- Because of the small number of these core abstractions, you could have a visual syntax as opposed to a wordy subroutine. Or your words could easily be translated to a visual representation. 
- Even your Machine which executes your routine could be specifc to your routine. And if that routine were heavily used, it could end up having a plugin that produces an ASIC chip to compute the result.
