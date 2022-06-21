# Hydra
## Test Driven Function Framework using Hydra's Constraint Plugins

![420px-Hercules_killing_the_hydra_headed_monster](https://user-images.githubusercontent.com/107733608/174702298-353afad3-96be-44c2-bf1a-b9f3cca65d54.jpg)


## Hydra's Native Constraints use Boolean Invariants, Regex for Complex String Invariants, and Query Selectors for Nested Invariants 
### Input:
    {
        output: "some/file/somewhere"
        someFunction:{
            inv: "(pname1 >= 10) && (/ab+c/ == pname2)"
            params:{
                pname1: int,
                pname2: string
            }
        }
    }
    
 ### Output:
    function someFunction()
 
## Hydra uses it's own Native File Type to give more Semantical Meaning to an otherwise JSON like Syntax 


## Hydra's Plugin Architechture gives you the ability to add in OCL or other Constraint Driven Plugins
