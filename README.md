# BacARscan
Bacterial Antibiotic Resistance scanning and annotations by profile Hidden Markov Models


***********How to use it? **************

######Files description#####

nARGhmm: Library of 254 nucleotide ARG HMMs

pARGhmm: Library of 254 protein ARG HMMs
ARG_Annotations: Annotation of 254 profile ARG HMMs

HMMER download and install as standalone using link: http://hmmer.org/download.html

*****Scanning of protein sequences will perform using hmmscan*****

“/hmmer-3.1b2-linux-intel-x86_64/src/hmmscan --cpu 4 -E 0.000001 --tblout abc.out pARGhmm protein.fasta”


****Scanning of gene sequences will perform using nhmmscan******

/hmmer-3.1b2-linux-intel-x86_64/src/nhmmscan --cpu 4 -E 0.000001 --tblout abc.out nARGhmm gene.fasta &


Using above commands user can scan their protein and nucleotide sequences; upon search it will give the similarity score and e-value. Depending on the scores user can select hits and retrieve their complete annotation using “ARG_Annotations” file.


Visit our website for latest version & scanning of ARGs using freely accessible tool: http://proteininformatics.org/mkumar/bacarscan/
