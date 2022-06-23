# Hydra 
Hydra is a plugin architecture that generates all kinds of services needed for your application that compliment Hydra's native features.

Hydra aims to be a minimalistic Abstract Syntax that orchastrates other orchastrating Syntax plugins

Hydra tells us that: when we can code abstractly we should. The plugins aim to show us why. Overtime, this type of Abstract Syntax will allow us to do a lot more in the way of code generation, and probably a ton of other cool things we don't know about with fewer lines of code. Opportunities arise out of abstraction.

The plugins are there to give context and opinion to your Abstract Syntax. This will allow Hydra to read like pseudo code or even natural language one day, and every term of art will have a context and opinion informed by your plugins. In otherwords, some plugins conflict with others. Better yet, other plugins add nuance in there own pipelines. That looks like the mythical Hydra when its done.

Every plugin to Hydra evaluates its own syntax. The syntax is nested under the plugin name. The plugin will look for the name, evaluate the syntax and have an Hydra output: keyword with its stringified evaluation so that things like Hyrarchy can access the evaluations predictably.

![images](https://user-images.githubusercontent.com/107733608/175181009-7d7129b8-465b-46c9-853a-3f3d5d644cd0.jpg)


## Basic Example:
    {
      //Native Hydra Objects
      Hydra:{
        objName1:{
          type: "Class",
          props:{
            size: "10",
            desc: "small thing"
          },
          methods:{
            size: get_size()

          }

        },
        objName2:{
          type: "Class",
          props:{
            size: "14",
            desc: "strong thing"
          },
          methods:{
            strength: get_strength()
          }
        },
        objName3:{
          type: "Class",
          props:{
            size: "18",
            desc: "weighty thing"
          },
          methods:{
            weight: get_weight()
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
