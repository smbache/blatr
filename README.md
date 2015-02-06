# Send emails from R using Blat SMTP mailer for Windows.

This package is a wrapper around Blat for windows which 
enables simple email features. For details on the available features, see the
[Blat documentation](http://www.blat.net/syntax/syntax.html "Blat documentation.").
You will need to download the Blat executables (public domain) separately,
or use the installer function in the `blatr` package. See below.

### Installation (you need `devtools` installed):

```R
devtools::install_github("smbache/blatr")

# for 64 bit Blat:
blatr:::install_blat(arch = 64) 

# for 32 bit Blat:
blatr:::install_blat(arch = 32) 

# The above commands will prompt ask you if you are sure you want
# to install Blat. To force this (e.g. for automated installation) use
blatr:::install_blat(arch = 64, force = TRUE)

```

### Usage:

```R
blat(...)

Arguments:
  ...  name=value pairs corresponding to blat arguments.
```

blat documentation and arguments can be found [here](http://www.blat.net/syntax/syntax.html). 


### Examples:
```R
# With attachment
blat(f      = "Your Name <your@email.com>",
     to     = "your-recipients@email.com",
     s      = "The subject",
     server = "server.address",
     attach = "C:\\path\\to\\attachment.txt",
     body   = "The text you wish to send.")

# With file as body
blat(f        = "Your Name <your@email.com>",
     to       = "your-recipients@email.com",
     s        = "The subject",
     server   = "server.address",
     attach   = "C:\\path\\to\\attachment.txt",
     filename = "C:\\path\\to\\file\\with\\body.txt")
``` 

### Blat License
Blat is public domain, but Blat may not be used to send 
unsolicited commercial eMail (UCE). Be sure to check out the
[full license](http://www.blat.net/?docs/license.txt)!

### Blat website
You get more information about Blat at [their website](http://blat.net)
