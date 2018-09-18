<center><img src="https://github.com/j-bresson/Spat-SDIF-Player/blob/master/images/spat-sdif-player.png" width=600></center>

# Spat-SDIF-Player

Spat-SDIF-Player is a Max patch or standalone application allowing to load spatialization data stored in [SDIF](http://sdif.sourceforge.net/) format, and to stream them as [SpatDIF](http://www.spatdif.org/)-compliant [OSC](http://opensoundcontrol.org/) messages to any OSC-compatible application.

SDIF files can be produced by [OpenMusic](http://repmus.ircam.fr/openmusic/) and the [OM-Spat](http://support.ircam.fr/docs/om-libraries/main/co/OM-Spat.html) library's SPAT-MATRIX objects using SAVE-SPAT-SDIF.

Only position data (SDIF frames/matrices of type "XSRC"/"XCAR"), orientation ("XSRC"/"XORI") and aperture ("XSRC"/"XAPE") are loaded in the player. 

--------
#### Dependencies

* MuBu for Max by ISMM ©Ircam-Centre Pompidou: http://forumnet.ircam.fr/fr/produit/mubu/
* CNMAT Max/MSP Externals (OSC) ©UC Berkeley: http://cnmat.berkeley.edu/downloads

--------
Jean Bresson — IRCAM / CIRMMT — 2010-2011.


--------
**See also (related articles):** 
* Jean Bresson, Marlon Schumacher. [Representation and Interchange of Sound Spatialization Data for Compositional Applications](https://hal.archives-ouvertes.fr/hal-01169015). International Computer Music Conference, Huddersfield, United Kingdom, 2011.
* Jean Bresson. [Spatial Structures Programming for Music](https://hal.archives-ouvertes.fr/hal-01161314). Spatial Computing Workshop (SCW), Valencia, Spain, 2012.


<img src="https://github.com/j-bresson/Spat-SDIF-Player/blob/master/images/spat-sdif-player-om-max.png" width=600 aligh="right">


#### Note for iuse in OpenMusic 

It is possible to control **Spat-SDIF-Player** from OpenMusic, via OSC communication on the "Incoming OSC" port (top-right of the window).  When an SDIFFile object is "played" from OM (selected + 'space' key), its pathname is sent for loading and rendering on the default OSC port.
