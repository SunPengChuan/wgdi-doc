Alignmenttrees
--------------

Phylogenetic tree construction using alignment or collinear genes.
A phylogenetic tree is constructed for gene sets that each row of the alignment file during this process. By using ASTRAL merge, you can obtain a multispecies or subgenomes coalescent tree.

.. rubric:: Parameters


.. tabularcolumns:: column spec

================ ========================================================================
Parameters       Standards and instructions
---------------- ------------------------------------------------------------------------
alignment        Type: **file**  |      Default: **-**

                 The merged file of multiple alignment files with the same reference.
---------------- ------------------------------------------------------------------------
gff              Type: **file**  |      Default: **-**
 
                 Gff of reference, If alignment has no reference species, delete it.
---------------- ------------------------------------------------------------------------
lens             Type: **file**  |    Default: **-**
                  
                 lens of reference, If alignment has no reference species, delete it.
---------------- ------------------------------------------------------------------------  
dir              Type: **folder** |  Default: **-**

                 Folder for phylogenetic trees.
---------------- ------------------------------------------------------------------------  
sequence_file    Type: **file**  |    Default: **-**
                  
                 In general, it is protein sequences (pep), if it is coding sequences (cds), cds_file need to be deleted.
---------------- ------------------------------------------------------------------------  
cds_file         Type: **file**   | Default: **none**

                 It is required when the method of constructing trees involvesv codon. Otherwise, it can be discarded.
---------------- ------------------------------------------------------------------------
codon_positon    Type:**str**  |      Default: **1,2,3**
                  
                 1,2 mean codon1&2; 1,2,3 mean no codon removed.
---------------- ------------------------------------------------------------------------
trees_file       Type: **file**  |    Default: **-**
                  
                 Merge multiple nwk-format tree files.
---------------- ------------------------------------------------------------------------  
align_software   Type:{ **muscle**, **mafft** }  |   Default: **muscle**

                 Software of multiple sequence alignment.
---------------- ------------------------------------------------------------------------
tree_software    Type:{ **iqtree**, **fasttree** }  |   Default: **iqtree**

                 Software of constructing phylogenetic trees.
---------------- ------------------------------------------------------------------------  
model            Type: **str**  |    Default: **-**
                  
                 Merge multiple nwk-format tree files.
---------------- ------------------------------------------------------------------------  
trimming         Type:{ **trimal**, **divvier**}  |   Default: **trimal**

                 Software of removal of spurious sequences.
---------------- ------------------------------------------------------------------------
minimum          Type: **int**  |   Default: **4**

                 Minimum number of gene sets in constructing phylogenetic tree.
---------------- ------------------------------------------------------------------------  
delete_detail    Type: **bool**   |    Default: **false**

                 Whether or not to keep intermediate files when constructing phylogenetic tree.
================ ========================================================================


Use command to enter the folder ``wgdi -at ? >> total.conf`` Take out the parameter file.
Afterwards, use the ASTRAL command ``java -jar /path/astral.5.7.7.jar -i trees_file.nwk -o out.tre -t 8``, you can obtain a multispecies or subgenomes coalescent tree.

.. code-block:: python

   [alignmenttrees]
   alignment = alignment file (.csv)
   gff = gff file (reference genome, If alignment has no reference species, delete it)
   lens = lens file (If alignment has no reference species, delete it)
   dir = output folder
   sequence_file = sequence file (.fa)
   cds_file = cds file (.fa)
   codon_positon = 1,2,3  (1,2 mean codon1&2; 1,2,3 mean no codon removed)
   trees_file =  trees (.nwk)
   align_software = mafft
   tree_software =  (iqtree,fasttree)
   model = MFP
   trimming =  trimal
   minimum = 4
   delete_detail = true


.. rubric:: Quick start

After the parameters are modified properly, then run ``wgdi -at total.conf`` 


.. rubric:: Example

The original results are easily accessible at `wgdi-example <https://github.com/SunPengChuan/wgdi-example>`_
