# Hydra 
- Aims to be a minimalistic Abstract Syntax that orchastrates other syntax plugins
- Uses a plugin/plugout architecture. Plugins extend Hydra's native features during Hydra Digestion. Plugouts are manifestions built using Hydra output.
- Tells us that: when we can code abstractly we should. The plugins aim to show us why. Overtime, this type of Abstract Syntax will allow us to do a lot more than meets the eye.
- Plugins are there to give context and opinion to your Abstract Syntax. This will allow Hydra to read like pseudo code or even natural language one day, and every term of art will have a context and opinion constrained by your plugins. In otherwords, some plugins can conflict with others. Better yet, other plugins add nuance in there own pipelines. That looks like the mythical Hydra when its done.

#### Plugins go into Hydra's belly (during digestion). 
![images](https://user-images.githubusercontent.com/107733608/175181009-7d7129b8-465b-46c9-853a-3f3d5d644cd0.jpg)
#### Plugouts are when Hydra surfaces one of its heads from beneath the sea. 


## somefile.hydra:
    //@ allows you to import other project files as dependencies and is reflected in code generating 
    //plugins output
    //The filename for a hydra file is the file name for your project and its associated code
    
    @/some/path/to/cool.hydra import CoolObject as Cool   
    {
          plugs:{

                jormungand:{
                    version: 3.0,
                    code:{

                    }

                }
                typhon:{
                    version: js6,
                    code:{

                    }

                }
          },

          //Native Hydra Objects
          hydra:{
                export objName1 as Obj1:{
                      type: class,
                      parent: Cool,
                      props:{
                        size: "10",
                        desc: "small thing"
                      },
                      methods:{
                        size: get_size(int, cool)

                      }

                },
                objName2:{
                      type: class,
                      props:{
                        size: "14",
                        desc: "strong thing"
                      },
                      methods:{
                        strength: get_strength(int, bool)
                      }
                },
                objName3:{
                      type: class,
                      props:{
                        size: "18",
                        desc: "weighty thing"
                      },
                      methods:{
                        get_weight: {
                            plugin: "Jormungand"
                            code:{
                                return self.size
                            }

                        }

                }
          }
    }
    
## Hydra Focuses on What your Building, Not How your Building it
- This is the basic power of declarations. They remain abstract, in as much as they only use a syntax that declares your objects. 
The "how" is the step by step sequence of operations needed to implement the "what". If we only focus on "what" we are building
for Hydra's purposes there is a good chance that a better tool will come along in the future that aids us in creating the "how".

    - For example, AI one day will be the best way to create what you describe. Therefore, Hydra wishes to remain pure to this objective
    to leverage future technologies while still remaining productive enough to be utilized heavily.

    - As AI changes how easily we build things at the "how" level, we can remain productive and needed at the "what" level with things like Hydra.
    Schema Interfacing is what remains stable to programmers long term. AI will train on this schema to give us what we want overtime.

## Hydra 0.1 Supported Features (eta: 18 months. In otherwords, go away and forget about this unless you want to help, and comeback when you remember):
1. plugin api
2. plugout api
3. interpreter (and sandbox websocket for text editor plugouts)
4. plug registry
5. basic plugs (Uranus, Jormungand, Hydrarchy, Orpheus, Hippocampus, and Hercules)
6. Comments are a native feature of Hydra files, but when they are exported to JSON with Hippocampus plugout they are put into a comment:"string" to not lose valuable info
7. Log Streams where each Hydra-Level plug has its own log stream and stack-trace.

## More on Plug Support:
To properly create a plug that also offers its own extending plugs, the plug your working on should utilize Hydra's Plug Library 


## Hydra 0.1 Keywords:
1. @
2. hydra
3. import
4. export
5. as
6. plugin
7. plugout
8. plugs
10. type
11. parent
12. class
13. props
14. methods
15. code

Please Join our Community and Help!
zeusofolympus1000@gmail.com
