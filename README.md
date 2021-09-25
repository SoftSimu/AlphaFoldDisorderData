# Proteins, structures and data from the manuscript

**AlphaFold2:  A role for disordered proteinprediction?
*by Carter J. Wilson, Wing-Yiu Choy, and Mikko Karttunen***

## Data organization ##
There is both a folder containing the PDB structures from AlphaFold2 used in this work, and a combined.dat file that contains all the raw predictions and sequence metrics. The organization of that file is as follows:

1 >UniProtID|DisProtID
2 Amino acid sequence
3 DisProt annotation (1 = disordered, 0 = ordered)
4 DisProt-PDB annotation (1 = disordered, 0 = ordered, - = no data)
5 DSSP assignment (H = a-helix, G = 310 helix, I = pi-helix, T = H-bond turn, E = B-strand, B = B-bridge, S = bend, - = coil)
6 PAE assignment ('|' are used to seperate values for each amino acid)
7 AucPred disorder score
8 AucPred binary prediction


