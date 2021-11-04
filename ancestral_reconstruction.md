
## Exercise 1: ProteoVision: visualization of proteins in 1D, 2D and 3D 
For this exercise you can use a multiple sequence alignment OR a single sequence.

**1. Go to [ProteoVision](https://proteovision.chemistry.gatech.edu/)** \
Skip the default tutorial and select the `DESIRE` mode.

![](https://github.com/Claualvarez/Sequence_analysis_intro/blob/master/figures/skip_tutorial.png)

**2. Select a phylogenetic group (or groups) and polymer.** \
For this tutorial, we will use the MSA of uL02 that includes Bacteria and Archaea. \
The MSA viewer will appear on the right pannel.

![](https://github.com/Claualvarez/Sequence_analysis_intro/blob/master/figures/TwinCons_params.png)

**3. Use the structure of E. coli for 3D visualization.** \
Once a polymer has been selected, two applets will appear on the right pannel: the topology viewr and the 3D viewer.

![](https://github.com/Claualvarez/Sequence_analysis_intro/blob/master/figures/uL02_2D_3D.png)

**4. Data mapping** \
Use the drop-down menu on the topology viewer to map sequence conservation (TwinCons or Shannon entropy) onto your protein.

![](https://github.com/Claualvarez/Sequence_analysis_intro/blob/master/figures/Alignment_tools.png)

Finally, download the alignment.
  
____
## Exercise 2: ANCESCON: Ancestral Sequence Reconstruction

The goal of ancestral sequence reconstruction methods is to generate the most likely sequence of internal nodes in a phylogeny. \
For this tutorial we will use the web-based implementation of ANCESCON in the MPI Bioinformatics Toolkit. \
The original web-based implementation is avaiable [here](http://prodata.swmed.edu/ancescon/ancescon.php), has more options to costumize the calculation, but requires extra steps for file-format conversion.

![](https://github.com/Claualvarez/Sequence_analysis_intro/blob/master/figures/MPI_loadANCESCON.png)

**1. Upload the MSA of uL02 and submit the job** \
Note: You may get the following message:

`We found an identical copy of your job in our database!`

Select the option to `Load existing job`.

**2. Visualize the results** \
ANCESCON outputs two results: a phylogeny (gene tree) and the reconstructions of the most likely sequences at each node. \
Select the vertical representation of the tree to examine the tree topology. 

![](https://github.com/Claualvarez/Sequence_analysis_intro/blob/master/figures/ANCESCON_Tree.png)

Go to the `Data` tab and scroll down. \
The reconstructed sequences are in a section called `The prediction for all ancestral nodes:`

![](https://github.com/Claualvarez/Sequence_analysis_intro/blob/master/figures/ANCESCON_results.png)

Keep scrolling down. \
The first sequences without a header corresponds to the prediction for the node at the root.

![](https://github.com/Claualvarez/Sequence_analysis_intro/blob/master/figures/ANCESCON_rootseq.png)

**3. Let's compare this result to results obtained with alternative alignments.** \
Use the following pre-computed reconstructions for the same set of sequences for the comparison:  

>
>\>uL02ab_ProteoVision_root \
MAIKKYKPTTPGRRHMTVSDFSEITKSTPEKSLLVPLKKTGGRNNQGRITVRHRGGGHKRQYRIIDFKRNKDGIPAKVASIEYDPNRSARIALLHYADGEKRYILAPKGLKVGDTVVSGEDADIKPGNCLPLRNIPVGTIVHNIELKPGKGGQLARSAGTSAQLMAKEGDYAQLRLPSGEMRMVLSECRATIGQVGNADHMNISLGKAGRSRWLGRRPTVRGVAMNPVDHPHGGGEGRTSGGRHPVSPWGKPAKGYKTRSKKKASDKFIVRRRKKKKKRK \
>\>uL02ab_mafft-default \
>AVVKCKPTSPGRRHVVKVVNPELHKGKPFAPLLEKNSKSGGRNNNGRITTRHIGGGHKQAYRIVDFKRNKDGIPAVVERLEYDPNRSANIALVLYKDGERRYILAPKGLKAGDQIQSGVDAAIKPGNTLPMRNIPVGSTVHNVEMKPGKGGQLARSAGTYVQIVARDGAYVTLRLRSGEMRKVEADCRATLGEVGNAEHMLRVLGKAGAARWRGVRPTVRGTAMNPVDHPHGGGEGRNFGKHPVTPWGVQTKGKKTRSNKRTDKFIVRRRS \
>\>uL02ab_clustal-omega
>AVVKCKPTSPGRRHVVKVVNPELHKGKPFAPLLEKNSKSGGRNNNGRITTRHIGGGHKQAYRIVDFKRNKDGIPAVVERLEYDPNRSANIALVLYKDGERRYILAPKGLKAGDQIQSGVDAAIKPGNTLPMRNIPVGSTVHNVEMKPGKGGQLARSAGTYVQIVARDGAYVTLRLRSGEMRKVEADCRATLGEVGNAEHMLRVLGKAGAARWRGVRPTVRGTAMNPVDHPHGGGEGRNFGKHPVTPWGVQTKGKKTRSNKRTDKFIVRRRS
>

Use your favourite alignment tool in the MPI bioinformatics toolkit to align the predicted sequences at the root.

![](https://github.com/Claualvarez/Sequence_analysis_intro/blob/master/figures/Alignment_tools.png)
____

### On Multiple Sequence Alignments

The goal of multiple sequence alignments is to introduce gaps such that residues in 
the same column are homologous.

#### Alignment methods
- Progressive construction:
  - These methods reduce MSAs to a series of pairwise operations.
  - Popular algorithms: [Clustal](https://www.ebi.ac.uk/Tools/msa/clustalo/), [T-Coffee](https://www.ebi.ac.uk/Tools/msa/tcoffee/).

- Iterative methods
  - Similar to progressive contruction methods + iterative realignment step.
  - Popular algorithms: [MUSCLE](https://www.ebi.ac.uk/Tools/msa/muscle/) and [MAFFT](https://www.ebi.ac.uk/Tools/msa/mafft/).

- Other methods
  - Structure-derived MSAs.

### Desktop alignment viewers 
- [SeaView](http://doua.prabi.fr/software/seaview)
- [AliView](https://ormbunkar.se/aliview/#DOWNLOAD) (recommended)
- [JalView](http://www.jalview.org/getdown/release/)


