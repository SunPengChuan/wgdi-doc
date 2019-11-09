ks
--

ks is calculate Ka/Ks for homologous gene pairs by Comdel.

.. rubric:: Parameters

Use command to enter the folder ``wgdi -ks ? > ks.conf`` Take out the parameter file.::

   [ks]
   cds_file = cds file
   pep_file = pep file
   align software = muscle
   pairs_file = gene  pairs file
   ks_file = ks result

.. tabularcolumns:: column spec

================ ========================================================================
Parameters        Standards and instructions
---------------- ------------------------------------------------------------------------
cds_file          Type: str     Default: -
                  
                     A cds file of one or more genomes.				  
---------------- ------------------------------------------------------------------------
pep_file          Type:str     Default:- 
                  
				     A protein file for one or more genomes. non-essential files, if you 
					 
				  do not write this parameter, Then this file will be translated through 
				  
				  the biopython module cds-file.
---------------- ------------------------------------------------------------------------
align_software    Type:{muscle,mafft}     Default: muscle

                     Multi-sequence comparison software.
---------------- ------------------------------------------------------------------------
pairs_file        Type:str     Default: -

                     The same gene pairs of ks need to be calculated, either by pressing, 
				  
				  or separating the list, or as the output of ColinearScan.
---------------- ------------------------------------------------------------------------
ks_file           Type:str     Default: -

                     The output file name of ks.
================ ========================================================================	  

.. rubric:: Example

.. rubric:: Modify

Modify the parameters that are right for you to run.

.. rubric:: Begin

Use ``wgdi -ks ks.conf`` to run the parameter file and output the results you want.

.. image :: _static/1.png
   :align: left