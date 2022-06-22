# Hydra
## Test Driven Function Framework using Hydra's Constraint Plugins

![420px-Hercules_killing_the_hydra_headed_monster](https://user-images.githubusercontent.com/107733608/174702298-353afad3-96be-44c2-bf1a-b9f3cca65d54.jpg)


## Hydra's Native Type-Safe Constraints use Boolean Invariants, Regex for Complex String Invariants, and Query Selectors for Nested Invariants 
### Basic Example: (In a Hydra File, Hydra will use your invariants, in the order in which they are expressed [as a pipeline] and/or as nested flows for clarity)

    export SomeFunction = {
        output: "some/file/somewhere.js"
        someFunction:{
            inv: {
                invname1: "(pname1 >= 10)" ,
                invname2: "(/ab+c/ == pname2)",
                invname3: {
                    callBackFunction:{
                        inv:{
                            invname1: "(pname1 <= 100)"
                        }
                        params:{
                            pname1: int 
                        }
                    }
                 } //interpreted as a callback function
                 invname4: {
                       param4->select(i<100) //all items in the collection should be under 100
                       param4->select(param4.size<=10)
                 }
                 invname5: {
                    //loop through collection 1 and get half of the values that represent the smaller half
                    inv: {
                        check subcollection1 to make sure each element is greater than items in collection2
                    }
                 }
                  
            }
            params:{
                pname1: int,
                pname2: string,
                pname3: function,
                pname4: int_collection
                pname5: {
                    //This parameter is an Object
                    objpropname1: int_collection,
                    objpropname2: int_collection,
                    pfunc: function
                }
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
