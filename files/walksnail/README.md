If this helps anyone else, here is what I did after I ssh'd into my pi rotorhazard
```
cd RotorHazard/src/server/static
```
I renamed the rotorhazard.js by adding .old just in case I need to go back.
```
mv rotorhazard.js rotorhazard.js.old
```
Now I'll download the new rotorhazard.js from github
```
wget  https://raw.githubusercontent.com/rickgode/Windows-RotorHazard-Install/main/files/walksnail/rotorhazard.js
```
