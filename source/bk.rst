blockks
-------

blockks is show Ks of blocks in a dotplot.
  
.. rubric:: Parameters

Use command to enter the folder ``wgdi -bk ? > blockks.conf`` Take out the parameter file.

.. code-block:: ruby

   [blockks]
   lens1 = lens1 file
   lens2 = lens2 file
   genome1_ name = Genome1 name
   genome2_ name = Genome2 name
   blockinfo = block information (*.csv)
   pvalue = 0.05
   tandem = true
   markersize = 1
   area = 0,1
   block_length = int number
   figsize = 10,10 
   savefile = save image(.png,.pdf,.svg)

.. tabularcolumns:: column spec

================ ========================================================================
Parameters        Standards and instructions
---------------- ------------------------------------------------------------------------
colinearity       Type: str    Default: -
                     
					 Colinscan results file.
---------------- ------------------------------------------------------------------------
ks                Type: str    Default: -
                     
					 ks calculation results.
---------------- ------------------------------------------------------------------------
markersize        Type: str    Default: 1
                     
					 The size of the control point.			 
---------------- ------------------------------------------------------------------------
area              Type: str    Default: 0,1
                     
					 Show the range of ks.
---------------- ------------------------------------------------------------------------
block_length      Type: str    Default: int number
                     
					 Show the minimum length of a collinear block.
---------------- ------------------------------------------------------------------------
position          Type: str    Default: order
                     
					 The position of the gene corresponds to the gff file.
---------------- ------------------------------------------------------------------------
figsize           Type: int,int    Default: 10,10
				  
                     Control the proportion of the size of the saved picture.
---------------- ------------------------------------------------------------------------
savefile          Type: {\*.png, \*.pdf,\*.svg}    Default: \*.png
                     
					 Save pictures support png, pdf，svg formats.
================ ========================================================================

.. rubric:: Example


.. rubric:: Modify

Modify the parameters that are right for you to run.

.. rubric:: Begin

Use ``wgdi –bk blockks.conf`` to run the parameter file and output the results you want.

.. image :: _static/1.png
   :align: left