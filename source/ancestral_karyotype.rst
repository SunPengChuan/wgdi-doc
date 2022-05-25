ancestral_karyotype
-------------------

Generation of ancestral karyotypes from chromosomes that retain the same structure in modern species. 

 
.. rubric:: Parameters

.. tabularcolumns:: column spec

========================= ========================================================================
Parameters                Standards and instructions
------------------------- ------------------------------------------------------------------------
gff                       Type: **file**  |      Default: **-**
 
                          Cat the relevant 'gff' files into a file.
------------------------- ------------------------------------------------------------------------
pep_file                  Type: **file**    |     Default: **none**

                          Cat the relevant 'pep.fa' files into a file.
------------------------- ------------------------------------------------------------------------
ancestor                  Type: **file**  |  Default: **none**

                          This file requires you to provide.
------------------------- ------------------------------------------------------------------------
mark                      Type: **str**  |  Default: **aak**

                          A shorthand for ancestral karyotype.
------------------------- ------------------------------------------------------------------------
ancestor_gff              Type: **file**  |  Default: **none**
                          Gff file of the created ancestral karyotype.
------------------------- ------------------------------------------------------------------------  
ancestor_lens             Type: **file**  |  Default: **none**

                          Lens file of the created ancestral karyotype.
------------------------- ------------------------------------------------------------------------  
ancestor_pep              Type: **file**  |    Default: **-**
                     
                          Pep file of the created ancestral karyotype.
------------------------- ------------------------------------------------------------------------ 
ancestor_file             Type: **file**  |    Default: **-**
      
                          Updated the ancestral karyotype file.
========================= ========================================================================

Use command to enter the folder ``wgdi -ak ? >> total.conf`` Take out the parameter file.

.. code-block:: python

    [ancestral_karyotype]
    gff = gff file (cat the relevant 'gff' files into a file)
    pep_file = pep file (cat the relevant 'pep.fa' files into a file)
    ancestor = ancestor file  (this file requires you to provide)
    mark = aak
    ancestor_gff =  result file
    ancestor_lens =  result file
    ancestor_pep =  result file
    ancestor_file =  result file


.. rubric:: Quick start


The original results are easily accessible at `wgdi-example <https://github.com/SunPengChuan/wgdi-example>`_
