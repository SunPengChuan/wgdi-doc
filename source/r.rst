retain
------

retain is show subgenomes in gene retention or genome fractionation.

.. rubric:: Parameters

Use command to enter the folder ``wgdi -r ? > retain.conf`` Take out the parameter file.::

   [retain]
   alignment = alignment file
   gff = gff file
   colors = red,blue,green
   refgenome = shorthand
   figsize = 10,12
   step = 50
   ylabel = y label
   savefile = retain file(result)
   figurefile = result(.png,.pdf)

.. tabularcolumns:: column spec

================ ========================================================================
Parameters        Standards and instructions
---------------- ------------------------------------------------------------------------
alignment         Type:str     Default: - 
                     
					 Colinear List.
---------------- ------------------------------------------------------------------------
colors            Type:{red,blue,green}     Default:-
                  
				     Set multiple sets of colors based on grouping, split with a comma.
---------------- ------------------------------------------------------------------------
refgenome         Type:str     Default: - 
                  
				     A short handbook of reference species.
---------------- ------------------------------------------------------------------------	  
figsize           Type:str     Default: - 
                  
				     The size ratio of the image.
---------------- ------------------------------------------------------------------------	  
step              Type:int     Default: - 
                  
				     The size of the sliding window.
---------------- ------------------------------------------------------------------------	  
ylabel            Type:str     Default: - 
                     
					 The y-axis label of the picture.
---------------- ------------------------------------------------------------------------	  
savefile          Type:str     Default: -  
                  
				     Results of the drawing.
---------------- ------------------------------------------------------------------------	  
figurefile        Type:{\*.png, \*.pdf}     Default: \*.png 
                  
				     Save pictures support png, PDF formats.
================ ========================================================================

.. rubric:: Example

.. rubric:: Modify

Modify the parameters that are right for you to run.

.. rubric:: Begin

Use ``wgdi -r retain.conf`` to run the parameter file and output the results you want.

.. image :: _static/1.png
   :align: left