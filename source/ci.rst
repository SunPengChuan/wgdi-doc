circos
------

circos is a simple way to run circos.

.. rubric:: Parameters

Use command to enter the folder ``wgdi -ci ? > circos.conf`` Take out the parameter file.::

   [circos]
   gff =  gff file
   lens = lens file
   radius = 0.2
   angle_gap = 0.05
   ring_width= 0.015
   colors  = color confige(chr:color,chr:color)
   position = end
   alignment = text.txt
   chr_label = Shorthand
   figsize = 10,10
   savefig = saving image(.png,.pdf)

.. tabularcolumns:: column spec

================ ========================================================================
Parameters        Standards and instructions
---------------- ------------------------------------------------------------------------
radius            Type: float    Default: 0.2
                     
					 Radius, value between 0-1.
---------------- ------------------------------------------------------------------------
angle_gap         Type: float    Default: 0.05
                     
					 Gap between chromosomes.
---------------- ------------------------------------------------------------------------
ring_width        Type: float    Default: 0.015
                     
					 The width of the ring.
---------------- ------------------------------------------------------------------------
colors            Type: str    Default: -
                     
					 Set multiple sets of colors based on grouping, split with a comma.
---------------- ------------------------------------------------------------------------
position          Type: {start,order,end}    Default: order

                     The position of the gene corresponds to the gff file.
---------------- ------------------------------------------------------------------------
alignment         Type: str    Default: -
                     
					 Colinear List.
---------------- ------------------------------------------------------------------------
chr_label         Type: str    Default: Shorthand
                     
					 A shorthand for chromosomes.
---------------- ------------------------------------------------------------------------
figsize           Type: int,int    Default: 10,10
                     
					 The size ratio of the image.
---------------- ------------------------------------------------------------------------
savefile          Type: {\*.png, \*.pdf}    Default: \*.png

                     Save pictures support png, PDF formats.
================ ========================================================================

.. rubric:: Example

.. rubric:: Modify

Modify the parameters that are right for you to run.

.. rubric:: Begin

Use `wgdi –ci circos.conf` to run the parameter file and output the results you want.

.. image :: _static/1.png
   :align: left