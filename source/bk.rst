blockks
-------

blockks is show Ks of blocks in a dotplot.
  
.. rubric:: Parameters

Use command to enter the folder ``wgdi -bk ? > blockks.conf`` Take out the parameter file.::

   [blockks]
   blast = blast file
   gff1 = gff1 file
   gff2 = gff2 file
   lens1 = lens1 file
   lens2 = lens2 file
   genome1_ name = Genome1 name
   genome2_ name = Genome2 name
   colinearity = colinearity(colinearscan,mcscanx)
   ks= ks file
   markersize = 1
   area = 0,1
   block_length = int number
   position = order
   figsize = 10,10 
   savefile = savefile(.png,.pdf)

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
                     
					 Shows the minimum length of a collinear block.
---------------- ------------------------------------------------------------------------
position          Type: str    Default: order
                     
					 The position of the gene corresponds to the gff file.
---------------- ------------------------------------------------------------------------
figsize           Type: int,int    Default: 10,10
				  
                     Controls the proportion of the size of the saved picture.
---------------- ------------------------------------------------------------------------
savefile          Type: {\*.png, \*.pdf}    Default: \*.png
                     
					 Save pictures support png, PDF formats.
================ ========================================================================

.. rubric:: Example


.. rubric:: Modify

Modify the parameters that are right for you to run.

.. rubric:: Begin

Use ``wgdi –bk blockks.conf`` to run the parameter file and output the results you want.

.. image :: _static/1.png
   :align: left