Introduction
------------


.. image :: _static/workflow.png


The WGDI workﬂow consists of three main parts: **(1)** Polyploidy inference using Dotplot, Collinearity extraction, Ks distributions 
**(2)** Hierarchical inference of genomic homology resulted from recursive paleopolyploidizations. 
**(3)** Subgenomic and ancestral genome reconstruction and other evolutionary scenarios.

WGDI contains multiple subroutines, the user only needs to modify the configuration file simply, and then enter the name of the subroutine to be executed, 
Such as ``wgdi -d your.conf``.  In the following, we will describe in detail the subroutines of WGDI software.


**WGDI subroutine and function**


+----------------------------+-------------------------------------------------------------------------------------------+
|       Parameters           | Functions                                                                                 |
+=========+==================+===========================================================================================+
| -h      | Help             | Show help message and exit                                                                |
+---------+------------------+-------------------------------------------------------------------------------------------+
| -v      | Version          | Show program's version number                                                             |
+---------+------------------+-------------------------------------------------------------------------------------------+
| -d      | DotPlot          | Show homologous gene dotplot                                                              |
+---------+------------------+-------------------------------------------------------------------------------------------+
| -icl    | Collinearity     | Improved version of ColinearScan                                                          |
+---------+------------------+-------------------------------------------------------------------------------------------+
| -ks     | CalKs            | Calculate Ka/Ks for homologous gene pairs by YN00                                         |
+---------+------------------+-------------------------------------------------------------------------------------------+
| -bi     | BlockInfo        | Collinearity and Ks speculate whole genome duplication                                    |
+---------+------------------+-------------------------------------------------------------------------------------------+
| -c      | Correspondence   | Extract event-related genomic alignment                                                   |
+---------+------------------+-------------------------------------------------------------------------------------------+
| -bk     | BlockKs          | Show Ks of blocks in a dotplot                                                            |
+---------+------------------+-------------------------------------------------------------------------------------------+
| -kp     | KsPeaks          | A simple way to get ks peaks                                                              |
+---------+------------------+-------------------------------------------------------------------------------------------+
| -pf     | PeaksFit         | Gaussian fitting of ks distribution                                                       |
+---------+------------------+-------------------------------------------------------------------------------------------+
| -a      | Alignment        | Show event-related genomic alignment in a dotplot                                         |
+---------+------------------+-------------------------------------------------------------------------------------------+
| -at     | AlignmentTrees   | Phylogenetic trees constructed by collinear genes                                         |
+---------+------------------+-------------------------------------------------------------------------------------------+
| -p      | P-index          | Polyploidy-index characterize the degree of divergence among subgenomes of a polyploidy   |
+---------+------------------+-------------------------------------------------------------------------------------------+
| -r      | Retain           | Show subgenomes in gene retention or genome fractionation                                 |
+---------+------------------+-------------------------------------------------------------------------------------------+
| -ci     | Circos           | A simple way to run circos                                                                |
+---------+------------------+-------------------------------------------------------------------------------------------+
| -conf   | Configure        | Display and modify the environment variable                                               |
+---------+------------------+-------------------------------------------------------------------------------------------+
