Setup anonymization problem
============================

Variable selection
------------------
In order to set up an SDC problem the user needs to select 

.. _fig11:

.. figure:: media/setupTable.png
   :align: center
   
   Table on Anonymize tab for variable selection
   
   
.. NOTE:: 
	All variables need to be of the appropriate variable type. If the variable type of a 
	variable is not suitable for the intended 

.. _tabsetup1:

.. table:: Columns in setup table
   :widths: auto
   :align: center
   
   =========================  =======================================================================================================================
	Column header              Description
   =========================  =======================================================================================================================
   Variable name			   Name of variable in original dataset
   Type                        Variable type in R (factor, integer, numeric, character)
   Key variables               Radio buttons to select variable as cat. or cont. key variable
   Weight                      Column to select variable as weight variable
   Hierarchical identifier     Column to select variable as hierarchical identifier
   PRAM                        Column to select variable for PRAM method
   Delete                      Column to select variable to be deleted from released dataset
   Number of levels            Number of different values (including NA/missing) in a categorical (type factor) variable
   Number of missing           Number of records with missing value for this particular variable
   =========================  =======================================================================================================================


.. NOTE:: 
	If an invalid variable choice is made, such as an invalid variable type 
	or a variable is selected for more than one choice, a pop-up window with an informative
	error message is shown. It is important to undo the invalid selection after clicking away 
	the error message, as this doesn't happen automatically. Not correcting the selection will
	make it later difficult to trace back the invalid selections. The blue setup button disappears and reappears once the problem is fixed.

Settings
--------

Besides the variable selection, there are two more parameters to be set: alpha and seed.

Alpha
~~~~~
The parameter alpha is used to compute the frequencies of . See for more information.

Seed
~~~~
Every time a probabilistic method is used, a different outcome is generated. For these 
methods it is often recommended that a seed be set for the random number generator
if you want to produce replicable results.

.. NOTE:: 
	Order of operations and use of undo matters for seed. 

Summary view
------------
After setting up the SDC problem, the application jumps automativcally to the Anonymize tab.
This tab first shows a Summary overview of the problem. The content of the summary page varies with
the SDC problem. For example, if no numerical key variables were selected, the information on
numeric key variables is omitted. Fig shows the summary page.

