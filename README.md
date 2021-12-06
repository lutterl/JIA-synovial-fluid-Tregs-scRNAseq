# JIA-synovial-fluid-Tregs-scRNAseq

Count data of scRNA-seq data derived from three patients with oligo JIA. 
Live CD3+CD4+CD25+CD127low cells were sorted into 384-well hard shell plates (Biorad) with 5 μl of vapor-lock (QIAGEN) containing 100-200 nl of RT primers, dNTPs and synthetic mRNA Spike-Ins and immediately spun down and frozen to −80°C. Cells were prepared for SORT-seq as previously described (Muraro MJ, Dharmadhikari G, Grün D, Groen N, Dielen T, Jansen E, et al. A Single-Cell Transcriptome Atlas of the Human Pancreas. Cell Syst. 2016 Oct;3(4):385-394.e3.). Illumina sequencing libraries were then prepared with the TruSeq small RNA primers (Illumina) and sequenced single-end at 75 bp read length with 60.000 reads per cell on a NextSeq500 platform (Illumina). Sequencing reads were mapped against the reference human genome (GRCh38) with BWA. 

Barcode counts = raw mapped counts

Read counts = UMI corrected version of barcode counts

Transcript counts = poisson counting statistics corrected version of UMI corrected version

# Scripts used for all analyses
All code used follows the guidelines as outlined by the publishers of each package
1. Quality control scRNAseq samples (run in R)
2. Script integrated scRNAseq analysis (run in R)
3. Script pySCENIC SF Treg (run in python using Jupyter notebook)
4. Script TCRseq analysis (run in R)
