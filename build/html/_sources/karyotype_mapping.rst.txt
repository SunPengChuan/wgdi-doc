karyotype_mapping
-----------------

Mapping from the known karyotype result to this species. 

 
.. rubric:: Parameters

.. tabularcolumns:: column spec

========================= ========================================================================
Parameters                Standards and instructions
------------------------- ------------------------------------------------------------------------
blast_reverse             Type: **bool**   |    Default: **false**

                          The first two columns of the blast result swap positions.
------------------------- ------------------------------------------------------------------------
score                     Type: **int**    |     Default: **100**

                          Score value in blast result.
------------------------- ------------------------------------------------------------------------
evalue                    Type: **float**  |  Default: **1e-5**

                          Evalue value in blast result.
------------------------- ------------------------------------------------------------------------
repeat_number             Type: **int**  |  Default: **10**

                          The maximum number of homologous genes is allowed to remove more than part of the population.
------------------------- ------------------------------------------------------------------------
ancestor_left             Type: **file**  |  Default: **none**

                          Ancestor location file (Only one of ('left', 'top') can be reserved)
------------------------- ------------------------------------------------------------------------  
ancestor_top              Type: **file**  |  Default: **none**

                          Ancestor location file (Only one of ('left', 'top') can be reserved)
------------------------- ------------------------------------------------------------------------  
blockinfo                 Type: **file**  |    Default: **-**
                     
                          blockinfo.csv filtered according to certain conditions '-c'
------------------------- ------------------------------------------------------------------------ 
the_other_lens            Type: **file**  |    Default: **-**
      
                          The lens file for the species for which you want to generate ancestor files.
------------------------- ------------------------------------------------------------------------ 
limit_length              Type: **int**  |    Default: **5**
      
                          Show the minimum length of blocks.
------------------------- ------------------------------------------------------------------------ 
the_other_ancestor_file   Type: **file**   |  Default: \* **.csv**
                    
                          The resulting file.
========================= ========================================================================

Use command to enter the folder ``wgdi -k ? >> total.conf`` Take out the parameter file.

.. code-block:: python

    [karyotype_mapping]
    blast = blast file
    blast_reverse = false
    gff1 = gff1 file
    gff2 = gff2 file
    score = 100
    evalue = 1e-5
    repeat_number = 5
    ancestor_left = ancestor location file (Only one of ('left', 'top') can be reserved)
    ancestor_top = ancestor location file
    the_other_lens = the other lens file
    blockinfo = block information (*.csv)
    blockinfo_reverse = false
    limit_length = 5
    the_other_ancestor_file =  result file



.. rubric:: Quick start


The original results are easily accessible at `wgdi-example <https://github.com/SunPengChuan/wgdi-example>`_
