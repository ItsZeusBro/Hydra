# Hydra 
Hydra is a plugin architecture that generates all kinds of services needed for your application that compliment Hydra's native features.

Hydra aims to be a minimalistic Abstract Syntax that orchastrates other orchastrating Syntax plugins

Hydra tells us that: when we can code abstractly we should. The plugins aim to show us why. Overtime, this type of Abstract Syntax will allow us to do a lot more in the way of code generation, and probably a ton of other cool things we don't know about with fewer lines of code. Opportunities arise out of abstraction.

The plugins are there to give context and opinion to your Abstract Syntax. This will allow Hydra to read like pseudo code or even natural language one day, and every term of art will have a context and opinion informed by your plugins. In otherwords, some plugins conflict with others. Better yet, other plugins add nuance in there own pipelines. That looks like the mythical Hydra when its done.

Every plugin to Hydra evaluates its own syntax. The syntax is nested under the plugin name. The plugin will look for the name, evaluate the syntax and have an Hydra output: keyword with its stringified evaluation so that things like Hyrarchy can access the evaluations predictably.

![images](https://user-images.githubusercontent.com/107733608/175181009-7d7129b8-465b-46c9-853a-3f3d5d644cd0.jpg)


## somefile.hydra:
    //@ allows you to import other project files as dependencies and is reflected in code generating 
    //plugins output
    //The filename for a hydra file is the file name for your project and its associated code
    
    @/some/path/to/cool.hydra import CoolObject as Cool   
    {
      plugout:{
        //create a special purpose plugout here using Hydra's api to do some plugin development on the fly
        //and see how it interacts with the rest of your hydra files. Hydra's full api is directly exposed
        //to every hydra file by default, because the interpreter is what recognizes those calls.
        pythonv3:{
            //create your python based plugout for Hydra output evaluation (hydra's evalated JSON gets injested by 
            //your Python as the keyword "output")
            //this code block creates a python 3 file and imports the Hydra JSON output (called output) 
            //every chance Hydra gets for immediate feedback.
            //So do something with output.whatever in python
        }
      }
      plugin:{
        js6:{
            //create your javascript plugin here using Hydra plugin API. Pull in specific hydra functionality,
            //push out your plugin to Hydra's pipeline with associated priority
            //Then export it to the plug registry and pull it back in using Hydra Cli
            //all plugins pushed to the registry are hashed so that if you keep this code here, there are no
            //duplicate plugin collisions. Dont worry about empty spaces as they are all sanitized before being
            //hashed.
        }
      }
      //Native Hydra Objects
      Hydra:{
        export objName1 as Obj1:{
          type: "Class",
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
          type: "Class",
          props:{
            size: "14",
            desc: "strong thing"
          },
          methods:{
            strength: get_strength(int, bool)
          }
        },
        objName3:{
          type: "Class",
          language: "python v3.0"
          props:{
            size: "18",
            desc: "weighty thing"
          },
          methods:{
            get_weight: {
                //this feature gets ignored if you do not insert the associated language plugin
                //insert python code here that would go inside of func get_weight: in your python file
                return self.size
            }
            
          }
        }

      }
    }
    
## Hydra Focuses on What your Building, Not How your Building it
This is the basic power of declarations. They remain abstract, in as much as they only use a syntax that declares your objects. 
The "how" is the step by step sequence of operations needed to implement the "what". If we only focus on "what" we are building
for Hydra's purposes there is a good chance that a better tool will come along in the future that aids us in creating the "how".

For example, AI one day will be the best way to create what you describe. Therefore, Hydra wishes to remain pure to this objective
to leverage future technologies while still remaining productive enough to be utilized heavily.

As AI changes how easily we build things at the "how" level, we can remain productive and needed at the "what" level with things like Hydra.
Schema Interfacing is what remains stable to programmers long term. AI will train on this schema to give us what we want overtime.

## Hydra 0.1 Supported Features (eta: 6-12 months):
1. plugin api
2. plugout api
3. interpreter (and sandbox websocket for text editor plugouts)
4. plug registry
5. basic plugs (Uranus, Uranus-plugout, python-plugout, Hydrarchy, Orpheus)

Please Join our Community and Help!
zeusofolympus1000@gmail.com
