colinearscan
------------

colinearscan is a simple way to run ColinearScan.
   
.. rubric:: Parameters

Use command to enter the folder ``wgdi -cl ? > colinearscan.conf`` Take out the parameter file.::

   [colinearscan]
   gff1 = gff1 file
   gff2= gff2 file
   lens1 = lens1 file
   lens2 = lens2 file
   blast = blast file
   dir = Output file
   evalue = 1e-5
   score = 100
   mg = 50,50
   repnum = 20
   positon = order

.. tabularcolumns:: column spec

================ ========================================================================
Parameters        Standards and instructions
---------------- ------------------------------------------------------------------------
dir               Type: str    Default: -
              
                     The directory of the generated file.
---------------- ------------------------------------------------------------------------ 
evalue            Type: float    Default: 1e-5

                     evalue value in blast result.
---------------- ------------------------------------------------------------------------         
score             Type: int    Default: 100
				  
                     Score value in blast results.
---------------- ------------------------------------------------------------------------  
mg                Type: int,int    Default: 50,50

                     This is the parameter of the colinearscan program mg.
---------------- ------------------------------------------------------------------------ 
repnum            Type: int    Default: 20
				  
                     The maximum number of homologous genes is allowed 
				  
				  to be removed more than part of the population.
---------------- ------------------------------------------------------------------------ 				  
position          Type: {start,order,end}    Default: order

                     The position of the gene corresponds to the gff file.
================ ========================================================================

.. rubric:: Example

.. rubric:: Modify

Modify the parameters that are right for you to run.

.. rubric:: Begin

Use ``wgdi -cl colinearscan.conf`` to run the parameter file and output the results you want.

.. image :: _static/1.png
   :align: left