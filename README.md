# Hydra (Abstract Syntax for Business Logic that Descends into your Native Language)
![download](https://user-images.githubusercontent.com/107733608/174929181-2b833d64-2109-4eb3-a67b-e257668856fa.jpg)
## Background Info:
Abstract Syntax is a great tool for architechts to instantiate projects with all of their associated: 
1. Concrete Dependencies
2. Functions
3. Classes with associated properties and methods
4. OOP Inheritance
5. Parameters and their associated types
6. Invariants and Looping Invariants
7. Callback functions
8. State Machine Flow (Initial State and Transition Functions) 
9. Exception Handling
10. REST Api's
11. Network Protocols
12. Abstract Modules (reference and link smaller Abstract Modules to create monolithic executable Abstract Syntax Files)
13. Abstract Database Schema

All in a single shcema, Hydra aspires to be a real declaritive sea monster! But thats not all! Hydra allows you to descend into writing functions in a language of your choice within a familiar Javascript Object or JSON notation.



## Hydra Main Features
1. Generate Diagrams using ascii art all in Javascript Objects or JSON that is bound to your Object Declarations (Using Uranus Plugin)
2. Generate Source Code Files with complete classes, functions, in the language of your choice (Using Language Plugins)
3. Generate Documentation tied to your Abstract Syntax filled with commentary (Using Hydrarchy Plugin)

Why ascii art for diagrams? Because it allows us to use diagram according to any standard

## Additional things
1. Hydra is an abstract declaritive syntax on top of a JSON or JsObject base layer. In otherwords its all JSON (or Javascript), but Hydra reads it differently to do powerful things
2. Hydra keeps itself pure, in the sense that it's an Abstract Syntax to keep itself language independent (and all the problems associated with). 
    - Language independence is important because if your language updates itself and Hydra no longer supports it, people can add that support without changing Hydra which would break other things downstream.
    - HOWEVER: This does not mean you can't write code in your favorite language nested in between more abstract language independent declarations 
4. Hydra is self-recognizing. 
    - This means that Hydra does not promote any underlying language through its choices. 
    - Self-recognition for a project like Hydra is important for various optimization reasons. 
    - Doing it any other way would lead to an eventual demise 

5. Hydra uses a standard interpreter for all Abstract Syntax
7.  Hydra's Plugin Architechture gives you the ability to add in cool plugins like Hercules-Constraints or other Plugins for whatever purpose
8. We currently are aiming to support python, javascript, and go scaffolding. Various others will need help from the community

## Some Cool things you can Build with Hydra!
1. A client in Javascript and server in Golang all connected with network code
2. State Machine Diagrams with their associated code
3. REST Api's
4. Almost anything having to do with business logic

## Basic Rules
1. Everything is an Object
2. Every Object has a name associated with it in a Hydra Context
3. Some Objects are Classes, others are Functions, Abstract Data Types, and Literals
4. Classes all use the specific keywords props and methods
5. Methods have function names and blocks that contain real code blocks (in your favorite language) and the keyword that specifies the language

Everything else is plugged into Hydra, including but not limited to: 
1. Abstract Diagram Syntax and Visuals associated with your Object Names (Uranus)
2. Testing Constraints hooked to all functions and methods that are hidden from your Hydra files (Hercules)
3. Microservice Orchastration with REST Api and other forms of communication (Lachesis)
4. AI Pipelines assistance with abstract directives (Odin and Cronus) 
5. CI/CD integration (Hermes) 
6. Documentation (Hydrarchy)
7. Persistence Orchastration (Homer) 
8. State Machines (Moira)
9. Identity/Permission services (Olympus)

Hydra Plugins work with their own Abstract Syntaxes and are evaluated by the plugin which is orchastrated by Hydra when necessary

### Hydra Workflow:
Hydra is in sync with your codebase because it generates that codebase and all of its associated files from Abstract Syntax; including classes, functions, etc. 
This means the following:
1. When you update function code in a Hydra file, it is reflected in your actual source file, and viceversa (IDE's should tuck this hydra low level code away unless you want to drill into on a case by case basis. This is to emphasize the Abstract Syntax features and plugins)
2. Hydra's interpreter makes real-time changes to your local repository
3. Hydra has plugin build scripts that run the code you change but only where you change it (and what it effects) to let you know in real time how your code performs (and its associated output logs [plugin enabled]). This feature should not work without a plugin, because each language and build context is highly specific.
