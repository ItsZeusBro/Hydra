# Hydra is a Computable Object Model Program (COMP) Semantic 
### It's too abstract to call it a pure functional language, and its too concrete to call it a pure visual model.
What this means is that you can reach the goal of your app using a Computable Object Model Program through pure context semantics at the top and execute pure functions at the bottom. 


Ultimately, the keystrokes that represent the Computable Object Model Program file take on the form of a concrete Hydra File for our purposes. Because Hydra's uses this context abstraction, it is able to Compute anything computable, using any Computational Paradigm needed for the Routine. To see why context is so powerful here look at the following diagram and it's six abstract components.

## All Hydra Computables are made up of the following core elements:
<img align="right" height="500" width="600" src="https://github.com/ItsZeusBro/Hydra/blob/99f5ff0bc33bbf89cf0b9451e02907c0ece4ce71/Computables.jpg">

1. Data
2. Data Structuring and Management
3. Routine
4. Machine
5. Result
6. Medium or Network



### Things to Note about the diagram:
- The Routine of a Computable can only be run on a Machine capable of carrying out its exact instructions in the routine's exact order.
    - So imagine in the example that the directed graph is capable of computing each step of the routine faithfully
- Lets assume that all Hydra Computables are sequential in the execution of their Routines. This means syntax initially takes precidence over semantic within the routines runtime. Semantic represents full evaluation of the underlying step, but this would not leverage concurrency. So The Hydra Machine Abstraction does not use this type of life-cycle for the evaluation of a Hydra File
- When Hydra speaks of concurrency, we call these Relative-Computables or Orchastrations (more on this later). 
    - They are not meant to be rigorously understood, rather, they describe loosely associated parts at the highest levels of your app moving in some sequence where sequence doesnt even matter that much. 
    - It looks similar to a brain storming session on a whiteboard, meaning, relating large concepts together in this thing called your app. Where the lines between the Computable Objects have no sequential semantic. 
    

## The six core abstractions should be thought of a bit differently for Relative Computables

1. Results as ***Source Data*** 
2. ***Structure and Management*** of those Results
3. A ***Routine*** associated on those Results     
4. A ***Machine*** capable of performing that Routine.
5. A Composite ***Result***
6. A place and method to send it to

### Notes on Relative Computables
- To understand the job of Relative Computables we need to understand the extremes. The absolute top layer of your application code (root or app level), and one of the absolute bottoms that knows nothing about anything other than their specific job for which they have everything they need. (leaf or pure functional level) 
    - In otherwords the entire application in the Computable Object Model is just a tree, with pure functions at the bottom, and pure associations at the top
- A Relative Computable is a mix of both. It translates the top to the bottom and the bottom to the top. The less of this code we have, the better. But it is still needed. 


## The six core abstractions should be thought of differently for the highest level called "App-Computables":
1. These are the results of all of your lower level Computables, whose results look more and more involved the more you go down. The App Level is the queitest place in your application with the slowest moving parts. Results bubbling up the stack are mere happy thoughts if things are going well, or just silence.
2. ***Structure and Management*** of those results are also less involved at the app level in as much
The ***Routine*** matters less the higher you go, but you still need one to get things done
- Moira aims to service the high level ***Machine*** Abstractions and the Low Level Machine

##### Why do we not add "Display" to the list?
- This is an important question. The result is a form of display when it is shared! So Network encapsulates the logic of Display. To network is to communicate. That is a form of display, and we wont really delve too much into this distinction because it's not relevant here (even though it is at the end).
- Suffice it to say that even your display on your phone is just some "Result" of some "Computable" shared over a Medium


##### What does this mean for Hydra?
- It means, we can focus on these abstract elements for all Hydra Computables from a high level, and not worry about the implementations underneath it.
- What this means for our purposes is that we nail down a descriptive syntax that is very formal, and very easy to reason about. Each Hydra File is basically a composite of these 6 principles. Each Hydra File describes a Syncronous Routine. Even Relative-Computable Hydra Files. 
- Relative-Computable Hydra Files represent concurrency through syncronicity. And we will touch on this soon.




### Does this abstraction help me build my app?
- That is exactly what Hydra is needed for. It aims to remove all of the complexity from implementation, and allow you to implement the design of your application and have more complex features and experiences.


