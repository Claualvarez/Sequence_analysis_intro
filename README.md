
## Exercise 1: Sequence similarity search

For this exercise you will need a query sequence in a FASTA format.

**1. Go to the ``Search program`` called *[ProtBLAST/PSI-BLAST](https://toolkit.tuebingen.mpg.de/tools/psiblast)* at [the MPI Bioinformatics toolkit](https://toolkit.tuebingen.mpg.de/).**

  ![](https://github.com/Claualvarez/Sequence_analysis_intro/blob/master/figures/MPI_BLAST.png)
  
**2. Paste your sequence in the input box.**

**3. Submit the job and wait while your submission is processed.**

  ![](https://github.com/Claualvarez/Sequence_analysis_intro/blob/master/figures/BLAST_processing.png)
  
**4. Examine the results.** \
  The reults window is divided in three sections ``Visualization``, ``Hitlist`` and ``Alignments``. \
  By clicking on any of the hits on the visualization section you will be redirected to the pairwise alignment between your query sequence and the hit you clicked on.
  
  ![](https://github.com/Claualvarez/Sequence_analysis_intro/blob/master/figures/BLAST_hits.png)
  
**5. Locate the ``Forward``button at the top of the ``Results``page and click on it.** \
  We will forward the *Aligned regions* with a E-value better than 0.00001 (1E-05) to a Multiple Sequence Alignment (MSA) algorithm.
  
  ![](https://github.com/Claualvarez/Sequence_analysis_intro/blob/master/figures/BLAST_forward.png)

  The program that we will use for this exercise is called MAFFT. \
  Loacte and select ``MAFFT``on the tools menu and click the ``Forward`` button.
  
  ![](https://github.com/Claualvarez/Sequence_analysis_intro/blob/master/figures/BLAST_forward_MAFFT.png)
  
  You will be redirected to a new program manager window.
  
_____

## Exercise 2: Multiple Sequence Alignment

**1. Align the sequences obtained by your prevouos sequence similarity search using MAFFT** \
  We will use the predefined default parameters. Click the ``Submit``button.

  ![](https://github.com/Claualvarez/Sequence_analysis_intro/blob/master/figures/MAFFT_input.png)
  
**2. Examine the results of MAFFT** \
  By default, the Bioinformatics Toolkit will display the results in the ``CLUSTAL Alignment`` format.
  
  ![](https://github.com/Claualvarez/Sequence_analysis_intro/blob/master/figures/MAFFT_default_out.png)

  Go to the ``AlignmentViewer``tab.
  
  ![](https://github.com/Claualvarez/Sequence_analysis_intro/blob/master/figures/MAFFT_AlnView.png)
  
  Use the horizontal scroll bar to examine the entire length of the alignment.
  
**3. Download the alignment** \
Go to ``FASTA Alignment`` and Download MSA.  

## Exercise 3: ProteoVision: visualization of proteins in 1D, 2D and 3D 
For this exercise you can use a multiple sequence alignment OR a single sequence.

**1. Go to [ProteoVision](https://proteovision.chemistry.gatech.edu/)** \
Skip the default tutorial.

![](https://github.com/Claualvarez/Sequence_analysis_intro/blob/master/figures/skip_tutorial.png)

We will use the 'User upload' mode.

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


