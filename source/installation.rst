Installation
------------

WGDI can be deployed in Windows, Linux, and Mac OS operating systems and can be installed via pip and conda. 

**Bioconda**

.. code-block:: python

   conda install -c bioconda  wgdi

**Pypi**

.. code-block:: python

   pip install wgdi

**Github**

.. code-block:: python

   git clone https://github.com/SunPengChuan/wgdi.git
   cd wgdi
   python setup.py install

**Dependencies**

Some parts of WGDI use the following third-party softwares: 

`PAML <http://abacus.gene.ucl.ac.uk/software/paml.html>`_  |  `MAFFT <https://mafft.cbrc.jp/alignment/software/>`_  | `MUSCLE <http://www.drive5.com/muscle/downloads.htm>`_  | `PAL2NAL <http://www.bork.embl.de/pal2nal/#Download>`_ `IQTREE <http://www.iqtree.org/#download>`_ 

After you download and install the above packages. You can run ``wgdi -conf help > conf.ini`` to configure the path of the existing software.

.. code-block:: python

   [ini]
   mafft_path = C:\bio\mafft-win\mafft.bat
   pal2nal_path = C:\bio\pal2nal.v14\pal2nal.pl
   yn00_path = C:\bio\paml4.9j\bin\yn00.exe
   muscle_path = C:\bio\muscle-win64.v5.3.exe

Add the directory of your software to the conf.ini file, and then execute ``wgdi -conf conf.ini`` to complete the configuration path.
 
.. code-block:: python

   [ini]
   mafft_path = /usr/bin/mafft
   pal2nal_path = /usr/local/bin/pal2nal.v14/pal2nal.pl
   yn00_path = /usr/bin/yn00
   muscle_path = /usr/bin/muscle
   iqtree_path = /usr/bin/iqtree

   



**Uninstall**

If you don't need ``wgdi``, you can uninstall with ``pip uninstall wgdi`` or ``conda remove wgdi``.
