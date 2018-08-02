Installation
====================================================================================

R and RStudio
------------------------------------------------------------------------------------
Note: set install dependencies to TRUE

Install R from the `CRAN website <https://cran.r-project.org>`_ .

.. image:: media/downloadR.png
   :scale: 100%
   
R is a free open source package available Linux, Windows and Mac OS X. 
Please install the latest version of R. If an earlier R version is installed,
please remove this version and reinstall the latest version.
 
Install RStudio from the website: https://www.rstudio.com/products/rstudio/download/ 

RStudio is a Graphical User Interface for R. 

Scroll down and select the file corresponding to your OS: 


The sdcMicro Package
------------------------------------------------------------------------------------
.. code-block:: R

		install.packages()
		second
 
Install the latest version of the sdcMicro add-on package (internet connection is required). 

To do so open the application R and type the commands install.packages(“sdcMicro”). 
A prompt will ask you to select a CRAN mirror (server) to install the package from. 
Note: also dependencies will be installed and the installation may take some time. 
Dependencies are other add-on packages, of which the functionality is required to run the sdcMicro package.


You can now load the sdcMicro package by typing library(sdcMicro) 
and launch the application by typing sdcApp(). 

The application opens in your default web browser through the local host IP 127.0.0.1:

**NOTE:** An internet connection is not required while using sdcMicro and sdcApp and the data 
stored locally on your computer or server. The web browser uses a local host IP, 
which is not connected to the internet and the browser is only used to communicate with 
the running R session.
    
Launching sdcApp
------------------------------------------------------------------------------------
test

