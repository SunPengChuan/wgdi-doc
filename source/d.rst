dotplot
-------

dotplot is show homologous gene dotplot.
  
.. rubric:: Parameters

Use command to enter the folder ``wgdi -d ? > dotplot.conf`` Take out the parameter file.::

   [dotplot]
   blast= blast file
   gffl = gff1 file
   gff2 = gfi2 file
   lens1 = lens1 file
   lens2 = lens2 file
   genome1_ name =  Genome1 name
   genome2_ name =  Genome2 name
   multiple  = 1
   score = 100
   evalue = 1e-5
   repnum = 20
   position = order
   markersize = 0.5
   figsize = 10,10
   savefile = savefile(. png, .pdf)

.. tabularcolumns:: column spec

================ ========================================================================
Parameters        Standards and instructions
---------------- ------------------------------------------------------------------------
multiple          Type: int    Default: 1
              
                     The best number of homologous genes.
---------------- ------------------------------------------------------------------------         
score             Type: int    Default: 100
				  
                     Score value in blast results.
---------------- ------------------------------------------------------------------------
evalue            Type: float    Default: 1e-5

                     evalue value in blast result.
---------------- ------------------------------------------------------------------------   
repnum            Type: int    Default: 20
				  
                     The maximum number of homologous genes is allowed 
				  
				  to be removed more than part of the population.
---------------- ------------------------------------------------------------------------  
position          Type: {start,order,end}    Default: order

                     The position of the gene corresponds to the gff file.
---------------- ------------------------------------------------------------------------   
markersiz         Type: float    Default: 0.5
  
                     The size of the point in the plot.
---------------- ------------------------------------------------------------------------
figsize           Type: int,int    Default: 10,10
				  
                     Controls the proportion of the size of the saved picture.
---------------- ------------------------------------------------------------------------  
savefile          Type: {\*.png,\*.pdf}    Default: \*.png

                     Save pictures support png, PDF, svg formats.
================ ========================================================================

.. rubric:: Example

.. rubric:: Modify

Modify the parameters that are right for you to run.

.. rubric:: Begin

Use ``wgdi -d dotplot.conf`` to run the parameter file and output the results you want.

.. image :: _static/1.png
   :align: left