Introduction
====================================================================================

What is sdcApp?
---------------

*sdcApp* is the Graphical User Interface (GUI) for the R package *sdcMicro* (see
`here <https://cran.r-project.org/web/packages/sdcMicro/index.html>`_). The *sdcApp* 
opens the functionality of sdcMicro to users not familiar with the statistical
programming language *R*. *sdcMicro* is an add-on package for the statistical software *R* 
for Statistical Disclosure Control (SDC) of microdata and includes functions for risk measurement, 
anonymization and utility measurement for
microdata. All functionality available in the *sdcMicro* package is also available in *sdcApp*.


Statistical Disclosure Control (SDC)
-------------------------------------
A large part of the data collected by statistical agencies cannot be published directly 
due to privacy and confidentiality concerns. These concerns are both of legal and ethical 
nature. SDC seeks to treat and alter the data so that the data can be published or 
released without revealing the confidential information it contains, while, at the same time, 
limit information loss due to the anonymization of the data. There are two strands of literature 
on SDC: 1) for microdata and 2) for tabular data. *sdcMicro* and *sdcApp* only provide the tools
and methodology for protecting microdata.

What is the purpose of the manual?
----------------------------------
This manual is designed to provide step-by-step guidance through the process of anonymizing a
dataset with microdata. Both the background information on methods and measures is 
provided as well as instructions on how to complete these steps in sdcApp. As *sdcApp* is a 
GUI for the *sdcMicro* package, users familiar with using *R* for statistical analysis
may prefer to carry out the anonymization process using *R* from command-line. 
More information and guidance on using *sdcMicro* from command-line 
is available in the SDC Practice Guide available `here <https://sdcpractice.readthedocs.io/en/latest/>`_.
This guide also provides more detailed background information on SDC.

Background literature on SDC for microdata
------------------------------------------
Add here links to websites/books

Outline of this guide
---------------------

This guide is divided into the following main sections:

(1)   	the Section `Installation and updating <installation.html>`__ guides the user through the installation process of sdcApp, which includes the installation of R, RStudio as well as the required packages. It also discusses the need and process of regular updates of all software components.
(2)  	the Section `Introduction to sdcApp <introsdcApp.html>`__ covers how to launch and close the application and provides a brief overview of structure of the application.  of the structure of the application
(3)  	the Section `Loading and preparing data <loadprepdata.html>`__ describes how to load microdata into the application. It also discusses the requirements to the 
(4)   	the Section `Setup anonymization problem <setup.html>`__  covers the variable selection and setup of an SDC problem.
(5)  	the Section `Risk measurement <risk.html>`__ covers methods to measure the disclosure risk in the microdata.
(6) 	the Section `Anonymization methods <anon.html>`__ covers anonymization methods for quantitative and qualitative variables.
(7) 	the Section `Utility measurement <utility.html>`__ covers the measurement of information loss resulting from anonymization of the data
(8)  	the Section `Export data and reports <export.html>`__ describes how to export the anonymized dataset and generate reports.
(9)   	the Section `Reproducibility <reproducibility.html>`__ covers functionality that render the anonymization process reproducable.

? Add case study ?