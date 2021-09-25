# Proteins, structures and data from the manuscript

**AlphaFold2:  A role for disordered protein prediction?
*by Carter J. Wilson, Wing-Yiu Choy, and Mikko Karttunen***

- **Manuscript at:** [bioarxiv](). 
- Supplementary information: [SI]()

## Data organization ##
There is a folder (structures/) containing the PDB structures from AlphaFold2 used in this work, the names of these files corresponds to their UniProt IDs. In addition there is a file (combined.dat) that contains all the raw predictions and sequence metrics. The organization of that file is as follows:

1. \>UniProtID\|DisProtID
2. Amino acid sequence
3. DisProt-PDB annotation (1 = disordered, 0 = ordered, - = no data)
4. DisProt annotation (1 = disordered, 0 = ordered)
6. DSSP assignment (H = a-helix, G = 310 helix, I = pi-helix, T = H-bond turn, E = B-strand, B = B-bridge, S = bend, - = coil)
7. PAE assignment ('|' are used to seperate values for each amino acid)
8. AUCpreD disorder score
9. AUCpreD binary prediction
10. AUCpreD-np disorder score
11. AUCpreD-np binary prediction
12. DisoMine disorder score
13. DisoMine binary prediction
14. ESpritz-D disorder score
15. ESpritz-D binary prediction
16. fIDPnn disorder score
17. fIDPnn binary prediction
18. fIDPlr disorder score
19. fIDPlr binary prediction
20. Predisorder disorder score
21. Predisorder binary prediction
22. RawMSA disorder score
23. RawMSA binary prediction
24. SPOT-Disorder1 disorder score
25. SPOT-Disorder1 binary prediction
26. SPOT-Disorder-S disorder score
27. SPOT-Disorder-S binary prediction
28. SPOT-Disorder2 disorder score
29. SPOT-Disorder2 binary prediction

And so on for all the proteins considered. Relevant data can be parsed by considering only the line of interest and every 28th line after that.
