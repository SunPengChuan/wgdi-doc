Polyploid classification
------------------------

Polyploid distinguish among subgenomes.

 
.. rubric:: Parameters

.. tabularcolumns:: column spec

==================== ========================================================================
Parameters           Standards and instructions
-------------------- ------------------------------------------------------------------------
blockinfo            Type: **file**  |    Default: **-**
                     
                     Output result of parameter `bi`
-------------------- ------------------------------------------------------------------------
ancestor_left        Type: **file**  |  Default: **none**

                     The ancestral chromosome region of the species on the left of dotplot.
-------------------- ------------------------------------------------------------------------  
ancestor_top         Type: **file**  |  Default: **none**

                     The ancestral chromosome region of the species on the top of dotplot.
-------------------- ------------------------------------------------------------------------
diff                 Type: **float** |  Default: **0.05**

                     More than this value is considered a significant difference.
-------------------- ------------------------------------------------------------------------
classid              Type: **str**  |    Default: **class1,class2**

                     The class name of the grouping according to the divided ancestral area.
-------------------- ------------------------------------------------------------------------
same_protochromosome Type: **bool**  |    Default: **False**

                     A synteny block spans two protochromosomes of the same color.
-------------------- ------------------------------------------------------------------------
savefile             Type: **file**   |  Default: \* **.csv**
                     
                     The resulting file.
==================== ========================================================================

Use command to enter the folder ``wgdi -pc ? >> total.conf`` Take out the parameter file.

.. code-block:: python

    [polyploidy classification]
    blockinfo = block information (*.csv)
    ancestor_left = file
    ancestor_top = file
    diff = 0.05
    classid = class1,class2
    same_protochromosome =  False
    savefile = result file(.csv)



.. rubric:: Quick start


The original results are easily accessible at `wgdi-example <https://github.com/SunPengChuan/wgdi-example>`_
