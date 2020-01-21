# Multiple sequence alignments

- The goal of multiple sequence alignments is to introduce gaps such that residues in 
the same column are homologous.

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
4. Open the results in SeaView.
   - Try aligning your sequences with clustal and muscle.
   - Upload your sequences to [MAFFT](https://mafft.cbrc.jp/alignment/server/)
