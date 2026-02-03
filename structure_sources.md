# Sourcing atomic structures for input

There are many ways to source input structures for molecular dynamics (MD) and density functional theory (DFT) calculations. The best approach depends on a few things:
* Is the structure periodic (e.g. is it a crystal, molecule, or molecular cluster)?
* Is it a well-known compound?

Here are the main sources I use for periodic atomic structures.

## Build from scratch

If the structure you need is simple or built using a number of common motifs (e.g. graphene, water molecules), it's usually not too difficult to build it yourself. There are many software packages and tools you can use to do this. Today, we will use [Atomic Simulation Environment (ASE)](ase.md).

## Databases

These are online repositories of crystal and molecular structures. You can actually access strucutres from some of these via ASE. Some that I have used are:
* [Materials Project](https://next-gen.materialsproject.org/) 
* [Crystallography Open Database](https://www.crystallography.net/cod/)
* [Cambridge Crystallographic Data Centre](https://www.ccdc.cam.ac.uk/structures/)

## Papers

Sometimes authors will publish their inputs or outputs as part of the supplementary information for a publication. I've had pretty good success finding and adapting atomic structures this way. 

You can search for papers featuring the strucutre your after, and also explore references and citations. I find that Nature papers are most likely to have attached structures - especially Nature Communications, since they often require full calculation repeatability.

## Next

Next we will create a structure using ASE. [Click here](ase_structure_creation.md).
