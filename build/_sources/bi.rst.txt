bi
-------

bi is collinearity and Ks speculate whole genome duplication.
  
.. rubric:: Parameters

Use command to enter the folder ``wgdi -bk ? > blockks.conf`` Take out the parameter file.::

   [b1ockinfo]
   blast = blast file
   gff1 = gffl file
   gff2 = gff2 file
   lens1 = lens1 file
   1ens2 = lens2 file
   colinearity = colinearity file
   score = 100
   evalue = 1e-5
   repnum = 30
   position = order
   ks = ks file
   ks_col = ka_ NG86
   savefile = block information (*.csv)

.. tabularcolumns:: column spec

================ ========================================================================
Parameters        Standards and instructions
---------------- ------------------------------------------------------------------------
colinearity       Type: str    Default: -
                     
					 Colinscan results file.
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
ks                Type: str    Default: -
                     
					 ks calculation results.
---------------- ------------------------------------------------------------------------
ks_col            Type: str    Default: -
---------------- ------------------------------------------------------------------------
savefile          Type: str    Default: \*.csv
                   
				     The resulting file.
================ ========================================================================

.. rubric:: Example

.. rubric:: Modify

Modify the parameters that are right for you to run.

.. rubric:: Begin

Use ``wgdi –bi blockinfo.conf`` to run the parameter file and output the results you want.

.. image :: _static/1.png
   :align: left