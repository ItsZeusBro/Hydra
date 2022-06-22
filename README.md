# Hydra
![download](https://user-images.githubusercontent.com/107733608/174929181-2b833d64-2109-4eb3-a67b-e257668856fa.jpg)
## Background Info:
Abstract Syntax is a great tool for architechts to instantiate projects with all of their associated: 
1. Dependencies
2. Functions
3. Classes with associated properties and methods
4. OOP Inheritance
5. Parameters and their associated types
6. Invariants and Looping Invariants
7. Callback functions
8. State Machine Flow (Initial State and Transition Functions) 
## First Release:

## Hydra Features
1. Hydra offers all of the declaritive features of an Abstract Syntax that are listed above
2. Hydra offers an abstract syntax (that is basically JSON) that is interpreted differently than the underlying JSON. This saves time initiating a project, especially if you use Hydrarchy Documentation, and Hydra plugins like Hercules that try to gain finer grain control within the Hydra Pipeline
3. The interpreter makes its run in layers which enables the pipeline to have semantical value in the future. (we don't know what that might be, we just think it might open things up later). It also helps us wrap our head around the plugins and how they interact with Hydra.


## Additional things
1. Hydra is an abstract declaritive syntax on top of a JSON base layer. In otherwords its all JSON, but Hydra reads it differently than JSON does
2. Hydra keeps itself pure, in the sense that it's an Abstract Syntax to keep itself language independent (and all the problems associated with). 
    - Language independence is important because if your language updates itself and Hydra no longer supports it, people can add that support without changing Hydra which would break other things downstream. 
4. Hydra is self-recognizing. 
    - This means that Hydra does not promote any underlying language through its choices. 
    - Self-recognition for a project like Hydra is important for various optimization reasons. 
    - Doing it any other way would lead to a more probable demise. 
6. Hydra's Plugin Architechture gives you the ability to add in Hercules-Constraints or other Plugins for whatever purpose
7. We currently are aiming to support python, javascript, and go translations. Various others will need help from the community
