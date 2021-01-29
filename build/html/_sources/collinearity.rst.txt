Improved collinearity
---------------------

colinearscan is a simple way to run ColinearScan.
   
.. rubric:: Parameters

.. tabularcolumns:: column spec

================ ========================================================================
Parameters        Standards and instructions
---------------- ------------------------------------------------------------------------
dir               Type: str    Default: -
              
                  The directory of the generated file.
---------------- ------------------------------------------------------------------------ 
evalue            Type: float    Default: 1e-5

                  Evalue in the blast result.
---------------- ------------------------------------------------------------------------         
score             Type: int    Default: 100
				  
                     Score value in the blast results.
---------------- ------------------------------------------------------------------------  
mg                Type: int,int    Default: 50,50

				The maximum clearance length (mg) is an important parameter for detecting collinear regions.
---------------- ------------------------------------------------------------------------ 
repeat_number            Type: int    Default: 20
				  
                     The maximum number of homologous genes is allowed 
				  
				  to be removed more than part of the population.
---------------- ------------------------------------------------------------------------ 				  
position          Type: {start,order,end}    Default: order

                     The position of the gene corresponds to the gff file.
================ ========================================================================

Use command to enter the folder ``wgdi -icl ? >> total.conf`` Take out the parameter file.

.. code-block:: python

   [collinearity]
   gff1 = gff1 file
   gff2 = gff2 file
   lens1 = lens1 file
   lens2 = lens2 file
   blast = blast file
   blast_reverse = false
   multiple  = 1
   process = 8
   evalue = 1e-5
   score = 100
   grading = 50,40,25
   mg = 40,40
   pvalue = 0.2
   repeat_number = 10
   positon = order
   savefile = collinearity file


.. rubric:: Quick start

After the parameters are modified properly, then run ``wgdi -icl total.conf`` 

.. rubric:: Example

The original results are easily accessible at `wgdi-example <https://github.com/SunPengChuan/wgdi-example>`_

.. image :: _static/collinearity.png
   :align: left