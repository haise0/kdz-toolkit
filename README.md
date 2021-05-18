# kdz-toolkit
A list of script tools, informational resources, and analysis reports for LG KDZ firmware files.


Disclaimer: **This is a work in progress.** 

`working-status:`
  - `kdzdumper     - somewhat`
  - `kdzinfo       - false   `
  - `kdzdownloader - false   `

## The Gist of Things
LG KDZ firmware is and always has been one hell of a problem to work around. Many great people from various places all over the world and the internet have assembled over years of time in order put their minds together and work towards a common goal. Some people viewed it as rooting their phones, and some unlocking their bootloaders; others wanted to carrier unlock, or crossflash to a different set of bands. I view all of these as the same thing: 

The right to fully own what you have purchased.


### Tools
kdzdumper.py
- A script made from [iscgar's kdz_extractor](https://gist.github.com/iscgar/e0da0868df7b2f179b000c61f12d1a8c) with patches to work around errors when dealing with some V3 KDZ files, as well as a few other ease-of-access changes and additions.

kdzinfo.py
- A script derived from part of the code for kdzdumper.py, designed to print informational data about KDZ files. Can assist with making patches, verifying the versions behind the KDZ, or just to generally be informative about the file.

kdzdownloader.py
- A script based off of [shinyquagsire23's lg_getkdz.py](https://gist.github.com/shinyquagsire23/0d6a5119ee7fb40de2fcfb9088168d63) designed to help pull new update files provided from various device information. Utilizes the gn_auth_model_check2.jsp API webpage. Additions include arguments to provide the choice to print the received xml response file, to download the most recent KDZ, and to specify a path for where to download one or both files. Printing and downloading parameters can be used together or by themselves. If a path isn't specified, it will by default create a new folder wherever the script is ran from called "downloads." Patches include changes to dialog and added parameters. including two help parameters (-h and --help).


## Todo
- [ ] Get everything here organized correctly
- [ ] Make patches to kdzdumper.py
- [ ] Create kdzinfo.py
- [ ] Modify kdzdownloader.py
- [ ] Add special thanks section
- [ ] Add analysis reports and informational resources sections
