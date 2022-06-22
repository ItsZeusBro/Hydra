# Hydra
![download](https://user-images.githubusercontent.com/107733608/174929181-2b833d64-2109-4eb3-a67b-e257668856fa.jpg)

## First Release:

## Features
1. OOP
2. Type-Strict or Typless
3. Pass by reference or copy
4. call backs
5. higher order functions
6. variadic paramters
7. invariants and loop invariants
8. language support


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
