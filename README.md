# kdz-toolkit
A list of script tools, informational resources, and analysis reports for LG KDZ firmware files.


Disclaimer: **This is a work in progress.** 

Working status for scripts:
```
kdz2imgs      - works for most. temporary fixes in progress for others.
kdzinfo       - false
kdzdownloader - false
```

## The Gist of Things
LG KDZ firmware is and always has been one hell of a problem to work around. Many great people, from various places all over the world and the internet, have assembled over years of time in order to put their minds together and work towards a common goal. Some people viewed it as rooting their phones, and some unlocking their bootloaders; others wanted to carrier unlock, or crossflash to a different set of bands. I view all of these as the same thing: 

The right to fully own what you have purchased.


### Tools
kdz2imgs.py
- [iscgar's kdz_extractor](https://gist.github.com/iscgar/e0da0868df7b2f179b000c61f12d1a8c) script.

kdzinfo.py
- A script derived from part of the code for kdz2imgs.py, designed to print informational data about KDZ files and exit. Can assist with making patches, verifying the versions behind the KDZ, or just to generally be informative about the file.

kdzdownloader.py
- A script based off of [shinyquagsire23's lg_getkdz.py](https://gist.github.com/shinyquagsire23/0d6a5119ee7fb40de2fcfb9088168d63) designed to help pull new update files provided from various device information. Utilizes the gn_auth_model_check2.jsp API webpage. Additions include arguments to provide the choice to print the received xml response file, to download the most recent KDZ, and to specify a path for where to download one or both files. Printing and downloading parameters can be used together or by themselves. If a path isn't specified, it will by default create a new folder wherever the script is ran from called "downloads." Patches include changes to dialog and added parameters. including two help parameters (-h and --help).


## Todo
- [ ] Get everything here organized correctly
- [x] ~Make patches to kdzdumper.py~ iscgar went ahead and did this for us. Send thank yous.
- [ ] Create kdzinfo.py
- [ ] Modify kdzdownloader.py
- [x] Add special thanks section
- [ ] Add analysis reports and informational resources sections


## Special Thanks
* [iscgar](https://gist.github.com/iscgar) for the updated and functional KDZ extractor and gorgeously informational tool.
* [shinyquagsire23](https://gist.github.com/shinyquagsire23) for saving a ton of the work for us by providing an incredible base template to make something already amazing even more spectacular.
* [steadfasterX](https://github.com/steadfasterX/) for being such an incredibly productive part of this journey since long before I ever arrived, and for paving the way and inspiring me personally to take on this kind of work with LG devices.
* [Lekensteyn](https://github.com/Lekensteyn/) for some remarkable reverse engineering work and the original creation of LGLAF, as well as impressive documentation revolving around the LAF protocol.
* [cxza](https://cxzstuff.blogspot.com/) for the many, many impressions he left on shaping the overall, global development of the entirety of cracking through LG's barriers, repetetively aiding numerous people in the XDA Forums, doing fantastic work with information gathering and resource extraction, and for carrying on with his help despite more often than not going unacknowledged. 
