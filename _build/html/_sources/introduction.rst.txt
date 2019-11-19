Introduction
====================================================================================

What is sdcApp?
---------------

*sdcApp* is the Graphical User Interface (GUI) for the R package *sdcMicro* (`TKM15`_) (see
`here <https://cran.r-project.org/web/packages/sdcMicro/index.html>`_). The *sdcApp* 
opens the functionality of *sdcMicro* to users not familiar with the statistical
programming language *R*. *sdcMicro* is an add-on package for the statistical software *R* 
for Statistical Disclosure Control (SDC) of microdata and includes functions for risk measurement, 
anonymization and utility measurement for
microdata. All functionality available in the *sdcMicro* package is also available in *sdcApp*.


Statistical Disclosure Control (SDC)
-------------------------------------
A large part of the data collected by statistical agencies cannot be published directly 
due to privacy and confidentiality concerns. These concerns are both of legal and ethical 
nature. SDC seeks to treat and alter the data in such a way that the data can be published or 
released without revealing the confidential information it contains, while, at the same time, 
limit information loss due to the anonymization of the data. There are two main strands of literature 
on SDC: 1) for microdata and 2) for tabular data. *sdcMicro* and *sdcApp* only provide the tools
and methodology for protecting microdata.

What is the purpose of the manual?
----------------------------------
This manual is designed to provide step-by-step guidance through the process of anonymizing a
dataset with microdata. The focus of this manual is on providing instructions on how to 
complete these steps in *sdcApp*, but also includes limited information on the
implemented methods and measures. For more in-depth information on the measures and methods 
as well a the SDC process, we refer to the accompanying theory guide
`Statistical Disclosure Control for Microdata: Theory <https://sdctheory.readthedocs.io/en/latest/>`_. 
As *sdcApp* is a GUI for the *sdcMicro* package, users familiar with using *R* for statistical analysis
may prefer to carry out the anonymization process using *R* from command-line. 
More information and guidance on using *sdcMicro* from command-line 
is available in the `Statistical Disclosure Control for Microdata: A Practice Guide for sdcMicro <https://sdcpractice.readthedocs.io/en/latest/>`_.

Background literature on SDC for microdata
------------------------------------------
There is a broad scientific literature available on SDC for microdata. The guide
`Statistical Disclosure Control for Microdata: Theory <https://sdctheory.readthedocs.io/en/latest/>`_
provides a full overview of all methods used and implemented in sdcMicro and sdcApp, as well
as provides an overview over the full SDC process. It also contains references to the 
appropriate literature. 

`HDFG10`_ (and [HDFG12]) is a handbook written by practitioners in NSOs and is especially worth mentioning 
for those seeking to read a complete overview. This volume also contains information on 
SDC for tabular data.

Outline of this guide
---------------------

This guide is divided into the following main sections:

(1)   	the Section `Installation and updating <installation.html>`__ guides the user through the installation process of *sdcApp*, which includes the installation of *R*, *RStudio* as well as the required packages. It also discusses the need and process of regular updates of all software components.
(2)  	the Section `Introduction to sdcApp <introsdcApp.html>`__ covers how to launch and close the application and provides a brief overview of structure of the application.
(3)  	the Section `Loading and preparing data <loadprepdata.html>`__ describes how to load microdata into the application. It also discusses the requirements to the microdata and how to prepare the microdata.
(4)   	the Section `Setup anonymization problem <setup.html>`__  covers the variable selection and setup of an SDC problem.
(5)  	the Section `Risk measurement <risk.html>`__ covers methods to measure the disclosure risk in the microdata.
(6) 	the Section `Anonymization methods <anon.html>`__ covers anonymization methods for quantitative and qualitative variables.
(7) 	the Section `Utility measurement <utility.html>`__ covers the measurement of information loss resulting from anonymization of the data.
(8)  	the Section `Export data and reports <export.html>`__ describes how to export the anonymized dataset and generate reports.
(9)   	the Section `Reproducibility <reproducibility.html>`__ covers functionality that render the anonymization process reproducable.
(10)	the Section `Case Studies <casestudies.html>`__ presents two case studies illustrating the full SDC process in *sdcApp*.

References
----------

.. [HDFG10] Hundepool, A., Domingo-Ferrer, J., Franconi, L., Giessing, S., Lenz, R., Naylor, J., et al. (2010). 
	**Handbook on Statistical Disclosure Control.**
	ESSNet SDC. Retrieved November 18, 2019 from https://ec.europa.eu/eurostat/cros/system/files/SDC_Handbook.pdf
	
.. [HDFG12]	Hundepool, A., Domingo-Ferrer, J., Franconi, L., Giessing, S., Schulte Nordholt, E., Spicer, K., and de Wolf, P.-P. (2012). 
	Statistical Disclosure Control. Chichester: John Wiley & Sons Ltd. doi:10.1002/9781118348239.
	
.. [TKM15]	Matthias Templ, Alexander Kowarik, Bernhard Meindl (2015). 
	Statistical Disclosure Control for Micro-Data Using the R Package sdcMicro. 
	**Journal of Statistical Software**, 67(4), 1-36.<doi:10.18637/jss.v067.i04>

