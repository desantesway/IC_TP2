# Reactive Systems & Concurrency Modeling (Second Assignment)

## **Grade: 16/20** 🎯

This repository contains my solutions for the practical assignment of the **Interaction and Concurrency** course. The project involved the formal modeling and analysis of concurrent systems, leveraging theoretical concepts and the mCRL2 toolset for verification.


## 🧠 Key Concepts Applied

- **Strong Bisimulation:** Formally proven equivalence between system states.
- **Process Algebra:** Used to model concurrent processes (`Road`, `Rail`, `Signal`).
- **Synchronization:** Handled via shared actions (`green`, `red`, `up`, `down`) to ensure safe coordination.
- **Model Checking:** Utilized mCRL2 to generate and analyze the system's state space.

## ⚙️ Technical Implementation

The core of the practical work was modeling a railway crossing controller:

- **Processes:** Defined three concurrent processes (`Road`, `Rail`, `Signal`).
- **Synchronization:** Implemented using action synchronization in mCRL2 to prevent unsafe states (e.g., train and car on the crossing simultaneously).
- **Verification:** The model was compiled into a Labeled Transition System (LTS) to verify correct behavior and ensure mutual exclusion.

## 📊 Outcome

The model successfully demonstrates a safe control logic for the railway crossing, where the `Signal` process arbitrates access to the critical section (the crossing), ensuring no collisions occur. The state space analysis confirms the absence of deadlocks and the preservation of safety properties.
