## General
This is a re-submission based on Email response from
Uwe Ligges and Prof. Brian Ripley. It seems the Blat 
URL was unstable, I have success browsing through the 
main website. I missed the title case and the period; 
has been corrected (again!). 
A short case for windows only is given below.

## Test environments
* local Windows installation (this is a Windows only package)
* win-builder (devel and release)

## R CMD check results
There were no ERRORs or WARNINGs.

There was one NOTE that SMTP is a possibly mis-spelled word.

## Downstream dependencies
There are no downstream dependencies.

## Case for windows-only package and other notes.
I've found no really good way for sending Emails using R
on Windows. Blat is a very flexible and powerful command
line tool for Windows. This wrapper therefore provides
an easy way of sending Emails through R when using
Windows. Blat is Windows-only.

The package requires public domain binaries to work. These 
are not included in the package, but can be installed from
within R using the package, or installed manually.

Indeed, I missed the R-devel output as the Email said
that check status was OK. I have now checked R-devel
output too.
