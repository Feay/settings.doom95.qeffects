# settings.doom95.qeffects
my settings file for qeffects running on enhanced doom95, with opengl renderer plus libretro shaders, instructions

also via programming (decompile dump) all command line switches for doom95, which seem to work when launching it from the command line
even with the new exe injection of doom95.exe with enhanced features like renderer and mouse support for win7+.....

intstructions:
## get doom95 portable, with patches, moddb.com/mods/doom95-portable
### get or own a doom wad of whatever sort...even shareware version I have 1,2, and tnt wads
### get https://github.com/libretro/glsl-shaders
### get https://github.com/crystice-softworks/QeffectsGL

# install doom95 portible, in my case my path is:
  C:\DOOM\Doom95Portable\
  the bigger doom95.exe lives here where i told it to unzip it too and a copy of cnc-ddraw config.exe
  this is what you normally interact with to config and launch doom95 portible with the patches
  place you wads in the data folder, in  my case:
  # 
    C:\DOOM\Doom95Portable\Data\GameData
# next unzip the extra shaders from https://github.com/libretro/glsl-shaders in the shaders folder, in my case:
    C:\DOOM\Doom95Portable\App\Doom\Shaders
# then unzip qeffects and place opengl32.dll and QeffectsGL.ini into the folder with the real doom95.exe in my case:
    C:\DOOM\Doom95Portable\App\Doom
# next and this part is important edit the QeffectsGL.ini as per the instructions 
    adding a [doom95.exe] section to QeffectsGL.ini
# finally, in the the \App\Doom folder with the real doom95 is a 2nd cnc-ddraw config.exe, you must use this to select the new shaders
  after you select a shader, go back up to C:\DOOM\Doom95Portable in my case and open cnc-ddraw config.exe, you can see your shader is 
  choosen now fortunate for us since it doesn't scan the shaders folder and we can't see the rest, no matter it seems to have applied 
  the one we want, for the render, which also selects openGL.
lastly launch using doom95 in C:\DOOM\Doom95Portable, which is for my case.

# ENJOY.
I have included my settings file, it seems that invalid lines are ignored and there is no commenting out characters reconized
there for i have put all the meanings on alternate lines and it seems to run well.
# Extra credit:
I have dumped all the command line switches.

screenshots:
![alt text](https://github.com/Feay/settings.doom95.qeffects/blob/main/with%20bloom%20NICE.jpg)
![alt text](https://github.com/Feay/settings.doom95.qeffects/blob/main/with%20emboss%20COOL.jpg)
    
