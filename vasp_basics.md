# Getting started with VASP

[Navigation Page](navigation_page.md)

This is a brief overview of the basics of using VASP. 

VASP is software that runs density functional theory (DFT) and ab initio molecular dynamics (AIMD) calculations, usually on periodic structures. It uses a plane-wave basis set to build the electronic wavefunctions.

VASP has in-depth documentation on their [wiki](https://vasp.at/wiki/The_VASP_Manual), including:
* Pages on all [input files](https://vasp.at/wiki/Input), [output files](https://vasp.at/wiki/Output), and [INCAR tags](https://vasp.at/wiki/Category:INCAR_tag)
* [Tutorials to get started](https://vasp.at/wiki/O_atom)
* [Theory on how VASP calculates things](https://vasp.at/wiki/Category:Theory)

## Inputs

There are four input files that each VASP calculation requires:

| File | Purpose | 
| --- | ------------- | 
| [INCAR](https://www.vasp.at/wiki/INCAR) | Text file containing all INCAR tags for the calculation. This is where you tell VASP what to do. Certain variables, like `ENCUT`, should be benchmarked for each project.| 
| [POSCAR](https://vasp.at/wiki/POSCAR) | Text file containing the atomic structure for your calculation.  We will look at building this today.  |  
| [KPOINTS](https://vasp.at/wiki/KPOINTS) | Text file containing the Bloch vectors (k points) used to sample the Brillouin zone. Can be a regular mesh, or a specified path (for plotting the band structure, for example).  The more k points, the more precise (and expensive) the calculation.  This should be benchmarked for each project and calculation type. |   
| [POTCAR](https://vasp.at/wiki/POTCAR) | Text file containing the pseudopotential for each atomic species in the same order as in the POSCAR. This is the equivalent of your exchange-correlation functional. These should not be edited. To use hybrid functionals, specify them in the INCAR file. | 

## Running VASP

Once the inputs are ready, run VASP from within the directory containing the input files. Once the calculation begins, VASP will start writing the outputs to this same directory. 

It's best practice to have a separate directory for each calculation, so you can look back and know the details of each job.

For information on how to run VASP on the available computing clusters in CTCMS, see our [VASP loop page](https://uq.sharepoint.com/:fl:/r/teams/6geo7aqm/Shared%20Documents/VASP/Running%20VASP%20on%20each%20cluster.loop?d=w821ea05106d340e5ac1d8ecc27060955&csf=1&web=1&e=Mpec4i&nav=cz0lMkZ0ZWFtcyUyRjZnZW83YXFtJmQ9YiUyMUlpOVZxUHV4eUVLYW11SW1UV2hnYklvMzkwRnpOdjFLbVJQSE9TdDVBSm84cTVwSTZrQzdSS05Gb0VVcnVRdHomZj0wMVFUUzdGRFNSVUFQSUZVWUc0VkFLWUhNT1pRVFFNQ0tWJmM9JTJGJmE9TG9vcEFwcCZwPSU0MGZsdWlkeCUyRmxvb3AtcGFnZS1jb250YWluZXI%3D) (login required).

## Outputs

VASP gives several different output files, depending on which task is performed. There are usually at least 7 files. Most of them can be read with a text editor, a notable exception being the [WAVECAR](https://vasp.at/wiki/WAVECAR) file, which is written in binary for VASP to read.

## Next

Next we will create a structure to use for a VASP calculation. [Click here](structure_sources.md).