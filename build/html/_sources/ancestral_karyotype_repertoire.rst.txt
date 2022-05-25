ancestral_karyotype_repertoire
------------------------------

Incorporate genes from collinearity blocks into the ancestral karyotype repertoire. 

 
.. rubric:: Parameters

.. tabularcolumns:: column spec

========================= ========================================================================
Parameters                Standards and instructions
------------------------- ------------------------------------------------------------------------
blockinfo                 Type: **file**  |    Default: **-**
                     
                          Output result of parameter `-bi` and `-c`.
------------------------- ------------------------------------------------------------------------
blockinfo_reverse         Type: **bool**   |    Default: **false**

                          The two species aligned swap positions.
------------------------- ------------------------------------------------------------------------
gff1                      Type: **file**  |      Default: **-**
 
                          Cat the relevant 'gff' files into a file.
------------------------- ------------------------------------------------------------------------
gff2                      Type: **file**  |      Default: **-**
 
                          Cat the relevant 'gff' files into a file.
------------------------- ------------------------------------------------------------------------
gap                       type: **int**  |   Default: **5**
                  
                          Minimum number of genes bounded by collinear genes corresponds to two ordered protogenes.
------------------------- ------------------------------------------------------------------------
ancestor                  Type: **file**  |  Default: **none**

                          This file requires you to provide.
------------------------- ------------------------------------------------------------------------
ancestor_new              Type: **file**  |  Default: **none**

                          Updated the ancestor file of ancestral karyotype..
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
ancestor_pep_new          Type: **file**  |    Default: **-**
      
                          Updated the pep file of ancestral karyotype.
========================= ========================================================================

Use command to enter the folder ``wgdi -ak ? >> total.conf`` Take out the parameter file.

.. code-block:: python

    [ancestral_karyotype_repertoire]
    blockinfo =  block information (*.csv)
    # blockinfo: processed *.csv
    blockinfo_reverse = False
    gff1 =  gff1 file (*.gff)
    gff2 =  gff2 file (*.gff)
    gap = 5
    mark = aak1s
    ancestor = ancestor file
    ancestor_new =  result file
    ancestor_pep =  ancestor pep file
    ancestor_pep_new =  result file
    ancestor_gff =  result file
    ancestor_lens =  result file


.. rubric:: Quick start


The original results are easily accessible at `wgdi-example <https://github.com/SunPengChuan/wgdi-example>`_
