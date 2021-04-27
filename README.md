# ProtPep37_2021
dataset of short peptides (2-7 amino acids) bound to proteins annotated for structural similarity and augmented with docking decoys

This folder contains the ProtPep37_2021 set of protein-peptide complexes, a set of 322 peptide with 3 to 7 amino acids bound to protein chain(s). The peptides and the binding site residues comprise only standard amino acids, have no missing atoms or alternate locations. Protein chains are defined as chains of amino acids with 50 or more amino acids.

The dataset also provides docking decoys and is annotated for structural similarity.

It is freely available under the LGPL 2.1 Open Source license

**Please cite**
Michel F. Sanner, Leonard Dieguez, Stefano Forli, Ewa Lis. Improving Docking Power for peptides using Random Forest, JCIM ...

<h2>complexes.list:</h2>
Contains the list of protein-peptide complex names. The names have 4 fields separated by underscore characters ('_'). The first field of the PDBID. The second is the chain ID of the peptide. The third is a dash-separated list of chain IDs in the biomolecule. The fourth field in the 0-based biomolecule used to build the biologically active molecule.

<h2>contactingChains.csv:</h2>
This comma separated file provides for each entry the complex name, the list of protein chains ID(s) and the number and length of these chains, the chain ID(s) short peptidic chains (i.e. chains with less than 50 amino acids and different from the peptide ligand) their number and length

<h2>similarityScores:</h2>
This folder contains a comma separated file for each of the 377 protein chain in the ProtPep37_2021 data set. the csv file provide a tm1 and tm2 column which hols the 2 TMscores reported by TM_align along with a min and max column for these 2 values.

<h2>peptides:</h2>
This folder contains PDBQT files of the crystallographic pose of the peptide ligands, along with ligand poses minimized with ADFR in the context of the rigid receptor.

<h2>proteins:</h2>
This folder contains PDBQT files of the chains of the biomolecule contacting the ligand peptide.


------------------------------------------------
Contact: Dr Michel Sanner sanner at scripps.edu
