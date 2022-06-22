# Hydra
## Test Driven Function Framework using Hydra's Constraint Plugins (Still designing the interface, back-off!)

![420px-Hercules_killing_the_hydra_headed_monster](https://user-images.githubusercontent.com/107733608/174702298-353afad3-96be-44c2-bf1a-b9f3cca65d54.jpg)


## Hydra's Native Constraints use Boolean Invariants, Regex for Complex String Invariants, and Query Selectors for piping Invariants 
### Basic Example:
// "=" operator is used to assign a Hydra scheme to a Hydra object that is exposed to supported languages
    SomeFunction = {
        output: "some/file/somewhere.js"
        someFunction:{
            inv: {
                inv1: "(pname1 >= 10)" ,
                inv2: "(/ab+c/ == pname2)",
                inv3: p4->(i<100)->(p4.size<=10)
                inv4: (objp1.disjointset(objp2).difference(objp3))->(i<100)
            }
            params:{
                p1: int,
                p2: string,
                p3: function,
                p4: int_collection
                p5: {
                    //This parameter is an Object
                    objp1: int_collection,
                    objp2: int_collection,
                    objp3: int_collection,
                    pfunc: function
                }
            }
        }
    }
    
 ### Output in some/file/somewhere.js:
 

 
## Hydra uses it's own Native File Type to give more Semantical Meaning to an otherwise JSON like Syntax 


## Hydra's Plugin Architechture gives you the ability to add in OCL or other Constraint Driven Plugins
