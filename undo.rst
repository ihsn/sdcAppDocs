Undo
====

Microdata anonymization is a trial-and-error process. It is necessary to several 
methods, each with different parameter settings, to find optimal set of 
anonymization measures that minimize the information loss, while reducing the risk of 
disclosure to an acceptable level. Before applying an alternative method to the same
variable or set of variables, it is important to undo the previously applied methods.
Only in this way, it is possible to compare the effect on risk and information
loss of a particular method or parameter setting. For instance to compare the 
effect of recoding the age variable in 5 or 10 year intervals, it is necessary to first
undo the recoding in 5-year intervals before recoding in 10 year intervals.

In *sdcApp* it is possible to undo the last anonymization step. In order to undo several
steps, it is required to save and reload the SDC problem. Both ways are explained below.

Undo one step
~~~~~~~~~~~~~
In order to undo one step, go to the **Undo** tab.
The screen shows 

risk measures etc are also reset, script not (completely), random seed not


Undo several steps
~~~~~~~~~~~~~~~~~~
Save and reload

Recommended to save the SDC problem after each method to be able to reload. This is also 
practical if *sdcApp* or *R* crash. Also useful to continue working at a later point of 
transfer a problem to a different computer	


Save a previously saved problem
+++++++++++++++++++++++++++++++

Load a previously saved problem
+++++++++++++++++++++++++++++++

.. NOTE::
	sdcApp exports four different file types
	Different file names for different files (data, sdcProblem)



