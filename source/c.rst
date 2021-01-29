correspondence
--------------

correspondence is extract event-related genomic alignment.

.. rubric:: Parameters

Use command to enter the folder ``wgdi -c ? > correspondence.conf`` Take out the parameter file.::

   [correspondence]
   blockinfo = blockinfo file(.csv)
   lens1 = lens1 file
   lens2 = lens2 file
   tandem = (true/false)
   pvalue = 0.05
   block_length = 5
   multiple = 1
   homo = 0,1
   savefile = savefile(.csv) 

.. tabularcolumns:: column spec

================ ========================================================================
Parameters        Standards and instructions
---------------- ------------------------------------------------------------------------
blockinfo         Type: str     Default:- 
                     
					 Integrate collinear and ks files.
---------------- ------------------------------------------------------------------------
tandem            Type: {true,false}     Default: true
                     
					 The criterion is that there are no more than 200 genes 
				  
				  with a difference in genetic location.
---------------- ------------------------------------------------------------------------
pvalue            Type: **float**  |    Default: **1**

                  Evaluate the compactness and uniqueness of collinear blocks, the range is 0-1, the better collinearity range is 0-0.2.
---------------- ------------------------------------------------------------------------ 
block_length      Type: str     Default: int number 
                  
				     Minimum length of collinear blocks.
---------------- ------------------------------------------------------------------------
multiple          Type: str     Default: 1
                  
				     The optimal number of homologous genes.
---------------- ------------------------------------------------------------------------
homo             Type: **int [1-5]**   Default: **1**

                 Evaluate the ratio of the best homologous gene pairs of collinearity block, with a range of -1, 1.
---------------- ------------------------------------------------------------------------
savefile          Type: \*.csv     Default: \*.csv 
                         
				     Save pictures support csv formats.
================ ========================================================================

.. rubric:: Example

.. rubric:: Modify

Modify the parameters that are right for you to run.

.. rubric:: Begin

Use ``wgdi –c correspondence.conf`` to run the parameter file and output the results you want.

.. image :: _static/1.png
   :align: left