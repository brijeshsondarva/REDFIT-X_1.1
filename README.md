# REDFIT-X-Cross-spectral-analysis-of-unevenly-spaced-paleoclimate-time-series

Name of the program: REDFIT-X



Title of manuscript: REDFIT-X: Cross-spectral analysis of unevenly spaced paleoclimate time series



Authors information:

Kristin Bjoerg Olafsdottir	olafsdottir@climate-risk-analysis.com, kristin904@msn.com

Michael Schulz			mschulz@marum.de

Manfred Mudelsee		mudelsee@climate-risk-analysis.com



Folders:

.\bin		      Executable files

.\src		      Fortran 90 source code

.\doc		      Documentation - User manual

.\example 	  Examples and configuration file




Additional information:

User manual with information about installation and how to run the program can be found in the .\example folder

A Fortran 90 compiler is needed to recompile REDFIT-X. We compiled the program with a Lahey compiler.

---------------------------------------------------------------------------------------------------------
-----------------------------Process for compile---------------------------------
~~~~~~~~~~~~~~~~~~~~~~
$ mkdir redfit
$ cd redfit
$ git clone https://github.com/brijeshsondarva/REDFIT-X_1.1.git
$ cd REDFIT-X_1.1/src/
$ ls
src$ vi redfit-x_1_1.f90  \\ edit the following changes in that file
~~~~~~~~~~~~~~~~~~~~~~
include '/home/user/redfit/src/nrtype.f90'

include '/home/user/redfit/src/nr.f90'

include '/home/user/redfit/src/nrutil.f90'

include '/home/user/redfit/src/avevar.f90'

include '/home/user/redfit/src/ran.f90'

include '/home/user/redfit/src/gammp.f90'

include '/home/user/redfit/src/gser.f90'

include '/home/user/redfit/src/gcf.f90'

include '/home/user/redfit/src/gammln.f90'

include '/home/user/redfit/src/erfcc.f90'

include '/home/user/redfit/src/sort.f90'

~~~~~~~~~~~~~~~~~~~~~~
src$  ftn redfit-x_1_1.f90
src$  ls
a.out  \\ executable
~~~~~~~~~~~~~~~~~~~~~~
