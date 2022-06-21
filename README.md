# Hydra
## Api Manifestations using Hydra's declaritive Invariants

![420px-Hercules_killing_the_hydra_headed_monster](https://user-images.githubusercontent.com/107733608/174702298-353afad3-96be-44c2-bf1a-b9f3cca65d54.jpg)


### Use this schema as an example for your hydra.json file to create your API function scaffolds, invariants, and documentation

    const regex = new RegExp('foo*');

    someFunction:{
        inv: (p1 >= 10) && (regex.test(p2))
        
        p1: {
            type: int
        }
        p2: {
            type: string
        } 
    
    }
    
 ## Scope
 ### Hydra 0.1 is not meant to produce a production ready documentation server
 It is meant to aid your efforts in building out your api's with a test driven approach. It's a developer tool to speed things up.
 Eventually it will go the distance and professionalize into a production ready documentation tool as well, but I don't know when.
    

