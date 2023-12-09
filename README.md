# **Windows Operating System**&#x20;

The RotorHazard server may be run on any computer with an operating system that supports Python. In these alternate configurations, one or more hardware nodes may be connected via USB -- see [doc/USB Nodes.md](https://github.com/RotorHazard/RotorHazard/blob/v4.0.0/doc/USB%20Nodes.md) for more information. The server may also be run using simulated (mock) nodes.

Install the RotorHazard server on Windows:

1. If the computer does not already have Python installed, download and install Python from <https://www.python.org/downloads/windows/>. For RotorHazard 4.0.0 you **MUST INSTALL** Python **3.11.7** (or earlier)  The minimum version of Python needed for RotorHazard is 3.7. To check if Python is installed and the version, open up a command prompt and enter \[python –version]  If you installed Python 3.12 you might get errors
2. The next thing you will need to install is the Visual Studio Installer.  In the Workloads tab on the top make sure and check “Desktop Development with C++ and install that.
3. From the RotorHazard [Releases page on github](https://github.com/RotorHazard/RotorHazard/releases), download the "Source code (zip)" file.
4. Unzip the downloaded file into a directory (aka folder) on the computer.  I suggest C:\Users\\{username}\\
5. Open up windows file explorer and navigate to C:\Users\\{username}\RotorHazard4.0.0\src\server directory then click in the address bar and type “cmd” it will open a command prompt in the correct directory

```
python -m pip install -r reqsNonPi.txt
```

6. Copy Config File

In the "src/server" directory, copy the config-dist.json file to config.json:

```
copy config-dist.json config.json
```

7.  Edit the Config file

You can open up notepad with a command to edit the config.json file.

```
notepad config.json
```

edit the config.json file and modify the ADMIN\_USERNAME and ADMIN\_PASSWORD values. These are the login credentials you will need to enter (in the browser popup window) to access the pages reserved for the race director (i.e., the Settings and Run pages).

This is also a good time to edit the com part
