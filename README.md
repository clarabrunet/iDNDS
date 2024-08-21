# iDNDS
Authors: Clara Brunet Villarejo, Miho Nakamura, Pere Puigbo

Year: 2024

Title: Indel-aware analysis of positive selection

**Description**:

This program calculates dNdS (modified from  Nei-Gojobori 1986) taking into account indels in the pairwise alignment. Indels are treated as non-synonymous substitutions in the pair-wise alignment.

**Reference**: 

Saeka Shimochi, Clara Brunet, Margalida Fontcuberta-Rigo, Katja Hrovat, Pere Puigbò, Miho Nakamura (2024) Bone mechano-response is driven by transitions in vertebrate evolution. In preparation. 

**Structure**:

- src/: Contains the Python libraries.
- scripts/: Contains the main launcher script.


**Requirements**:

Python

Biopython

**Usage**:

The main launcher script takes a FASTA file as input containing two aligned codon sequences.

```bash
python iDNDS.py <fasta_file>
```
**Output**: 

- Nd: Total observed non-synonymous substitutions.
- Sd: Total observed synonymous substitutions.
- N: Total expected non-synonymous sites.
- S: Total expected synonymous sites.
- pn and ps: Proportion of observed non-synonymous and synonymous changes.
- dn and ds: Adjusted rates of non-synonymous and synonymous changes.
-    dN/dS: Positive selection ratio.
