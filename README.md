# Hydra
![download](https://user-images.githubusercontent.com/107733608/174929181-2b833d64-2109-4eb3-a67b-e257668856fa.jpg)

## Upcoming Features
1. Hydra is an abstract declaritive syntax on top of a JSON base layer
2. Hydra keeps itself pure, in the sense that it's an Abstract Syntax to keep itself language independent (and all the problems associated with). Language independence is important because if your language updates itself and Hydra no longer supports it, people can add that support without changing Hydra which would break other things downstream. 
3. Hydra is self-recognizing. This means that Hydra does not promote any underlying language through its choices. Self-recognition for a project like Hydra is important for various optimization reasons. Doing it any other way would lead to a more probable demise. 
4. Hydra's Plugin Architechture gives you the ability to add in Hercules-Constraints or other Plugins for whatever purpose
5. We currently are aiming to support python, javascript, and go translations.
