Introduction to sdcApp
=======================

sdcApp is a user-friendly application for microdata anonymization 
and is built on the Shiny technology 
(see `here <https://www.shiny.org>`). Shiny allows users to 
communicate through a GUI that runs in a webbrowser with a local R session. The local
R session performs the necessary calculations. In the case of sdcApp, most functionality 
used in R is included in the sdcMicro package (see `here <https://www.sdcMicro.org>`).

sdcApp has tab structure	 and consists of seven tabs, which in turn consist of 
up to three panels. This structured is further explored below. 
The tabs and panels are used to navigate through the app.

Starting sdcApp
-----------------
After succcesful installation (cf. ), sdcApp is ready for use. Every single time sdcApp is
used, first the applications R or RStudio need to be opened. See the Section  
`Installation and updating`_
on how to install R and RStudio. After launching R or RStudio, 
the sdcMicro package needs to be loaded and sdcApp needs to be launched. This is done by 
entering the code as shown in code02 in the R console.

.. code-block:: R
   :linenos:
   :caption: Loading sdcMicro package and launching sdcApp
   :name: code02
   
   # Load sdcMicro package
   library(sdcMicro)
   
   # Launch sdcApp (opens in browser window)
   sdcApp()
   
The application opens in a new tab in your default web browser. In case you prefer to use
an alternative web browser, you can simply copy the internal path and paste it into
a different browser on the same machine. The application opens on the **About/Help** tab (see).

Getting started
---------------

Use testdata dataset: all examples in this guide are illustrated with the testdata dataset.


Set storage path
----------------


Tab structure
-------------
The sdcApp consists of eight different tabs. The tabs can be selected in the navigation
bar at the top of the page. The navigation bar is visible at all times. The content
of each tab may change as function of the current state of the SDC process. For example, 

Panel structure
---------------

Each tab can consists of two panels: the left sidebar and the main panel. 
. The left panel allows the user to navigate between different function on the 
tab. Some tabs have an additional right sidebar, which provide summary information 
on the current 
	

.. figure:: media/appStructure.png
   :align: center
   
   Risk/Utility tab with navigation bar and panel structure

Quiting sdcApp
------------------
It is recommended to quit R or RStudio after quitting sdcApp to ensure that nothing is 
left in the memory. This also applies to a restart due to sdcApp not responding.