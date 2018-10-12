Risk measurement
================

Summary view
------------

Global risk measure
~~~~~~~~~~~~~~~~~~~
For categorical variables

:math:`k`-anonymity
~~~~~~~~~~~~~~~~~~~
The risk measure :math:`k`-anonymity is based on the principle that, in a safe
dataset, the number of individuals sharing the same combination of
values (keys) of categorical quasi-identifiers should be higher than a
specified threshold :math:`k`. :math:`k`-anonymity is a risk
measure based on the microdata to be released, since it only takes the
sample into account. An individual violates :math:`k`-anonymity if the
sample frequency count :math:`f_{k}` for the key :math:`k` is smaller
than the specified threshold :math:`k`. For example, if an
individual has the same combination of quasi-identifiers as two other
individuals in the sample, these individuals satisfy 3-anonymity but
violate 4-anonymity. In the dataset in :numref:`tab41`, six individuals
satisfy 2-anonymity and four violate 2-anonymity. The individuals that
violate 2-anonymity are sample uniques. The risk measure is the number
of observations that violates k-anonymity for a certain value of *k*,
which is

.. math:: \sum_{i}^{}{I(f_{k} < k)},

where :math:`I` is the indicator function and :math:`i` refers to the
:math:`i`\ :sup:`th` record. This is simply a count of the number of
individuals with a sample frequency of their key lower than :math:`k`.
The count is higher for larger :math:`k`, since if a record satisfies
:math:`k`-anonimity, it also satisfies :math:`(k + 1)`-anonimity. The
risk measure :math:`k`-anonymity does not consider the sample weights,
but it is important to consider the sample weights when determining the
required level of :math:`k`-anonymity. If the sample weights are large,
one individual in the dataset represents more individuals in the target
population, the probability of a correct match is smaller, and hence the
required threshold can be lower. Large sample weights go together with
smaller datasets. In a smaller dataset, the probability to find another
record with the same key is smaller than in a larger dataset. This
probability is related to the number of records in the population with a
particular key through the sample weights.

In the summary view

.. _fig24:

.. figure:: media/summary_k_anon.png
   :align: center
   
   Information on :math:`k`-anonymity violators in summary view
   
Risk measures for numerical key variables
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


Household risk
~~~~~~~~~~~~~~~~~~~
If household identifier is selected, household risk will automatically be displayed.

Detailed view
-------------
The Risk/Utility tab provides more detailed information on risk measures and records at 
(high) risk.

Risky observations
~~~~~~~~~~~~~~~~~~~

SUDA
~~~~~~~~~~~~~~~~~~~
The SUDA algorithm identifies all the MSUs in the sample, which in turn
are used to assign a SUDA score to each record. This score indicates how
“risky” a record is. The potential risk of the records is determined
based on two observations:

-  The smaller the size of the MSU within a record (i.e., the fewer
   variables are needed to reach uniqueness), the greater the risk of
   the record

-  The larger the number of MSUs possessed by a record, the greater the
   risk of the record

.. _fig24:

.. figure:: media/risk_suda_setup.png
   :align: center
   
   Compute SUDA scores
   
.. _fig24:

.. figure:: media/risk_suda_result.png
   :align: center
   
   Result of SUDA calculation

l-diversity
~~~~~~~~~~~~~~~~~~~
A dataset
satisfies :math:`l`-diversity if for every key :math:`k` there are at least
:math:`l` different values for each of the sensitive variables. In the
example, the first two individuals satisfy only 1-diversity, individuals
4 and 6 satisfy 2-diversity. The required level of :math:`l`-diversity
depends on the number of possible values the sensitive variable can
take. If the sensitive variable is a binary variable, the highest level
if :math:`l`-diversity that can be achieved is 2. A sample unique will
always only satisfy 1-diversity.

To compute :math:`l`-diversity for sensitive variables in sdcApp


k-anonymity
~~~~~~~~~~~~~~~~~~~

.. _fig24:

.. figure:: media/summary_k_anon.png
   :align: center
   
   Information on :math:`k`-anonymity violators for any level of :math:`k`



