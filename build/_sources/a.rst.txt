align
-----

align is show event-related genomic alignment in a dotplot.

.. rubric:: Parameters

Use command to enter the folder ``wgdi -a ? > align.conf`` Take out the parameter file.::

   [alignment]
   gff1 =  gff1 file
   gff2 =  gff2 file
   lens1 = lens1 file
   lens2 = lens2 file
   genome1_ name =  Genome1 name
   genome2_ name =  Genome2 name
   markersize = 0.5
   position = order
   colors = red,blue,green
   figsize = 10,10
   savefile = savefile(.csv)
   savefig= savefig(.png,.pdf)
   block_list = 1.txt
   blockinfo = block information file

.. tabularcolumns:: column spec

================ ========================================================================
Parameters        Standards and instructions
---------------- ------------------------------------------------------------------------
markersize        Type: str    Default: 0.5

                     The size of the control point.					 
---------------- ------------------------------------------------------------------------
position          Type: str    Default: order

                     The position of the gene corresponds to the gff file.
---------------- ------------------------------------------------------------------------
colors		      Type: {red,blue,green}    Default: red,blue,green
	 
                     Set multiple sets of colors based on grouping, split with a comma.
---------------- ------------------------------------------------------------------------
figsize           Type: int,int    Default: 10,10
				  
                     Controls the proportion of the size of the saved picture.
---------------- ------------------------------------------------------------------------
savefile          Type: str    Default: \*.csv

                     A resulting collinear list.
---------------- ------------------------------------------------------------------------
savefig           Type: {*.png,*.pdf}    Default: \*.png

                     Save pictures support png, PDF formats.
---------------- ------------------------------------------------------------------------
block_list        Type: str    Default: -

                     Add a class column to the blockinfo file to group and express 
					 
			      different groups with Raab numbers.     
---------------- ------------------------------------------------------------------------
blockinfo         Type:str     Default:- 
                     
					 Integrate collinear and ks files.
================ ========================================================================

.. rubric:: Example

.. rubric:: Modify

Modify the parameters that are right for you to run.

.. rubric:: Begin

Use ``wgdi -a align.conf`` to run the parameter file and output the results you want.

.. image :: _static/1.png
   :align: left