Reproducibility
================

Reproducibility is key to the SDC process, as ...

Exporting *R* script
--------------------
*sdcApp* is a GUI for the *R* package *sdcMicro*. All steps executed in *sdcApp* are translated 
into *R* commands. Therefore, the full anonymization can also be performed from command-line
in *R*. While carrying out the anonymization process, the code to perform the same action
from command-line is generated. The code can be viewed and exported on the **Reproducibility**
tab by selecting **View the current script** from the left sidebar (cf. :numref:`fig111`).
The script also contains comments, which are the lines starting with the hash tag (:code:`#`).
These comments are meant to help with the interpretation of the code blocks.

.. _fig111:

.. figure:: media/reproScript.png
   :align: center
   
   *R* script to reproduce anonymization process after setting up SDC problem

The goal of the *R* script is threefold: 
1) To reproduce the steps taken in the anonymization process. This guarantees
the reproducibility, since the all variabele selections and parameters are contained in the 
code and the order of the application of different methods is preserved in the code.
2) As a starting point to learn *R* and use *sdcMicro* from *R* command-line. Especially for 
users with some degree of familiarity with *R*, the script 
3) To rerun the same methods with different parameter settings without the need to make
all selections by mouseclick in the GUI. It's relatively easy to change the parameter settings 
in the *R* code and rerun the code. However, the code does not include commands to shw
the results.

By clicking on the blue button **Save script to file** at the top of the page, the script
is saved as *R* script (extension .R) on disk to the selected storage path on the 
**About/Help** tab (see `Introduction to sdcApp <introsdcApp.html>`__). 
The filename of the exported script starts with 'exportedScript_sdcMicro' followed 
by a date and time stamp, e.g., 'exportedScript_sdcMicro_20181010_1212.R'.

In order to run the script in *R*, open the saved script in *RStudio*. The only 
thing to do is to change the path of the input file to the actual file path on your computer.
In the second line of the *R* script, 

.. NOTE:: 
	In case a method was applied in *sdcApp* and subsequently reverted by using the **Undo**
	button, the method is not erased from the script, but rather the undo command is added.
	For example, if local suppression was applied and reverted, this appears as follows in 
	the script:

	.. code-block:: R
		:linenos:
		
		## Local suppression to obtain k-anonymity
		sdcObj <- kAnon(sdcObj, importance=c(1,2,3), combs=NULL, k=c(3))
		sdcObj <- undolast(sdcObj)
	
	This code preceding the :code:`undoLast`command and the :code:`undoLast`command
	can be deleted without changing the results.

   		
Exporting reports
-----------------
It is extremely important to document the SDC process of microdata both for internal 
use as well as for external use. The internal report should contain detailed descriptions
of all steps carried out as well as reasoning for 


Internal report
~~~~~~~~~~~~~~~
An important step in the SDC process is reporting, both internal and external. 
Internal reporting contains the exact description of anonymization methods used, 
parameters but also the risk measures before and after anonymization. This allows 
replication of the anonymized dataset and is important for supervisory authorities/bodies
to ensure the anonymization process is sufficient to guarantee anonymity according 
to the applicable legislation.

Report is just technical overview, not complete

.. _fig112:

.. figure:: media/reproScript.png
   :align: center
   
   Exporting an internal report

External report
~~~~~~~~~~~~~~~
The external report

External reporting informs the user that the data has been anonymized, 
provides information for valid analysis on the data and explains the limitations to 
the data as a result of the anonymization. A brief description of the methods used 
can be included. The release of anonymized microdata should be accompanied by the 
usual metadata of the survey (survey weight, strata, survey methodology) as well as 
information on the anonymization methods that allow researchers to do valid analysis 
(e.g., amount of noise added, transition matrix for PRAM).
