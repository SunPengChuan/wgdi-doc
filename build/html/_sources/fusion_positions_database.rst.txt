Fusion_positions_database
-------------------------

Determine whether these fusion events occur in other genomes.

 
.. rubric:: Parameters

.. tabularcolumns:: column spec

========================= ========================================================================
Parameters                Standards and instructions
------------------------- ------------------------------------------------------------------------
pep                       Type: **file**  |    Default: **-**
                     
                          A protein file for a genome.
------------------------- ------------------------------------------------------------------------
fusion_positions          Type: **file**  |  Default: **none**

                          See https://wgdi.readthedocs.io/en/latest/usage.html.
------------------------- ------------------------------------------------------------------------
NumGeneSetsPerSide        Type: **int**  |  Default: **100**

                          The number of genes within a single synteny block that spans across both sides of the fusion breakpoints.
------------------------- ------------------------------------------------------------------------
ancestor_left             Type: **file**  |  Default: **none**

                          Result file.
------------------------- ------------------------------------------------------------------------
ancestor_lens             Type: **file**  |  Default: **none**

                          Result file.
------------------------- ------------------------------------------------------------------------
ancestor_pep              Type: **file**  |    Default: **none**

                          Result file.
------------------------- ------------------------------------------------------------------------
ancestor_file             Type: **file**  |    Default: **none**
      
                          Result file.
========================= ========================================================================

Use command to enter the folder ``wgdi -fpd ? >> total.conf`` Take out the parameter file.

.. code-block:: python

    [fusion_positions_database]
    pep = pep file
    gff = gff file
    fusion_positions = fusion_positions file
    NumGeneSetsPerSide = 100
    ancestor_gff =  result file
    ancestor_lens =  result file
    ancestor_pep =  result file
    ancestor_file =  result file


.. rubric:: Quick start


The original results are easily accessible at `wgdi-example <https://github.com/SunPengChuan/wgdi-example>`_
