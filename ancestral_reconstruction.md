
## Exercise 1: ProteoVision: visualization of proteins in 1D, 2D and 3D 
For this exercise you can use a multiple sequence alignment OR a single sequence.

**1. Go to [ProteoVision](https://proteovision.chemistry.gatech.edu/)** \
Skip the default tutorial.

![](https://github.com/Claualvarez/Sequence_analysis_intro/blob/master/figures/skip_tutorial.png)

We will use the 'DESIRE' mode.

![](https://github.com/Claualvarez/Sequence_analysis_intro/blob/master/figures/user_upload_mode.png)

**2. Upload your sequence(s) in FASTA format** \
The MSA viewer will appear on the right pannel once you upload your sequence(s).

**3. Use the PDB code of your protein for the visualization and select a polymer ** \
Once a polymer has been selected, two applets will appear on the right pannel: the topology viewr and the 3D viewer.

![](https://github.com/Claualvarez/Sequence_analysis_intro/blob/master/figures/proteovision_loaded_str.png)

**4. Data mapping** \
Use the drop-down menu on the topology viewer to map data onto your protein.

![](https://github.com/Claualvarez/Sequence_analysis_intro/blob/master/figures/proteovision_menu.png)

Finally, you can download the computed data as pymol script.
  
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


