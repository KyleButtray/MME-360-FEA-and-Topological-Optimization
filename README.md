# MME 360 – [Add course title, e.g. "Mechanics of Materials" / "FEA"]

[1-2 sentence overview — e.g. finite element analysis of structural components
under load, validated against theory, using Creo Simulate / Nastran.]

## Projects & Labs

| Folder | What it is | Description (add yours) |
|---|---|---|
| `Bridge/` | Full bridge structure model + assembly parts (base, clamp plate, rollers, test frame) and STL exports; `Da Bridge.png` is a render of the final design | TODO — this looks like a capstone-style project; give it a full write-up |
| `Cantilevered Beam/` | Cantilevered beam FEA: part model, mesh (`.fem`), solved results (`.dat`, `.f04`, `.f06`), and a solver convergence plot | TODO |
| `Plant hanger/` | Plant hanger FEA with two solution runs, including stress/convergence result files and plots | TODO |
| `Tensile Bar/` | Tensile bar FEA: part, mesh, and solved results | TODO |
| `body_Buttray.prt`, `tensegrity table.prt` | Additional part models | TODO |

> **Heads up on file size:** the FEA result files (`.op2`, `.dat`) in `Plant hanger/` are ~28–30 MB each — well under GitHub's 100 MB hard limit, but large enough to slow down cloning. If you don't need the raw solver output long-term, consider keeping just the summary plots/PDFs and dropping the `.op2`/`.dat` files, or using [Git LFS](https://git-lfs.com) for them.

## Suggested next steps to polish this repo
- [ ] For each FEA project, state: the loading/boundary conditions, mesh approach, and key result (e.g. max stress, deflection) — this is what makes an FEA project readable to a non-expert
- [ ] Embed the existing result plots (`*_Solution_Monitor_Graphs.html` → screenshot, or the `.png` convergence plots) directly in this README
- [ ] `dean-cain-superman.gif` — looks like a stray/inside-joke file; remove it or move it into whichever project it's actually a reference for
- [ ] Rename `Bridge`, `Cantilevered Beam`, `Plant hanger`, `Tensile Bar` to lowercase-hyphenated folder names for consistency (optional, but common convention)

## Tools used
Creo Simulate (FEA), MSC Nastran solver
