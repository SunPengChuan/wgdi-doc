BlockInfo
---------

The color distinction in the dot plot, the collinearity result and the Ks result are integrated into one file. 
This file contains the main information to achieve the purpose of easily screening the collinearity fragments.
  
.. rubric:: Parameters

.. tabularcolumns:: column spec

================ ========================================================================
Parameters       Standards and instructions
---------------- ------------------------------------------------------------------------
collinearity     Type: **file** |    Default: **-**
                     
                 Colinearscan or MCScanX result file or gene pairs divided by tab.
---------------- ------------------------------------------------------------------------
score            Type: **int**  |   Default: **100**
  
                 Score value in the blast results.
---------------- ------------------------------------------------------------------------
evalue           Type: **float**   |  Default: **1e-5**

                 Evalue value in blast result. 
---------------- ------------------------------------------------------------------------
repeat_number    Type: **int**  |   Default: **10**
  
                 The maximum number of homologous genes is allowed to remove more than part of the population.
---------------- ------------------------------------------------------------------------
position         Type: {**order**}  |   Default: **order**

                 The position of a gene corresponds to the gff file.
---------------- ------------------------------------------------------------------------
ks               Type: **file**  |    Default: **-**
                     
                 Ks calculation results.
---------------- ------------------------------------------------------------------------
ks_col           Type: **str**    Default: **NG86**

                 The result calculated by ks_YN00 or other methods is a single column.
---------------- ------------------------------------------------------------------------
savefile         Type: **file**   |  Default: \* **.csv**
                    
                 Result file.
================ ========================================================================

Use command to enter the folder ``wgdi -bi ? >> total.conf`` Take out the parameter file.

.. code-block:: python

   [blockinfo]
   blast = blast file
   gff1 =  gff1 file
   gff2 =  gff2 file
   lens1 = lens1 file
   lens2 = lens2 file
   collinearity = collinearity file
   score = 100
   evalue = 1e-5
   repeat_number = 10
   position = order
   ks = ks file
   ks_col = ks_NG86
   savefile = block information (*.csv)

.. rubric:: Quick start

After the parameters are modified properly, then run ``wgdi -bi total.conf`` 

.. rubric:: Example

The original results are easily accessible at `wgdi-example <https://github.com/SunPengChuan/wgdi-example>`_

================= ========================================================================
columns           Information
----------------- ------------------------------------------------------------------------
id                Type: **str** 
                     
                  Unique id.
----------------- ------------------------------------------------------------------------
chr1,chr2         Type: **int**
  
                  Two chromosomes corresponding to collinearity block.
----------------- ------------------------------------------------------------------------
start1,end1       Type: **int**

                  The region of chromosome 1 on collinearity block. 
----------------- ------------------------------------------------------------------------
start2,end2       Type: **int**
  
                  The region of chromosome 2 on collinearity block. 
----------------- ------------------------------------------------------------------------
pvalue            Type: **float**

                  Evaluate the compactness and uniqueness of collinear blocks, the range is 0-1, the better collinearity range is 0-0.2.
----------------- ------------------------------------------------------------------------
length            Type: **int**
                     
                  The length of collinearity block.
----------------- ------------------------------------------------------------------------
ks_median         Type: **float**

                  The median of ks value on collinearity block.
----------------- ------------------------------------------------------------------------
ks_average        Type: **float**
                    
                  The average of ks value on collinearity block.
----------------- ------------------------------------------------------------------------
homo1-5           Type: **float**

                  The average of scores of different color dots (red=1, blue=0, gray=-1) on synteny blocks.
----------------- ------------------------------------------------------------------------
block1,block2     Type: **str**
  
                  Gene pairs in collinear blocks
----------------- ------------------------------------------------------------------------
ks                Type: **str**

                  Output result of parameter `ks`.
----------------- ------------------------------------------------------------------------
tandem_ratio      Type: **float**

                  The density of tandem repeats, in general, a synteny block greater than 0.5 is unreliable.
----------------- ------------------------------------------------------------------------
density1,density2 Type: **float**
                     
                  Density of collinear blocks.
----------------- ------------------------------------------------------------------------
class1,class2     Type: **str**

                  Class of collinear blocks.
================= ========================================================================