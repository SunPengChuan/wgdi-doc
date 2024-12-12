Fusions_detection
-----------------

Extract the fusion positions dataset. 

 
.. rubric:: Parameters

.. tabularcolumns:: column spec

========================= ========================================================================
Parameters                Standards and instructions
------------------------- ------------------------------------------------------------------------
blockinfo                 Type: **file**  |    Default: **none**
                     
                          Output result of parameter `bi`.
------------------------- ------------------------------------------------------------------------
ancestor                  Type: **file**  |  Default: **none**

                          Ancestor location file.
------------------------- ------------------------------------------------------------------------
min_genes_per_side        Type: **int**  |  Default: **5**

                          The number of genes spanned by a synteny block on both sides of a breakpoint.
------------------------- ------------------------------------------------------------------------
density                   Type: **float**  |  Default: **0.3**

                          Synteny block density relative to the protochromosome indicates collinearity; values near 1 signify greater clarity.
------------------------- ------------------------------------------------------------------------
filtered_blockinfo        Type: **file**  |    Default: **none**

                          blockinfo.csv filtered by this program.
========================= ========================================================================

Use command to enter the folder ``wgdi -fd ? >> total.conf`` Take out the parameter file.

.. code-block:: python

    [fusions_detection]
    blockinfo = block information (*.csv)
    ancestor = ancestor file
    min_genes_per_side = 5
    density = 0.3
    filtered_blockinfo = result blockinfo (.csv)


.. rubric:: Quick start


The original results are easily accessible at `wgdi-example <https://github.com/SunPengChuan/wgdi-example>`_
