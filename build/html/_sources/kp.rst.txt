kspeaks
-------

kspeaks is a simple way to get ks peaks.
   
.. rubric:: Parameters

Use command to enter the folder ``wgdi -kp ? > kp.conf`` Take out the parameter file.::

  [kspeaks]

   blockinfo = block information (*.csv)
   pvalue = 0.05
   tandem = true
   block_ length = int number
   ks_area = 0,10
   multiple = 1
   homo = 0,1
   fontsize = 9
   area = 0,3
   figsize = 10,6.18
   savefig = saving image(.png,.pdf)
   savefile = ks medain savefile

.. tabularcolumns:: column spec

================ ========================================================================
Parameters        Standards and instructions
---------------- ------------------------------------------------------------------------
blockinfo         Type: str     Default: -
                     
					 Integrate collinear and ks files.
---------------- ------------------------------------------------------------------------
pvalue            Type:str     Default: 0.05 

                     P-value in collinear results.
---------------- ------------------------------------------------------------------------	  
tandem            Type:str     Default: true
                     
					 The criterion is that there are no more than 200 genes 
				  
				  with a difference in genetic location.
---------------- ------------------------------------------------------------------------	  
block_length      Type:str     Default: int number 
                  
				     Minimum length of collinear blocks.
---------------- ------------------------------------------------------------------------	  
ks_area           Type:str     Default: 0,10 
                     
					 Show the range of ks.
---------------- ------------------------------------------------------------------------	  
multiple          Type:str     Default: 1
                  
				     The optimal number of homologous genes.
---------------- ------------------------------------------------------------------------	  
homo              Type:str     Default: 0,1
                  
				     Collinear fragments favor the best matching values, 
					 
				  with a range of -1, 1.
---------------- ------------------------------------------------------------------------	  
fontsize          Type:str     Default: 9 
                      
				     The size of the font.
---------------- ------------------------------------------------------------------------	  
area              Type:str     Default: 0,3
                  
				     The extent of the drawing display.
---------------- ------------------------------------------------------------------------	  
figsize           Type:str     Default: 10,6.18
                  
				     The size ratio of the image
---------------- ------------------------------------------------------------------------	  
savefig           Type:{\*.png, \*.pdf}     Default: \*.png 
                     
					 Save pictures support png, PDF formats.
---------------- ------------------------------------------------------------------------	  
savefile          Type:*.csv     Default: \*.csv 
                         
				     Save pictures support csv formats.
================ ========================================================================

.. rubric:: Example

.. rubric:: Modify

Modify the parameters that are right for you to run.

.. rubric:: Begin

Use ``wgdi -kp kp.conf`` to run the parameter file and output the results you want.

.. image :: _static/1.png
   :align: left