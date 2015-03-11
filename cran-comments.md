## Minor update information:
This minor update fixes a bug where filenames to be used as
email body was not always quoted correctly for the system command.

I also corrected the quotation style for 'Blat' in the 
title and description, as requested.

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
