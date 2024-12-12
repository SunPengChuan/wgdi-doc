Changelog
---------

.. rubric:: 0.7.1

* Added extract the fusion positions dataset (-fpd).
* Added determine whether these fusion events occur in other genomes (-fd).
* Improved the karyotype_mapping (-km) effect.
* Fixed the problem caused by the Python version, now it is compatible with version 3.12.

.. rubric:: 0.6.5

* Fixed some issues (-sf).
* Added new tips to avoid some errors.

.. rubric:: 0.6.4

* Fixed the problem caused by the Python version, now it is compatible with version 3.11.3.

.. rubric:: 0.6.3
    
* Fixed some issues (-ks, -sf).

.. rubric:: 0.6.2

* Added find shared fusions between species (-sf).

.. rubric:: 0.6.1

* Fixed issue with alignment (-a). Only version 0.6.0 has this bug.

.. rubric:: 0.6.0

* Fixed issue with improved collinearity (-icl).
* Added a parameter 'tandem_ratio' to blockinfo (-bi).

.. rubric:: 0.5.9

* Update the improved collinearity (-icl). Faster than before, but lower than MCscanX, JCVI.
* Fixed issue with ancestral karyotype repertoire (-akr).

.. rubric:: 0.5.8

* Fixed issue with gene names (-ks).

.. rubric:: 0.5.7

- Fixed issue with chromosome order (-ak).
- Fixed issue with gene names (-ks).  This version is not fixed, please install the latest version.

.. rubric:: 0.5.5 and 0.5.6

* Add ancestral karyotype (-ak)
* Add ancestral karyotype repertoire (-akr)

.. rubric:: 0.5.4

* Improved the alignmenttrees (-km) effect.
* little change (-at).

.. rubric:: 0.5.3

* Fixed legend issue with (-kf).
* Fixed calculate Ks issue with (-ks).
* Improved the karyotype_mapping (-km) effect.
* Improved the alignmenttrees (-at) effect.

.. rubric:: 0.5.2

* Fixed some bugs.

.. rubric:: 0.5.1

* Fixed the error of the command (-conf).
* Improved the karyotype_mapping (-km) effect.
* Added the available data set of alignmenttree (-at). Low copy data set (for example, single-copy_groups.tsv of sonicparanoid2 software).

.. rubric:: 0.4.9
   
* The latest version adds karyotype_mapping (-km) and karyotype (-k) display.
* The latest version changes the calculation of extracting pvalue from collinearity (-icl), making this parameter more sensitive. Therefore, it is recommended to set to 0.2 instead of 0.05.
* The latest version has also changed the drawing display of ksfigure (-kf) to make it more beautiful.