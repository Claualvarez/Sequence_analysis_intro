# Multiple Sequence Alignments

- The goal of multiple sequence alignments is to introduce gaps such that residues in 
the same column are homologous.

**Alignment methods**
- Progressive construction:
  - These methods reduce MSAs to a series of pairwise operations.
  - These algorithms are heuristic.
  - Popular algorithms: Clustal, T-Coffee.

- Iterative methods
  - Similar to progressive contruction methods + iterative realignment step.
  - Popular algorithm: MUSCLE and MAFFT.

1. Download and install [SeaView](http://doua.prabi.fr/software/seaview)
2. Copy and paste the following lines
   ```
   >human
   KRSV
   >chimp
   KRV
   >gorilla
   KSV
   >orang
   KPRV
   ```
   
   How we align sequences affects tree estimation.

3. Download the results of the sequence similarity search in fasta format.
4. Open the fasta file in SeaView.
   - Try aligning your sequences with clustal and muscle.
   - Upload your sequences to [MAFFT](https://mafft.cbrc.jp/alignment/server/)

5. Multiple structure alignment and multiple sequence aligmnment.
   In a multiple structure alignment, positions correspond to similar three-dimensional
   conformations. Structure similarity does not always imply homology.
   > Carpentier and Chomilier (2019). Bioinformatics, 35 (20), 3970-3980
   
   
