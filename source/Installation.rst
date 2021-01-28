Installation
------------

Python package and command line interface (IDLE) for the analysis of whole genome duplications (WGDI). The environment required for installation is python3.

Method
""""""

*Bioconda*

.. code-block:: python

   conda install -c bioconda  wgdi

*Pypi*

.. code-block:: python

   pip install wgdi

*Github*

.. code-block:: python

   git clone https://github.com/SunPengChuan/wgdi.git
   cd wgdi
   python setup.py install

Third party software
""""""""""""""""""""

Some parts of WGDI use the following additional python libraries:

`paml <http://abacus.gene.ucl.ac.uk/software/paml.html>`_   


`mafft <https://mafft.cbrc.jp/alignment/software/>`_   


`muscle <http://www.drive5.com/muscle/downloads.htm>`_   

`pal2nal <http://www.bork.embl.de/pal2nal/#Download>`_   

After you download and install the above package. You can run the following command to configure the path of the existing software.

.. code-block:: python

   wgdi -conf help > conf.ini

conf.ini::

   [ini]
   mafft_path = C:\bio\mafft-win\mafft.bat
   pal2nal_path = C:\bio\[pal2nal.v14\pal2nal.pl
   yn00_path = C:\bio\paml4.9j\bin\yn00.exe
   muscle_path = C:\bio\muscle3.8.31_i86win32.exe


Uninstall
"""""""""

If you don't need ``wgdi``, you can uninstall with ``pip uninstall wgdi`` or ``conda remove wgdi``.
