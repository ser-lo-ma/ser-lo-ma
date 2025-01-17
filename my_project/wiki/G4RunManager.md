The RunManager is the only mandatory manager object that the user must create. The EventManager, SteppingManager… are created and deleted manually by this main one. This manager controls the flow of a run including the set up of the simulation environment. When running [[Multithreading]] mode, the class should be substituted by G4MTRunManager

The Geant4RunManager has a few requirements:
- [[G4VUserDetectorConstruction]] (defines the geometry of the problem).
- [[Physics Lists]] derived from the class [[G4VUserPhysicsList]] (defines the particles and physics interactions). 
- An Action, derived from [[G4VUserActionInitialization]] containing **at least** a Primary generator derived from [[G4VUserPrimaryGeneratorAction]].
