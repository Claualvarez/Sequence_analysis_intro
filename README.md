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
  Click on the names of the tabs to explore other programs in the Bioinformatics Toolkit.

  ![](https://github.com/Claualvarez/Sequence_analysis_intro/blob/master/figures/Welcome_hhblits.png)

> Which one of the ``Search`` programs would you use for structure prediction? \
> What are the ``Alignment`` programs in the Bioinformatics toolkit? \
> Which program reconstructs ancestral protein sequences?
_____

## Exercise 2: Sequence similarity search

For this exercise you will need a query sequence in a FASTA file format.

**1. Go to the ``Search program`` called *[ProtBLAST/PSI-BLAST](https://toolkit.tuebingen.mpg.de/tools/psiblast)*.**

  ![](https://github.com/Claualvarez/Sequence_analysis_intro/blob/master/figures/MPI_BLAST.png)
  
**2. Paste your sequence in the input box or upload it using the ``Upload Sequence`` button.**

**3. Submit the job and wait while your submission is processed.**

  ![](https://github.com/Claualvarez/Sequence_analysis_intro/blob/master/figures/BLAST_processing.png)
  
**4. Examine the results** \
  The reults section is divided in three sections ``Visualization``, ``Hitlist`` and ``Alignments``. \
  By clicking on any of the hits displayed on the visualization section you will be redirected to the pairwise alignment between your query sequence and the hit you clicked on.
  
  ![](https://github.com/Claualvarez/Sequence_analysis_intro/blob/master/figures/BLAST_hits.png)
  
**5. Locate the ``Forward``button at the top of the ``Results``page and click on it.** \
  We will forward the *Aligned regions* with a E-value better than 0.00001 (1E-05) to a Multiple Sequence Alignment algorithm.
  
  ![](https://github.com/Claualvarez/Sequence_analysis_intro/blob/master/figures/BLAST_forward.png)



