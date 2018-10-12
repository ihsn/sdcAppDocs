Loading and Preparing Data
==========================

Loading data
------------

Testdata
--------
sdcApp comes with two testdata datasets: testdata and testdata2. The testdata dataset is
used for 

.. NOTE:: 
	All examples in the testdata
	
Other datasets
--------------
sdcApp supports datasets in several foreign data formats (cf. :numref:`tabloadprep71`). 
If the microdata is not in one of these dataformats,another software can be used to convert the 
data, such as StatTransfer. In order to load a dataset, select in the left sidebar of the 
Microdata tabtabloadprep

.. _tabloadprep1:

.. table:: Data formats compatible with sdcApp
   :widths: auto
   :align: center
   
   ==========  ================
   Software     File extension
   ==========  ================
   R/RStudio	.rdata
   SPSS			.sav
   SAS			.sas7bdat
   CSV			.csv, .txt
   STATA		.dta
   ==========  ================

Inspect and explore data
------------------------
After loading the dataset into sdcApp, the data is shown. A this moment, the user should 


Preparing data
--------------
Most datasets need to be prepared before the start of the anonymization process. Examples 
of data preparation are removing variables that are not suitable for release, etc. It is
recommended to carry out the data preparation in a statistical software of choice, before 
loading the data in sdcApp. Data preparation includes 

After loading the data in sdcApp, still some steps may need to be carried, which are 
specific to the needs of the sdcApp. These steps are discussed in the following subsections.

Convert variable type
^^^^^^^^^^^^^^^^^^^^^

Set missing values to NA
^^^^^^^^^^^^^^^^^^^^^^^^
Missing values play an important role in anonymization of microdata. In particular when 
measuring disclosure risk of categorical key variables (see `Risk`__). sdcApp only considers
the R missing value :code:`NA` as missing. Therefore, it is important to recode other missing values,
such as 9, 99, 998 or 999, "Missing", "Not applicable" after loading the
data to the R missing value :code:`NA`, if appropriate. Many standard missing value codes 
in the data, such as :code:`.` in STATA are automatically converted to NA upon loading
the data into *sdcApp*.



.. _fig57:

.. figure:: media/prepareMissingToNA.png
   :align: center
   
   Screen to set specific value in a variable to NA


Create stratification variable
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Hierarchical data
^^^^^^^^^^^^^^^^^


