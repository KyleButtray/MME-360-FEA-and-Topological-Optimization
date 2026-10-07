# MME 360 – FEA and Topological Optimization

finite element analysis of structural components
under load, validated against theory, using Siemens NX Nastran & Topological Optimization

## Projects & Labs

| Folder | What it is | Description (add yours) |
|---|---|---|
| `Bridge/` | Full bridge structure model + assembly parts (Loading profile, test frame) and STL exports | Generated a bridge model to optimize a 3D printed bridge for minimum weight to support the given test constraints. Bridge was then printed and physically tested under load to compare to FEA results. Loading conditions include mounting the bridge on the "test frame.prt" and applying a load of 200lbs to the "Loading profile.prt". |
| `Cantilevered Beam/` | Cantilevered beam FEA: part model, mesh (`.fem`), solved results (`.dat`, `.f04`, `.f06`), and a solver convergence plot | Used Nastran FEA to simulate the bending stress created by an applied load at the end of a cantilevered beam. Experimented with different mesh shapes and sizes to observe convergence to a certain stress value while optimizing simulation time. |

## Tools used
Siemens NX, Nastran solver (FEA)
