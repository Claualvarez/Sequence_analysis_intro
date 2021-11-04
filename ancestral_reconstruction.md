
## Exercise 1: ProteoVision: visualization of proteins in 1D, 2D and 3D 
For this exercise you can use a multiple sequence alignment OR a single sequence.

**1. Go to [ProteoVision](https://proteovision.chemistry.gatech.edu/)** \
Skip the default tutorial.

![](https://github.com/Claualvarez/Sequence_analysis_intro/blob/master/figures/skip_tutorial.png)

We will use the 'DESIRE' mode.

**2. Select a phylogenetic group (or groups) and polymer.** \
For this tutorial, we will use the MSA of uL02 that includes Bacteria and Archaea. \
The MSA viewer will appear on the right pannel.

![](https://github.com/Claualvarez/Sequence_analysis_intro/blob/master/figures/TwinCons_params.png)

**3. Use the structure of E. coli for 3D visualization and select a polymer ** \
Once a polymer has been selected, two applets will appear on the right pannel: the topology viewr and the 3D viewer.

![](https://github.com/Claualvarez/Sequence_analysis_intro/blob/master/figures/uL02_2D_3D.png)

**4. Data mapping** \
Use the drop-down menu on the topology viewer to map sequence conservation (TwinCons or Shannon entropy) onto your protein.

![]()

Finally, download the alignment.
  
____

### Additional information

The goal of multiple sequence alignments is to introduce gaps such that residues in 
the same column are homologous.

#### Alignment methods
- Progressive construction:
  - These methods reduce MSAs to a series of pairwise operations.
  - Popular algorithms: [Clustal](https://www.ebi.ac.uk/Tools/msa/clustalo/), [T-Coffee](https://www.ebi.ac.uk/Tools/msa/tcoffee/).

- Iterative methods
  - Similar to progressive contruction methods + iterative realignment step.
  - Popular algorithms: [MUSCLE](https://www.ebi.ac.uk/Tools/msa/muscle/) and [MAFFT](https://www.ebi.ac.uk/Tools/msa/mafft/).
  
### Desktop alignment viewers 
- [SeaView](http://doua.prabi.fr/software/seaview)
- [AliView](https://ormbunkar.se/aliview/#DOWNLOAD) (recommended)
- [JalView](http://www.jalview.org/getdown/release/)


