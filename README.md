# Hydra
## Test Driven Function Framework using Hydra's Constraint Plugins

![420px-Hercules_killing_the_hydra_headed_monster](https://user-images.githubusercontent.com/107733608/174702298-353afad3-96be-44c2-bf1a-b9f3cca65d54.jpg)


## Hydra's Native Constraints use Boolean Invariants, Regex for Complex String Invariants, and Query Selectors for Nested Invariants 
### Basic Example:
In a Hydra File, Hydra will use your invariants in the order in which they are expressed (as a pipeline)
    export SomeFunction = {
        output: "some/file/somewhere.js"
        someFunction:{
            inv: {
                invname1: "(pname1 >= 10) && (/ab+c/ == pname2)",
                invname2: 
            }
            params:{
                pname1: int,
                pname2: string
            }
        }
    }
    
 ### Output in some/file/somewhere.js:
 
    function someFunction(pname1, pname2) {
        assert(Hydra.Somefunction.inv)
        //code goes here
        assert(Hydra.Somefunction.inv)
        return
    }
 
 
## Hydra uses it's own Native File Type to give more Semantical Meaning to an otherwise JSON like Syntax 


## Hydra's Plugin Architechture gives you the ability to add in OCL or other Constraint Driven Plugins
