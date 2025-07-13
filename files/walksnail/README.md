If this helps anyone else, here is what I did after I ssh'd into my pi rotorhazard.

Before making any changes, any currently-running RotorHazard server should be stopped.  If installed as a service, it may be stopped with a command like:
```
sudo systemctl stop rotorhazard
```
Change Directories
```
cd RotorHazard/src/server/static
```
I renamed the rotorhazard.js by adding .old just in case I need to go back.
```
mv rotorhazard.js rotorhazard.js.old
```
Now I'll download the new rotorhazard.js from github change the folder to 4.2 for an older version
```
wget  https://raw.githubusercontent.com/rickgode/Windows-RotorHazard-Install/main/files/walksnail/4.3/rotorhazard.js
```
