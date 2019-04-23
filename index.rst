sdcMicro GUI manual
===================
The application of many anonymization methods is complex and requires knowledge of the methods and access to suitable tools for implementation. For users comfortable with using R, the package sdcMicro provides a tool for the application of a comprehensive suite of methods commonly used and described in the literature on disclosure control. Users not familiar with R, but who have an immediate need for tools to anonymize microdata, would benefit from a friendly Graphic User Interface (GUI) for the sdcMicro package.

To provide a GUI environment for the non-R user, the World Bank through a Grant from DFID,  funded the initial development of a Shiny GUI application called sdcApp, which has been added to the sdcMicro package.

Users of sdcApp can implement the most widely used anonymization methods present in the sdcMicro package without requiring in-depth knowledge of R. In addition to the anonymization methods implemented in the sdcMicro package, sdcApp offers a comprehensive set of risk and utility measures. This includes functions to measure, visualize and compare risk and utility throughout the anonymization process.  sdcApp also helps users by producing reports on the methods used in formats suitable for internal and external audiences and saves the underlying R code to ensure reproducibility.  For users of other statistical packages, sdcApp supports importing and exporting microdata in several formats. Like R, sdcMicro is open source and available in the CRAN repositories. 

Authors: Matthew Welch - Senior Statistician, World Bank, Thijs Benschop, Consultant,  World Bank

.. toctree::
   :maxdepth: 2
   :caption: Table of contents

   introduction
   installation
   about
   loadprepdata
   setup
   risk
   anon
   utility
   export
   reproducibility
