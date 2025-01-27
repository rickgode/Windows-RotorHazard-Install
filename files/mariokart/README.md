If this helps anyone else, here is what I did after I ssh'd into my pi rotorhazard.

Before making any changes, any currently-running RotorHazard server should be stopped.  If installed as a service, it may be stopped with a command like:
```
sudo systemctl stop rotorhazard
```
Change Directories
```
cd RotorHazard/src/server/static/audio
```
I renamed both the buzzer.mp3 and stage.mp3 by adding .old just in case I need to go back.
```
mv stage.mp3 stage.mp3.old
```
```
mv buzzer.mp3 buzzer.mp3.old
```
Now I'll download the new files from github
```
wget  https://raw.githubusercontent.com/rickgode/Windows-RotorHazard-Install/main/files/mariokart/buzzer.mp3
```
```
wget  https://raw.githubusercontent.com/rickgode/Windows-RotorHazard-Install/main/files/mariokart/stage.mp3
```
