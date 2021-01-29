Dotplot
-------

Dotplot is show homologous gene dotplot.

  
.. rubric:: Parameters

.. tabularcolumns:: column spec

================ ========================================================================
Parameters       Standards and instructions
---------------- ------------------------------------------------------------------------
blast_reverse    Type: **bool**   |    Default: **false**

                 The first two columns of the blast result swap positions.
---------------- ------------------------------------------------------------------------
multiple         Type: **int**   |    Default: **1**

                 The best number of homologous genes shown with red dots.
---------------- ------------------------------------------------------------------------         
score            Type: **int**    |     Default: **100**

                 Score value in the blast results.
---------------- ------------------------------------------------------------------------
evalue           Type: **float**  |  Default: **1e-5**

                 Evalue value in blast result.
---------------- ------------------------------------------------------------------------   
repeat_number    Type: **int**  |  Default: **10**

                 Restriction of gene number relative to another genome.
---------------- ------------------------------------------------------------------------  
position         Type: {**order**, **start** , **end** }  |  Default: **order**

                 The position of the gene corresponds to the gff file.
---------------- ------------------------------------------------------------------------  
ancestor_left    Type: **file**  |  Default: **none**

                 The ancestral chromosome region of the species on the left of dotplot.
---------------- ------------------------------------------------------------------------  
ancestor_top     Type: **file**  |  Default: **none**

                 The ancestral chromosome region of the species on the top of dotplot.
---------------- ------------------------------------------------------------------------   
markersize       Type: **float**   | Default: **0.5**

                 The size of the point in the plot.
---------------- ------------------------------------------------------------------------
figsize          Type: **int,int** |  Default: **10,10**

                 Control the proportion of the size of the saved picture.
---------------- ------------------------------------------------------------------------  
savefile         Type: {\*. **png**,\*. **pdf**}  |  Default: \*. **png**

                 Save pictures support png, pdf, svg formats.
================ ========================================================================

Use command to enter the folder ``wgdi -d help >> total.conf`` Take out the parameter file.

.. code-block:: python

   [dotplot]
   blast = blast file
   blast_reverse = false
   gff1 =  gff1 file
   gff2 =  gff2 file
   lens1 = lens1 file
   lens2 = lens2 file
   genome1_name =  Genome1 name
   genome2_name =  Genome2 name
   multiple  = 1
   score = 100
   evalue = 1e-5
   repeat_number = 10
   position = order
   ancestor_left = none
   ancestor_top = none
   markersize = 0.5
   figsize = 10,10
   savefig = savefile(.png,.pdf)

.. rubric:: Quick start

After the parameters are modified properly, then run ``wgdi -d total.conf`` 


.. rubric:: Example

The original results are easily accessible at `wgdi-example <https://github.com/SunPengChuan/wgdi-example>`_

.. image :: _static/vvi161s_vvi161s.dotplot.order.png
   :align: left

.. image :: _static/vvi161s_vvi161s.dotplot.end.png
   :align: left