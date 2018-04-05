# pasta-databases
databases for mafft-homologs

This repository contains the databases (and sub-method) needed for some sub-aligner in PASTA

See `https://github.com/smirarab/pasta/` for the most up to date version of PASTA and instructions

The databases are for use in MAFFT-Homologs
Katoh, K. and Standley, D. M. (2013). MAFFT multiple sequence alignment software
version 7: Improvements in performance and usability. Molecular Biology and
Evolution, 30(4), 772–780.

See `https://mafft.cbrc.jp/alignment/software/manual/mafft-homologs2.1.html` for more information about MAFFT-Homologs
The databases within this repository are SWISS-PROT
Bairoch, A., & Apweiler, R. (2000). 
The SWISS-PROT protein sequence database and its supplement TrEMBL in 2000. 
Nucleic Acids Research, 28(1), 45–48.

See `http://www.uniprot.org/` for the most up to date version of SWISS-PROT

The sub-method used by MAFFT-Homologs is BLASTALL
Stephen F. Altschul, Thomas L. Madden, Alejandro A. Schäffer, Jinghui Zhang, Zheng Zhang, Webb Miller, and David J. Lipman (1997), 
"Gapped BLAST and PSI-BLAST: a new generation of protein database search programs", 
Nucleic Acids Res. 25:3389-3402.

See `http://nebc.nerc.ac.uk/bioinformatics/documentation/blast/blastall.html` for more information about BLASTALL

If you would like to use anoter database with MAFFT-Homologs inside of PASTA, you will need to add the datasets to this folder,
and you will need to edit the homologs file within sate-tools-linux (or sate-tools-mac) and change the localdb accordingly

localdb = "$CONTRALIGN_DIR/pasta-databases/swissprot" <- this line specifically
the last part ('swissprot') should be the beginning of the database files you would mafft-homologs to use.

