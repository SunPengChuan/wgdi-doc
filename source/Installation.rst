Installation
------------

Python package and command line interface (IDLE) for the analysis of whole genome duplications (WGDI). The environment required for installation is python3.

Method
""""""

We recommend using a python installation directly by using the commands available on PyPI:

.. code-block:: python

   pip install wgdi

upgrade with just one terminal command:

.. code-block:: python

   pip install --upgrade wgdi

Or use `Git <https://git-scm.com/>`_ to get the latest version of the source code on github, and install our program.

.. code-block:: python

   git clone https://github.com/SunPengChuan/wgdi.git
   cd wgdi
   python setup.py install

Third party software
""""""""""""""""""""

Some parts of WGDI use the following additional python libraries:

`paml <http://abacus.gene.ucl.ac.uk/software/paml.html>`_   

Yang, Z. 1997. PAML: a program package for phylogenetic analysis by maximum likelihood
Computer Applications in BioSciences 13:555-556.
Yang, Z. 2007. PAML 4: a program package for phylogenetic analysis by maximum likelihood.
Molecular Biology and Evolution 24: 1586-1591

`mafft <https://mafft.cbrc.jp/alignment/software/>`_   

Levy, A, I Salas González, M. Mittelviefhaus, S Clingenpeel, S Herrera Paredes, J Miao, K Wang, G Devescovi, K Stillman, F Monteiro, BR Alvarez, DS Lundberg, T-Y Lu, S Lebeis, Z Jin, M McDonald, AP Klein, ME Feltcher, T Glavina del Rio, SR Grant, SL Doty, RE Ley, DA Pelletier, J Vorholt, SG Tringe†, T Woyke† and JL Dangl† 
(2017) Genomic determinants of bacterial adaptation to plants. Nature Genetics doi: 10.1038/s41588-017-0012-9.

`muscle <http://www.drive5.com/muscle/downloads.htm>`_   

Edgar, R.C. (2004) MUSCLE: multiple sequence alignment with high accuracy and high throughput.Nucleic Acids Res. 32(5):1792-1797.
doi:10.1093/nar/gkh340
Edgar, R.C. (2004) MUSCLE: a multiple sequence alignment method with reduced time and space complexity BMC Bioinformatics, (5) 113.
doi:10.1186/1471-2105-5-113

`pal2nal <http://www.bork.embl.de/pal2nal/#Download>`_   

Mikita Suyama, David Torrents, and Peer Bork (2006)
PAL2NAL: robust conversion of protein sequence alignments into the corresponding codon alignments.
Nucleic Acids Res. 34, W609-W612.

After you download and install the above package. Go to the installation location of **WGDI**, find the **conf.ini** located in the wgdi folder, and change the location of its module to the location where you installed the module.

.\\Python\\Python37-32\\Lib\\site-packages\\wgdi\\conf.ini::

   [ini]
   mafft_path = C:\bio\mafft-win\mafft.bat
   pal2nal_path = C:\bio\[pal2nal.v14\pal2nal.pl
   yn00_path = C:\bio\paml4.9j\bin\yn00.exe
   muscle_path = C:\bio\muscle3.8.31_i86win32.exe

We recommend installing **Git** to work with **WGDI**, so you can quickly switch working directories when you start a large number of tasks.

Uninstall
"""""""""

If you don't need ``WGDI``, you can uninstall with ``pip uninstall wgdi``.
