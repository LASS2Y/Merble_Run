# Merbl Run

A 3D-printed marble run designed in Onshape: an 8 mm marble rolls through a rail, a plinko board, a staircase and a funnel.

This is my Week 2 (CAD) project for Hack Club's **Half Life** program, built by following the [merbl guide](https://github.com/karnxx/merbl/blob/main/guide.md).

![Marble run render](images/render.png)

## Parts

| Part | How it's made | Key dimensions |
|---|---|---|
| Rail | Sweep of a C-shaped profile along a 3D path, with a U-turn | Ø9 mm inner / Ø14 mm outer, 20° opening |
| Plinko | Extruded board with a linear pattern of diamond pegs | 3 mm floor, 16 mm walls, pegs spaced 17 mm |
| Staircase | Stepped sketch extruded three times (floor + two walls) | 5 × 5 mm steps, 10 mm floor, 3 mm walls |
| Funnel | Revolve, then two fillets | 13.5 mm fillets |
| Marble | Revolved semicircle | Ø8 mm |

## CAD

- Onshape document: [marble](https://cad.onshape.com/documents/79d43b1c606cd961a2091fa4/w/d65fd6ded1f243f0b2b967c1/e/dde4b8347fda98495cc02b7b)
- STL exports: [`cad/`](cad/)

Each part is a separate module and is printed on its own.

## Printing

Sliced in UltiMaker Cura:

- PLA, 0.2 mm layers, 15% infill
- Tree supports, placement "Touching Buildplate"
- The open side of each channel faces up, and supports must never grow inside the channel where the marble rolls. Support blockers are used where needed.

## What I learned

- Sweeps, point-normal planes and composite curves
- New / Add / Remove extrudes, start offsets and extrude directions
- Revolve, fillet and the Transform tool
- Exporting STLs and slicing with tree supports

## Status

- [x] Rail
- [x] Plinko
- [x] Staircase
- [x] Funnel
- [x] STL export
- [ ] Slicing (fixing supports inside the rail)
- [ ] Test print
