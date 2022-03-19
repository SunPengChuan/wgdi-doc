Karyotype
---------

Show genome evolution from reconstructed ancestors.

 
.. rubric:: Parameters

.. tabularcolumns:: column spec

================ ========================================================================
Parameters        Standards and instructions
---------------- ------------------------------------------------------------------------
ancestor         Type: **file**  |    Default: **-**
                     
                 The specie's ancestral chromosome regions, result of parameter '-km'.
---------------- ------------------------------------------------------------------------
width            Type: **float** |  Default: **0.5**

                 The width of the chromosomes in the figure.
---------------- ------------------------------------------------------------------------
figsize          Type: **int,int** |  Default: **10,10**

                 Control the proportion of the size of the saved picture.
---------------- ------------------------------------------------------------------------ 
savefile         Type: **file**   |  Default: \* **.csv**
                    
                 The resulting file.
================ ========================================================================

Use command to enter the folder ``wgdi -k ? >> total.conf`` Take out the parameter file.

.. code-block:: python

    [karyotype]
    ancestor = ancestor chromosome file
    width = 0.5
    figsize = 10,6.18
    savefig = save image(.png, .pdf, .svg)



.. rubric:: Quick start


The original results are easily accessible at `wgdi-example <https://github.com/SunPengChuan/wgdi-example>`_

.. image :: _static/vvi161s.ancestor.svg
   :align: left