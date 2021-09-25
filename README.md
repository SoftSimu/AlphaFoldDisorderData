# Proteins, structures and data from the manuscript

**AlphaFold2:  A role for disordered proteinprediction?
*by Carter J. Wilson, Wing-Yiu Choy, and Mikko Karttunen***

## Data organization ##
There is a folder (structures/) containing the PDB structures from AlphaFold2 used in this work, the names of these files corresponds to their UniProt IDs. In addition there is a file (combined.dat) that contains all the raw predictions and sequence metrics. The organization of that file is as follows:

1. \>UniProtID\|DisProtID
2. Amino acid sequence
3. DisProt annotation (1 = disordered, 0 = ordered)
4. DisProt-PDB annotation (1 = disordered, 0 = ordered, - = no data)
5. DSSP assignment (H = a-helix, G = 310 helix, I = pi-helix, T = H-bond turn, E = B-strand, B = B-bridge, S = bend, - = coil)
6. PAE assignment ('|' are used to seperate values for each amino acid)
7. AUCpreD disorder score
8. AUCpreD binary prediction
9. AUCpreD-np disorder score
10. AUCpreD-np binary prediction
11. DisoMine disorder score
12. DisoMine binary prediction
13. ESpritz-D disorder score
14. ESpritz-D binary prediction
15. fIDPnn disorder score
16. fIDPnn binary prediction
17. fIDPlr disorder score
18. fIDPlr binary prediction
19. Predisorder disorder score
20. Predisorder binary prediction
21. RawMSA disorder score
22. RawMSA binary prediction
23. SPOT-Disorder1 disorder score
24. SPOT-Disorder1 binary prediction
25. SPOT-Disorder-S disorder score
26. SPOT-Disorder-S binary prediction
27. SPOT-Disorder2 disorder score
28. SPOT-Disorder2 binary prediction

And so on for all the proteins considered. Relevant data can be parsed by considering only the line of interest and every 28th line after that.