## Concurrency through Syncronicity:
Just because each Hydra File is Syncronous, and just because we only care about Hydra Files, does not mean that we can't compute things in parallel!
- Higher Order Hydra Files are the same as Lower order Hydra Files, with the exception that Higher Order ones reason about lower order ones. 
- While a Relative-Computable is kicking off a Hydra Process, that Hydra Computable is concurrently executed with the next Hydra Computable. 
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
        source:{
            //Things related to a source context:
            1. Data Typing
            2. Comparators
            3. Type Casting
            4. Type Inference
            5. Input operations and interfaces
            6. Simple Data Structs (Nodes belonging to a graph)
            7. Data Macros
            8. Databases
        },
        structure:{
            //Things related to Data Structure Context
            1. Databases
            2. Searching
            3. Sorting
            4. Inserting, Modifying, and Deleting
            5. Stacks and Queues
            6. Trees
            7. Structure Optimization
        },
        routine:{
            //Things related to Routine Context
            1. Routine Syntax
            2. Callable Apis
            3. Object Oriented Programming (even though Hydra does not 
            levearage the full power of OOP, because its a different paradigm. 
            Everything of relevance is a computer, not a mere object in 
            Computer Object Modeling.
            4. Interpreters
            5. Compilers
            6. ABI's
            7. Assembly and ASIC's
        },
        machine: {
            //Things related to Machine Context
            1. Computational Paradigms (State Machines, General Purpose Machines, 
            Specific Purpose Machines)
            2. Other Computable Object Models (Hydra Files) are an instance of 
            a Specific Purpose Machine
            3. Machine Configuration and Initial State
        },
        artifact: {
            //Things related to the Result (Artifact) context
            1. The result of a Machine's syncronous routine. Every machine at its 
            most abstract and highest level (unless its statistical) uses syncronicity. 
            The result is therefore pseudo-deterministic. Its high level steps are
            determined, its low level effects are more impacted by non-deterministic 
            behavior as a result of timing issues between concurrent processes, and 
            user input.
            2. Results are closely related to display because they represent the final 
            state of a machine. The output is returned, and that is why the two concepts 
            are so closely associated. When choosing a context, pay close attention to 
            these differences.
        
        }, 
        display: {
            //Things related to the Display context
            1. All results of the machine are returned from the machine as output. 
            This return process exposes the result to some consumer. This is considered 
            "display". Display can be an elaborate and complex process (involving 
            animations, etc) for the output of a machine or app, as the app's utility 
            and productivity is closely associated with its display.
        }
    
    }
    
### Notes on High Level Scheme:
- The artifact destination in the way of some structure somewhere is not strictly necessary
    - For example, it could be stored in the local structure, some other hydra structure, 
    or sent straight to some network or display (same thing)
- The routine can be written in a high level or low level language depending on plugin support
- The machine can be any computational machine, so long as it is able to complete the result
- The data source can be a simple path to a file, a socket, IPC, or a database handler
- If a plugin acts as a Machine, it is also a Hydra Computable Template File that can be 
tailored to your app

### Hydra has a Plugin Enabled Environment:
- Every single Hydra Computable Object utilizes its own plugins. If you want to Display the 
results of a State Machine for your Sub-Routine that searches a Red-Black Tree filled with 
nodes of strings coming from a file stream, on a simple web page; a single Hydra Computable
Object should suffice.

### Benefits:
- Because of the small number of these core abstractions, you could have a visual 
syntax as opposed to a wordy subroutine. Or your words could easily be translated 
to a visual representation. 
- Even your Machine which executes your routine could be specifc to your routine. 
And if that routine were heavily used, it could end up having a plugin that produces 
an ASIC chip to compute the result.
- Production is just another computable environment, and running a Hydra file on your 
dev server should be no different than running it in the cloud or on some user device.
- Eventually user devices would not need a Machine to Compute anything. They would only 
display output and recieve input over a network.
- Your whole stack is recursive at the file level. This lends itself to functional 
programming paradigms as opposed to functional languages.
- Every File is a Computable Object not a Class, which enforces Concurrency across 
your whole program.
- Every File is a Computer. Your most Abstract Orchastration File is your App's Computer 
that is specific to your App, not the Platform it runs on.
- Architects can worry about Orchastration. Programmers only need to look at the file 
they are programming. This seperation of concerns is optimal.
