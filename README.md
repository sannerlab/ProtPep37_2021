![stripSet](https://user-images.githubusercontent.com/47902071/119055938-b3e3ca00-b97e-11eb-84c4-2ca058dd473d.png)

# ProtPep37_2021
dataset of short peptides (3-7 amino acids) bound to proteins annotated for structural similarity and augmented with docking decoys

This folder contains the ProtPep37_2021 set of protein-peptide complexes, a set of 322 peptide with 3 to 7 amino acids bound to protein chain(s). The peptides and the binding site residues comprise only standard amino acids, have no missing atoms or alternate locations. Protein chains are defined as chains of amino acids with 50 or more amino acids.

The dataset also provides docking decoys and is annotated for structural similarity.

It is freely available under the LGPL 2.1 Open Source license

For convienence we also provide the set of 47 complexes use in the benchmark by Rentzsch et al. (10.1093/bib/bbv008) along with decoys (pep47folder) .

**Please cite**
Michel F. Sanner, Leonard Dieguez, Stefano Forli, Ewa Lis. Improving Docking Power for peptides using Random Forest, JCIM ...

<h2>Content</h2>

<h3>complexes.list</h3>
Contains the list of protein-peptide complex names. The names have 4 fields separated by underscore characters ('_'). The first field of the PDBID. The second is the chain ID of the peptide. The third is a dash-separated list of chain IDs in the biomolecule. The fourth field in the 0-based biomolecule used to build the biologically active molecule.

<h3>contactingChains.csv</h3>
This comma separated file provides for each entry the complex name, the list of protein chains ID(s) and the number and length of these chains, the chain ID(s) short peptidic chains (i.e. chains with less than 50 amino acids and different from the peptide ligand) their number and length

<h3>similarityScores/</h3>
This folder contains a comma separated file for each of the 377 protein chain in the ProtPep37_2021 data set. the csv file provide a tm1 and tm2 column which hols the 2 TMscores reported by TM_align along with a min and max column for these 2 values.

<h3>peptides/</h3>
This folder contains the following 4 subfolders containing PDBQT files for the peptides:
     <ul>
     <li>XR: crystallographic peptide</li>
     <li>XM: minimized crystallographic peptide</li>
     <li>DO: poses resulting fom docking (multimodel pdb file)</li>
     <li>NS: poses resulting fom neighborhood search docking (multimodel pdb file)</li>
     </ul>
     NOTE: 2h2f_B_A-B_0 and 4k75_B_A-B_0 have no docked poses (only NS poses)
    
<h3>proteins/</h3>
This folder contains PDBQT files of the chains of the biomolecule contacting the ligand peptide.

<h3>pep47</h3>
This folder containg the set of 47 complexes used as testing set, including the original PDBQT files and the CPPs we calculated.

------------------------------------------------
Contact: [mailto](mailto:sanner@scripps.edu) Dr. Michel Sanner 

![stripCPP](https://user-images.githubusercontent.com/47902071/119056253-3a98a700-b97f-11eb-98b1-a0466d304f8d.png)
