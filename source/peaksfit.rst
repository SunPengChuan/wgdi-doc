PeaksFit
--------

peaksfit is gaussian fitting of ks distribution.

  
.. rubric:: Parameters

.. tabularcolumns:: column spec

================ ========================================================================
Parameters        Standards and instructions
---------------- ------------------------------------------------------------------------
blockinfo        Type: **file**  |    Default: **-**
                     
                 Output result of parameter `bi`
---------------- ------------------------------------------------------------------------
mode             Type: {**median**, **average**, **total**}   | Default: **median**

                 Different processing methods of ks value on collinearity block.
---------------- ------------------------------------------------------------------------
tandem_length    Type: **int**   | Default: **200**

                 If tandem=true, the maximum range of tandem influence.
---------------- ------------------------------------------------------------------------
bins_number      Type: **int**   |   Default: **200**
                     
                 Show the minimum length of a collinear block.
---------------- ------------------------------------------------------------------------
fontsize         Type: **float**   | Default: **9**

                 The fontsize of label in the plot.
---------------- ------------------------------------------------------------------------
area             Type: **str**   Default: **-1,3**
                     
                 Show the range of ks.
---------------- ------------------------------------------------------------------------
figsize          Type: **int,int** |  Default: **10,10**

                 Control the proportion of the size of the saved picture.
---------------- ------------------------------------------------------------------------
savefile         Type: {\*. **png**,\*. **pdf**, \*. **svg**}  |  Default: \*. **png**

                 Save pictures support png, pdf, svg formats.
================ ========================================================================

Use command to enter the folder ``wgdi -pf ? >> total.conf`` Take out the parameter file.

.. code-block:: python

   [peaksfit]
   blockinfo = block information
   mode = median
   bins_number = 200
   ks_area = 0,10
   fontsize = 9
   area = 0,3
   figsize = 10,6.18
   savefig = saving image



.. rubric:: Quick start

After the parameters are modified properly, then run ``wgdi -pf total.conf`` 


.. rubric:: Example

The original results are easily accessible at `wgdi-example <https://github.com/SunPengChuan/wgdi-example>`_

.. image :: _static/vvi161s_vvi161s.kspeaks.fit.png
   :align: left