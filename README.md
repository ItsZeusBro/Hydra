# Hydra is a Computable Object Model Program (COMP) Semantic. (Not Syntax Dependent) 
### It's too abstract to call it a language, and its too concrete to call it a model.
What this means is that you can reach the goal of your app using a Computable Object Model Program through pure context associations at the model level and execute pure syncronous functions at the bottom that are totally independent of one another. 


Ultimately, the keystrokes that represent the Abstract COMP description take on the form of a concrete Hydra File for our purposes. Because Hydra's uses core COMP abstractions, it is able to Compute anything that is computable, using any Computational Paradigm needed for the Routines instructions. To see why COMP contexts are so powerful here look at the following diagram and it's six abstract components. They are generalizable that can represent every vertical level of your application.

## All Hydra Computables are made up of the following 6 core elements:
<img align="right" height="500" width="600" src="https://github.com/ItsZeusBro/Hydra/blob/99f5ff0bc33bbf89cf0b9451e02907c0ece4ce71/Computables.jpg">

0. Zeroware (Moira, Clotho, Lachesis, and Attropos)
1. Data
2. Data Structuring and Management
3. Routine
4. Machine
5. Result
6. Medium or Network



## Three levels of the COMP paradigm:

### Fully Syncronous
These Computable files have a set of instructions that are most primitive in your application. The primitive instructions are closely associated to the hardware. They utilize the hardware to ensure certain things get done in a very specific order. These COMP files are more about sequence than the abstract utilization of outside services, which are less understood. If you want to make sure something gets done in a very specific way, you don't use outside services. We call these Physical Computables.
### Syncronous and Asyncronous
These Computable files are hydrids. (Hybrids with a 'd'). They basically can touch down to perform syncronous behavior when they need to, or can be loose enough in sequence that sequence almost doesn't matter to the output. We call these Relative Computables.

### Fully Asyncronous
These Computable files have components that are so independent of one another, they can be visually represented with a mere association without direction. This is how your app level logic should be formulated at the very top. It's almost like brainstorming with abstract concepts that are actually very opinionated versions of those concepts under the hood.




### Does this abstraction help me build my app?
- That is exactly what Hydra is needed for. It aims to remove all of the complexity from implementation, and allow you to implement the design of your application and have more complex features and experiences. The long term vision of Hydra is to have a ecosystem of plugin components that interface with the 6 core abstractions. Ideal plugins only interface with a single abstraction, this is what we strive for, but is extremely difficult.


## More detail on what is in a Hydra File:
1. A Data Source
2. A Data Management Structure and Interface
3. An Abstract Routine Syntax (a bit like pseudo code)
4. A Reference to a Machine that is capable of executing it
5. A Result or "Artifact" Destination
6. A Reference to a Medium or Network to Send the results to

### It Should feel something like this (but is not limited to this because there are many ways to describe a Computable Object):
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
    
### There are no API's or Libraries in this abstraction. Every machine just depends on a type of input
- In otherwords, every Computable Machine expects a certain source of data, its type, and its structure.
- If this is not provided correctly into the machine, it is just ignored by the Computable. Please See Moira and Clotho. 
- This means error handling is premptive and seperate from the code that does something. 
- If your code recieves proper input, it should just execute without error (that is Moira), or not 
execute at all (that is Clotho) 
    - There is no in-between, because that is a security vulnerability. (That is Hydra)


### Benefits:
- Because of the small number of these core abstractions, you could have a visual 
syntax as opposed to a wordy subroutine. Or your words could easily be translated 
to a visual representation. 
- Even your Machine which executes your routine could be specifc to your routine. 
And if that routine were heavily used, you could end up having a result that produces 
an ASIC chip to compute the result faster.
- Production is just another computable environment, and running a Hydra file on your 
dev server should be no different than running it in the cloud or on some user device.
- Eventually user devices would not need a Machine to Compute anything. They would only 
display output and recieve input over a network.
- Your whole stack is recursive at the semantic level. This lends itself to functional 
programming paradigms.
- Every File is a Independent Computable Object which enforces Concurrency across 
your whole program where its needed most, at the top. 
- Architects can only worry about Orchastration. Programmers only need to look at the file 
they are programming. This seperation of concerns is optimal.
