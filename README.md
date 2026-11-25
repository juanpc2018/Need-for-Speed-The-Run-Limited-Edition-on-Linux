# [Need for Speed: The Run (2011)](https://en.wikipedia.org/wiki/Need_for_Speed%3A_The_Run) Limited Edition on Linux
BlackBox version, Frostbyte 2 engine.

**The Trick to Run games on Linux is like a Combination lock...** </br>
GPU year </br>
Nvidia Propietary driver version </br>
Linux version </br>
Kernel Version </br>
DXVK version </br>
Wine version </br>

This guide may Not work on other systems with different configuration, </br>
that break the combination. </br>

Game Works at 3440x1440x50fps but requires WideScreen Fix / Patch. </br>

**Tested Working:** </br>
[pearOS 20.04.4](https://archive.org/details/pearOS_Monterey_64bit-12-beta-2021.07.01) </br>
2016 GPU [NVIDIA](https://www.techpowerup.com/gpu-specs/?mfgr=NVIDIA&year=2016) </br> 
2016 [AMD](https://www.techpowerup.com/gpu-specs/?mfgr=AMD&year=2016) GPU Unknown. </br> 
[Quadro M6000 24 GB](https://www.techpowerup.com/gpu-specs/quadro-m6000-24-gb.c2824) = [GTX 980 Ti (Q2 2015)](https://www.techpowerup.com/gpu-specs/geforce-gtx-980-ti.c2724) = [Titan X (Q1 2015)](https://www.techpowerup.com/gpu-specs/geforce-gtx-titan-x.c2632) </br>
[DXVK 1.10.0](https://github.com/doitsujin/dxvk/releases/tag/v1.10) </br>
PlayOnLinux 4.3.4 </br>
32-Bit Wine 7.9 </br>
NVIDIA Propietary Driver 470, forget about 535 & 570 with a 2016 GPU. </br>

#### HW tested: </br>
AMD 7600x </br>
[ASRock X670E PG](https://pg.asrock.com/mb/AMD/X670E%20PG%20Lightning/index.asp) UEFI v2.10 </br>
intel i3-12100 </br>
[ASRock Z790 LiveMixer](https://www.asrock.com/mb/Intel/Z790%20LiveMixer/Specification.asp) UEFI v9.04 </br>

[X] VSync in the game. </br>
[X] Vsync in NVIDIA X Settings. </br>

WQHD monitor: [LG 34GP64A](https://www.lg.com/us/monitors/lg-34gp63a-b-gaming-monitor) are 3440x1440 x 50fps using HDMI & 160fps DisplayPort. </br>

[Ubuntu 20.04.4](https://old-releases.ubuntu.com/releases/focal/) has a problem with: </br>
pulseaudio-module-jack = Not recommended for JackAudio. </br>
Should work ok:
[Kubuntu 20.04.4 LTS](https://web.archive.org/web/20220312054528/http://cdimage.ubuntu.com/kubuntu/releases/20.04.4/release/kubuntu-20.04.4-desktop-amd64.iso.torrent) | [SHA256SUM](https://web.archive.org/web/20220305015630/http://cdimage.ubuntu.com/kubuntu/releases/20.04.4/release/SHA256SUMS) | [archive](https://web.archive.org/web/20220305014143/https://cdimage.ubuntu.com/kubuntu/releases/20.04.4/release/) </br>

Probably works Ok: </br>
Kubuntu 22.04.1 </br>
[DXVK 1.10.3](https://github.com/doitsujin/dxvk/releases/tag/v1.10.3) </br>

The problem with .2 .3 .4 [.5](https://web.archive.org/web/20241008203731if_/https://cdimage.ubuntu.com/kubuntu/releases/22.04.5/release/kubuntu-22.04.5-desktop-amd64.iso.torrent) is that comes with newer versions of critical software like gcc, </br>
making very dificult to install CURL & Liquorix Kernel = Not Recommended. </br>

### Basic Rules: </br>
Wine 8.x requires newer glibc.so.6 Not available on 20.04.4 </br>
Game Launchers like [Lutris 0.5.18](https://github.com/lutris/lutris/releases) come with libraries, Not included on 20.04.4 </br>
[PlayOnLinux 4.3.4](https://www.playonlinux.com/en/download.html) depends on system libraries, but allows to most Wine versions. </br>
DXVK-2.0 does Not work with 2016 GPU's. </br>

[Wine 32-Bit Focal stable](https://gitlab.winehq.org/wine/wine/-/wikis/Debian-Ubuntu) </br>

```
$ sudo dpkg --add-architecture i386 
$ sudo mkdir -pm755 /etc/apt/keyrings
$ wget -O - https://dl.winehq.org/wine-builds/winehq.key | sudo gpg --dearmor -o /etc/apt/keyrings/winehq-archive.key -
$ sudo wget -NP /etc/apt/sources.list.d/ https://dl.winehq.org/wine-builds/ubuntu/dists/focal/winehq-focal.sources
$ sudo apt install --install-recommends winehq-stable
```

### OBS 25.03.3 
OBS can record the whole Screen with: </br>
* Screen Capture (XSHM) </br>
3D games look ok on screen, but recorded .h264 .mkv has Tearing... .mp4 untested. </br>

3D Game Requires another source with higher priority: </br>
* Window Capture (Xcomposite) </br>
[X] Lock X server when capturing BATMAN Window,</br>
Option is only visible when game is Running, Windowed. </br>
and/or Turn-Off Screen Capture (XSHM) </br>

--------------------------

**Test to see if 32-Bit 3D Vulkan VK Mesa Drivers are installed properly on the system:** </br>
[Unigine Tropics-1.3 (2008-2010)](https://benchmark.unigine.com/tropics) [.run](https://assets.unigine.com/d/Unigine_Tropics-1.3.run) [Benchmark](https://benchmark.unigine.com/) for Linux OpenGL. </br>
32/64-Bit [Heaven-4.0 (2009)](https://benchmark.unigine.com/heaven) Requires to be forced to work at 32-Bit. </br>
Optional: [Sanctuary-2.3 (2007)](https://benchmark.unigine.com/sanctuary) </br>

64-bit OS requires to [Enable 32-bit](https://gitlab.winehq.org/wine/wine/-/wikis/Debian-Ubuntu) architecture: </br>
> sudo dpkg --add-architecture i386 </br>

> $ ./1024x768_windowed.sh </br>
or... </br>
> $ ./1920x1080_windowed.sh </br>
