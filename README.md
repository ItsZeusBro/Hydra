# Hydra
## Test Driven Function Framework using Hydra's Constraint Plugins (Still designing the interface, back-off!)

![420px-Hercules_killing_the_hydra_headed_monster](https://user-images.githubusercontent.com/107733608/174702298-353afad3-96be-44c2-bf1a-b9f3cca65d54.jpg)


## Hydra's Native Constraints use Boolean Invariants, Regex for Complex String Invariants, and Query Selectors for piping Invariants 
### Basic Example:
    someFunc = {
        out: "some/file/somewhere.js"
        inv: {
            inv1: "(p1 >= 10)" ,
            inv2: "(/ab+c/ == p2)",
            inv3: p4->(i<100)->(p4.size<=10)
            inv4: (objP1.disjointset(objP2).difference(objP3))->(i<100)
        }
        params:{
            p1: <int>,
            p2: <string>,
            p3: <function>,
            p4: <intCollection>
            p5: {
                //This parameter is an Object
                objP1: <int_collection>,
                objP2: <int_collection>,
                objP3: <int_collection>,
                pFunc: <function>
            }
        }
    }

Hydra takes this assignment and creates a Hydra Object called someFunc. This object both generates code, and is callable from supported languages 
    
 ### Output in some/file/somewhere.js:
 

 
## Hydra uses it's own Native File Type to give more Semantical Meaning to an otherwise JSON like Syntax 


## Hydra's Plugin Architechture gives you the ability to add in OCL or other Constraint Driven Plugins

## Hydra creates the test files with functions that are bound to your implementation, and can be included as a build step in pipeline
