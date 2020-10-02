# Tutorial: Introduction to sequence analysis using the MPI Bioinformatics Toolkit

______

## Exercise 1: Getting to know the Bioinformatics Toolkit

**1. Go to https://toolkit.tuebingen.mpg.de/**
  
   ![](https://github.com/Claualvarez/Sequence_analysis_intro/blob/master/figures/Welcome.png)
 
 **2. Explore the Welcome page** \
   At the top of the page there are seven tabs that correspond to different types of analysis that you can perform on an amino acid sequence.
 
   The ``Search`` programs in the Bioinformatics Toolkit are the following:
   - HHblits
   - HHpred
   - HMMER
   - PatternSearch
   - ProtBLAST/PSI-BLAST
  
  Hover over the name of the programs to get a short description of what they do. \
  Click on the different tabs to explore other programs in the Bioinformatics Toolkit.

  ![](https://github.com/Claualvarez/Sequence_analysis_intro/blob/master/figures/Welcome_hhblits.png)

> Which one of the ``Search`` programs would you use for structure prediction? \
> What are the ``Alignment`` programs in the Bioinformatics toolkit? 

_____

## Exercise 2: Sequence similarity search

For this exercise you will need a query sequence in a FASTA format.

**1. Go to the ``Search program`` called *[ProtBLAST/PSI-BLAST](https://toolkit.tuebingen.mpg.de/tools/psiblast)*.**

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

## Exercise 3: Mulstiple Sequence Alignment

**1. Align the sequences obtained by your prevouos sequence similarity search using MAFFT** \
  We will use the predefined default parameters. Click the ``Submit``button.

  ![](https://github.com/Claualvarez/Sequence_analysis_intro/blob/master/figures/MAFFT_input.png)
  
**2. Examine the results of MAFFT** \
  By default, the Bioinformatics Toolkit will display the results in the ``CLUSTAL Alignment`` format.
  
  ![](https://github.com/Claualvarez/Sequence_analysis_intro/blob/master/figures/MAFFT_default_out.png)

  Go to the ``AlignmentViewer``tab.
  
  ![](https://github.com/Claualvarez/Sequence_analysis_intro/blob/master/figures/MAFFT_AlnView.png)
  
  Use the horizontal scroll bar to examine the entire length of the alignment.
  
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

_____

## Assignment

1. Search for homologous sequences in the PDB using the HHpred program (Search tab) in the MPI bioinformatics toolkit.
2. Select the best 10 hits, make sure to select unique hits (select only hits with different identifiers). 
3. Forward selected to AlignmentViewer (click on View Alignment).
4. The logo plot will show the most conserved positions in the alignment.
5. Copy the input sequences from the input tab and go to PhyML (in the Classification tab).
6. Compute the maximum-likelihood tree of your sequences.

The names of the nodes in the final tree correspond to PDB entries (PDBcode_chain)
You can use these codes to inspect the protein structures related to your query using pymol.
