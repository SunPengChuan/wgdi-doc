karyotype_mapping
-----------------

Quickly find shared fusions between species. 

 
.. rubric:: Parameters

.. tabularcolumns:: column spec

========================= ========================================================================
Parameters                Standards and instructions
------------------------- ------------------------------------------------------------------------
blockinfo                 Type: **file**  |    Default: **-**
                     
                          blockinfo.csv filtered according to certain conditions '-c'
------------------------- ------------------------------------------------------------------------
lens1                     Type: **file**  |  Default: **none**

                          Lens file and  new lens file created by this program.
------------------------- ------------------------------------------------------------------------
lens2                     Type: **file**  |  Default: **none**

                          Lens file and  new lens file created by this program.
------------------------- ------------------------------------------------------------------------
ancestor_left             Type: **file**  |  Default: **none**

                          Ancestor location file.
------------------------- ------------------------------------------------------------------------
ancestor_top              Type: **file**  |  Default: **none**

                          Ancestor location file.
------------------------- ------------------------------------------------------------------------
classid                   Type: **str**  |    Default: **class1,class2**

                          The class name of the grouping according to the divided ancestral area.
------------------------- ------------------------------------------------------------------------
limit_length              Type: **int**  |    Default: **5**
      
                          Show the minimum length of blocks.
------------------------- ------------------------------------------------------------------------
savefile                  Type: **file**   |  Default: \* **.csv**
                    
                          The resulting file.
------------------------- ------------------------------------------------------------------------
filtered_blockinfo        Type: **file**   |  Default: \* **.csv**
                    
                          blockinfo.csv filtered by this program.
========================= ========================================================================

Use command to enter the folder ``wgdi -sf ? >> total.conf`` Take out the parameter file.

.. code-block:: python

    [shared_fusion]
    blockinfo = block information (*.csv)
    lens1 = lens file, new lens file
    lens2 =  lens file,  new lens file
    ancestor_left = ancestor file
    ancestor_top = ancestor file
    classid = class1,class2
    limit_length = 10
    savefile = result file(.csv)
    filtered_blockinfo = result blockinfo (.csv)

.. rubric:: Quick start


The original results are easily accessible at `wgdi-example <https://github.com/SunPengChuan/wgdi-example>`_
