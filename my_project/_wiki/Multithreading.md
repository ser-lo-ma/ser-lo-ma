---
layout: wiki
title: Multithreading
---
Geant4 parallelism works with a _master-worker_ model, where a main thread is created that controls the simulation while a number of worker threads simulate the individual events. This is implemented by G4MTRunManager (derived from [[G4RunManager]]). The master thread owns the geometry and physics, but each thread contains a copy of the less memory intensive classes. If working on multithreaded mode, it is important to **merge** the output of all different threads. 
#### Sources:
- [Geant4 Book for Toolkit Developers](https://geant4-userdoc.web.cern.ch/UsersGuides/ForToolkitDeveloper/fo/BookForToolkitDevelopers.pdf)
- [Geant4 Book For Application Developers](https://geant4-userdoc.web.cern.ch/UsersGuides/ForApplicationDeveloper/fo/BookForApplicationDevelopers.pdf)