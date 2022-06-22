# Hydra
## Abstract Test Driven Function Framework using Hydra's Native Constraints and Constraint Plugins
![420px-Hercules_killing_the_hydra_headed_monster](https://user-images.githubusercontent.com/107733608/174702298-353afad3-96be-44c2-bf1a-b9f3cca65d54.jpg)


## Hydra's Native Constraints use Boolean Invariants, Regex for Complex String Invariants, and Query Selectors for piping Invariants 
### Basic Example:
    someFunc = {
        out: "some/file/someWhere.js" //you can use .py and Hydra will generate python files
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

### Additional Info:
1. Hydra takes the assignment to someFunc and creates a Hydra Object called someFunc. This object generates test code, and is also callable from supported languages 
2. Hydra uses it's own Native File Type to give more Semantical Meaning to an otherwise JSON like Syntax 
3. Hydra keeps itself pure, in the sense that it's an Abstract Syntax to keep itself language independent (and all the problems associated with) and self-recognizing. Language independence is important because if your language updates itself and Hydra no longer supports it, people can add that support without changing Hydra which would break other things downstream. Self-recognition for a project like Hydra is important for various optimization reasons. (Lending itself to specific paradigmns takes away from Hydra) 

## Future Releases:
1. Hydra's Plugin Architechture gives you the ability to add in OCL or other Constraint Driven Plugins
2. python and golang support
