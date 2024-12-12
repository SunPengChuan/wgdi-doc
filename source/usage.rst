Usage
-----
  
We support the use of **WGDI** to complete the work on the icon number.

.. toctree::

   dotplot
   collinearity
   ks
   blockinfo
   correspondence
   blockks
   kspeaks
   peaksfit
   ksfigure
   polyploidy_classification
   ancestral_karyotype
   ancestral_karyotype_repertoire
   karyotype_mapping
   karyotype
   shared_fusions
   fusion_positions_database
   fusion_detetion
   alignment
   alignment_tree
   retain
   pindex
   circos
   
**Common file**


* conf

The conf file contains parameters required for the corresponding operation, which are read when WGDI is performed.
Using ``wgdi -* ? > *.conf`` to get the configuration file in the current directory and modify it to run.
If you don't know which files are needed, you can view it through ``wgdi -* ?`` or ``wgdi -* help``  or ``wgdi -* example``. These three commands are equivalent.

In conf file: **gff1** , **lens1** , **genome1_name** and **gff2**,  **lens2**, **genome2_name** represent the files of species 1 and 2 respectively. 
We will no longer explain these in this documentation.

* gff

.. tabularcolumns:: column spec

====== ============ ======================================================
Column Information  Explanation
1      Chr          Chromosome number 
2      Id           Gene name
3      Strat        The starting location of a gene 
4      End          The ending location of a  gene
5      Direction    Direction of a gene sequence
6      Order        Order of each chromosome, starting from 1
7      Original     Original id and  not read
====== ============ ======================================================

* lens

.. tabularcolumns:: column spec

========= =========== =========================================
Column    Information Explanation                   
1         Chr         Chromosome number
2         Length      Length of chromosome sequences
3         Number      Number of chromosome genes      
========= =========== =========================================

*  blast

The protein-coding genes from each genome were compared against itself and other genomes using `BLASTP <ftp://ftp.ncbi.nlm.nih.gov/blast/executables/LATEST/>`_  (e-value < 10-5, and outfmt = 6) or other similar protein sequence searching software ( `MMseqs2 <https://github.com/soedinglab/MMseqs2>`_ , `DIAMOND <https://github.com/bbuchfink/diamond>`_ ).

* ancestor file

Required documents for karyotype evolution analysis

.. tabularcolumns:: column spec

========= =========== =============================================================
Column    Information Explanation                   
1         Chr         Chromosome number
2         Start       Homologous regions of these protochromosomes in this genome
3         End         Homologous regions of these protochromosomes in this genome
4         Color       These protochromosomes with different colors
5         Subgenomes  Subgenomes according to protochromosomes
========= =========== =============================================================

* Fusino postions file

Required documents for shared fusion events

.. tabularcolumns:: column spec

========= =========== ===============================================================================
Column    Information Explanation                   
1         Chr         Chromosome number
2         Breakpoint  The breakpoints of fusions, with multiple breakpoints listed on separate lines.
3         Mark        The unique marks of unique fusions
========= =========== ===============================================================================

**Tips**

* You can use ``wgdi -conf ? > total.conf`` generates a **total.conf** file with all parameters, and when you modify the parameters and run WGDI, WGDI will only read the parameters corresponding to the total.conf file to execute your command.

* When a folder runs WGDI, WGDI automatically generates results for you in the background, and you can exit the folder and go to the next folder to start working.

* WGDI performs the **conf** file for the current folder, so you can copy the **conf** file in bulk and make parameter modifications appied to the target folder.
