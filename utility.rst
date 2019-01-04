Utility measurement
===================

General utility measures in *sdcApp*
------------------------------------

Compare summary statistics
~~~~~~~~~~~~~~~~~~~~~~~~~~

Categorical variables
+++++++++++++++++++++

Continuous variables
+++++++++++++++++++++

IL1s measure
~~~~~~~~~~~~


Customized utility measures
---------------------------
As the statistical analyses based on the microdata depend, amongst others,
on to the topic of the survey, the country and the definition of the variables,
it is not feasible to include all these measures in *sdcApp*. Instead, it is recommended 
to compute the statistics and indicators and perform statistical an econometric
analyses on the original and anonymized datasets and evaluate the differences in the results.
If a publication based on the microdata is already published, it is recommended
to recompute the statistics in these publications from the anonymized dataset.

The approach is to compare the indicators calculated on the untreated data and the 
data after anonymization with different methods. If the differences between the 
indicators are not too large, the anonymized dataset can be released for use by 
researchers. It should be taken into account that indicators calculated on samples 
are estimates with a certain variance and confidence interval. Therefore, for sample 
data, it is more informative to compare the overlap of confidence intervals and/or 
to evaluate whether the point estimate calculated after anonymization is contained 
within the confidence interval of the original estimate.

.. NOTE::
	Some analyses may no longer be possible or not possible in exactly the same way.
	E.g. regression on age if age is recoded in 5-year intervals.

In order to do so, it is posible to export the dataset at any point in *sdcApp*.
See Export dataset. Several datasets can be exported after applying different methods 
with different parameters settings to compare the information loss resulting from
the anonymization. This information can be used to select the anonymization methods 
as well as to inform the user about the implications of the anonymization on
the validity of the dataset for analysis.	


