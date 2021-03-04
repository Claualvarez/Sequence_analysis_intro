
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

  The MSA that we will use is MAFFT. Loacte and select ``MAFFT``on the tools menu and click the ``Forward`` button.
  
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
  
**3. Download the alignment** 

## Exercise 3: ProteoVision: visualization of proteins in 1D, 2D and 3D
For this exercise we will use the multiple sequence alignment that was generated using the MPI Bioinformatica toolkit.

**1. Go to [ProteoVision](https://proteovision.chemistry.gatech.edu/)
Skip the default tutorial.



And select the 'User upload' mode.
  
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


