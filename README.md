# [Need for Speed: The Run (2011)](https://en.wikipedia.org/wiki/Need_for_Speed%3A_The_Run) Limited Edition on Linux
BlackBox version, Frostbyte 2 engine.
[GOG](https://www.gog.com/dreamlist/game/need-for-speed-the-run-2011) </br>

**The Trick to Run games on Linux is like a [Combination Lock](https://en.wikipedia.org/wiki/Combination_lock)...** </br>
GPU year </br>
Nvidia Propietary driver version </br>
Linux version </br>
Kernel Version </br>
DXVK version </br>
Wine version </br>

This guide may Not work on other systems with different configuration, </br>
that jam the lock. </br>

Game Works at 3440x1440x50fps but requires WideScreen Fix / Patch. </br>
NFS The Run is smart.. </br>
during intermision screens / menus lowers FPS, to allow GPU to cool down. </br>

https://nfsmods.xyz/search?search=nfs&game=11&category=0&order=1&showAllNFS=0 </br>
https://nfsmods.xyz/search?search=fix&game=11&category=0&order=1&showAllNFS=0 </br>
https://nfsmods.xyz/search?search=run&game=11&category=0&order=1&showAllNFS=0 </br>

https://nfsmods.xyz/mod/282 </br>
https://nfsmods.xyz/mod/3251 </br>
https://nfsmods.xyz/mod/5373 </br>
https://nfsmods.xyz/mod/4918 </br>
https://nfsmods.xyz/mod/4904 </br>
https://nfsmods.xyz/mod/5541 </br>
https://nfsmods.xyz/mod/4920 </br>
https://nfsmods.xyz/mod/3472 </br>
https://nfsmods.xyz/mod/2852 </br>
https://nfsmods.xyz/mod/4919 </br>
https://nfsmods.xyz/mod/4921 </br>
https://nfsmods.xyz/mod/6287 </br>
https://nfsmods.xyz/mod/6841 </br>
https://nfsmods.xyz/mod/7701 </br>

EA shut down servers, All On-line features are Disabled / Missing. </br>
The Run will softlock on "Connecting to Autolog servers..." screen during startup.  </br>
Fusion Fix bypass login prompts, saving from having to block the game in Windows Firewall. </br>

Frostbite 2 engine, packs video assets inside compiled archive chunks (.sb and .toc files) rather than loose .bik files like Batman: Arkham Asylum. </br>
Deleting or altering those archive files will break the game or cause it to crash on launch. </br>

skip intro videos & logo screens by using a lightweight ASI plugin NFS The Run Fusion Fix: </br>

https://github.com/KilLo445/NFSPatcher </br>
https://github.com/KilLo445/NFSPatcher/releases </br>
Patcher Requires NET480/481, Mono does Not work. </br>
https://dotnet.microsoft.com/en-us/download/dotnet-framework/thank-you/net48-offline-installer </br>

v1.0.4 </br>

    Need for Speed 2 SE
    Need for Speed III: Hot Pursuit
    Need for Speed: High Stakes
    Need for Speed: Hot Pursuit 2
    Need for Speed: Underground
    Need for Speed: Underground 2
    Need for Speed: Most Wanted (2005)
    Need for Speed: Carbon
    Need for Speed: The Run

https://github.com/ThirteenAG/WidescreenFixesPack </br>
https://github.com/ThirteenAG/WidescreenFixesPack/releases </br>
**TheRun** </br>
https://github.com/ThirteenAG/WidescreenFixesPack/releases/tag/nfstherun </br>


**Tested Working:** </br>
[pearOS 20.04.4](https://archive.org/details/pearOS_Monterey_64bit-12-beta-2021.07.01) </br>
2016 GPU [NVIDIA](https://www.techpowerup.com/gpu-specs/?mfgr=NVIDIA&year=2016) </br> 
2016 [AMD](https://www.techpowerup.com/gpu-specs/?mfgr=AMD&year=2016) GPU Unknown. </br> 
[Quadro M6000 24 GB](https://www.techpowerup.com/gpu-specs/quadro-m6000-24-gb.c2824) = [GTX 980 Ti (2015)](https://www.techpowerup.com/gpu-specs/geforce-gtx-980-ti.c2724) = [Titan X (2015)](https://www.techpowerup.com/gpu-specs/geforce-gtx-titan-x.c2632) </br>
[DXVK 1.10.0](https://github.com/doitsujin/dxvk/releases/tag/v1.10) </br>
[PlayOnLinux 4.3.4](https://www.playonlinux.com/en/download.html) </br>
32-Bit Wine 7.9 </br>
NVIDIA Propietary Driver 470, forget 535 & 570 with 2016 GPU's. </br>

#### HW tested: </br>
AMD 7600x </br>
[ASRock X670E PG](https://pg.asrock.com/mb/AMD/X670E%20PG%20Lightning/index.asp) UEFI v2.10 </br>
intel i3-12100 </br>
[ASRock Z790 LiveMixer](https://www.asrock.com/mb/Intel/Z790%20LiveMixer/Specification.asp) UEFI v9.04 </br>

[_] VSync Dissablen in the game, limits to 30fps. </br>
[X] Vsync in NVIDIA X Server Settings, does Not affect VK drivers. </br>

WQHD monitor: </br>
[LG 34GP64A](https://www.lg.com/us/monitors/lg-34gp63a-b-gaming-monitor) </br>
3440x1440 x 50fps using HDMI & 160fps DisplayPort. </br>
HDMI looks higher quality, more color depth bits, </br>
DP seems h.264 compressed, requires different color settings. </br>

[Ubuntu 20.04.4](https://old-releases.ubuntu.com/releases/focal/) has a problem with: </br>
pulseaudio-module-jack = Not recommended for JackAudio. </br>
Should work ok:
[Kubuntu 20.04.4 LTS](https://web.archive.org/web/20220312054528/http://cdimage.ubuntu.com/kubuntu/releases/20.04.4/release/kubuntu-20.04.4-desktop-amd64.iso.torrent) | [SHA256SUM](https://web.archive.org/web/20220305015630/http://cdimage.ubuntu.com/kubuntu/releases/20.04.4/release/SHA256SUMS) | [archive](https://web.archive.org/web/20220305014143/https://cdimage.ubuntu.com/kubuntu/releases/20.04.4/release/) </br>

**Probably works:** </br>
[Kubuntu 22.04.1](https://web.archive.org/web/20221008203731if_/https://cdimage.ubuntu.com/kubuntu/releases/22.04.1/release/kubuntu-22.04.1-desktop-amd64.iso.torrent) </br>
Depends on GPU & Nvidia propietary driver version: </br>
[DXVK 1.10.1](https://github.com/doitsujin/dxvk/releases/tag/v1.10.1) </br>
[DXVK 1.10.2](https://github.com/doitsujin/dxvk/releases/tag/v1.10.2) </br>
[DXVK 1.10.3](https://github.com/doitsujin/dxvk/releases/tag/v1.10.3) </br>

The problem with .2 .3 .4 [.5](https://web.archive.org/web/20241008203731if_/https://cdimage.ubuntu.com/kubuntu/releases/22.04.5/release/kubuntu-22.04.5-desktop-amd64.iso.torrent) </br>
is that comes with newer versions of critical software like gcc </br>
making very dificult to install CURL & Liquorix Kernel = Not Recommended. </br>
Updating 22.04.1 to .5 Not Recomended. </br>

### Basic Tips & Rules: </br>
Games Require Lowlatency Kerner or Liquorix Kernel </br>
6.3.13-1-liquorix-amd64 #1 ZEN SMP PREEMPT liquorix 6.3-13ubuntu1~focal (2023-08-06) x86_64 x86_64 x86_64 GNU/Linux
is the last for 20.04.x </br>
requires manual compile, Not available on Liquorix Repo anymore. </br>
22.04.1 still available. </br>
Wine 8.x requires newer glibc.so.6 Not available on 20.04.4 </br>
Game Launchers like [Lutris 0.5.18](https://github.com/lutris/lutris/releases) come with libraries, Not included on 20.04.4 </br>
[PlayOnLinux 4.3.4](https://www.playonlinux.com/en/download.html) depends on system libraries, but allows to download most Wine versions. </br>
DXVK-2.0 does Not work with 2016 GPU's. </br>

**System Wine Not needed:** </br>
[Wine 32-Bit Focal stable](https://gitlab.winehq.org/wine/wine/-/wikis/Debian-Ubuntu) </br>

```
$ sudo dpkg --add-architecture i386 
$ sudo mkdir -pm755 /etc/apt/keyrings
$ wget -O - https://dl.winehq.org/wine-builds/winehq.key | sudo gpg --dearmor -o /etc/apt/keyrings/winehq-archive.key -
$ sudo wget -NP /etc/apt/sources.list.d/ https://dl.winehq.org/wine-builds/ubuntu/dists/focal/winehq-focal.sources
$ sudo apt install --install-recommends winehq-stable
```

--------------------------

**Test to see if 32-Bit 3D Vulkan VK Mesa Drivers are installed properly on Linux:** </br>
[Unigine Tropics-1.3 (2008-2010)](https://benchmark.unigine.com/tropics) [.run](https://assets.unigine.com/d/Unigine_Tropics-1.3.run) [Benchmark](https://benchmark.unigine.com/) for Linux OpenGL. </br>
32/64-Bit [Heaven-4.0 (2009)](https://benchmark.unigine.com/heaven) Requires to be forced to run at 32-Bit. </br>
Optional: [Sanctuary-2.3 (2007)](https://benchmark.unigine.com/sanctuary) </br>

64-bit OS requires: [Enable 32-bit](https://gitlab.winehq.org/wine/wine/-/wikis/Debian-Ubuntu) architecture: </br>
> sudo dpkg --add-architecture i386 </br>

> $ ./1024x768_windowed.sh </br>
or... </br>
> $ ./1920x1080_windowed.sh </br>

-----------------------------

Install DXVK.dlls on Winprefix "Virtual Windows dos_c drive" from Linux </br> 
$ export WINEPREFIX=/home/user/.PlayOnLinux/wineprefix/x32_7.9 </br> 
cd /dxvk-1.10.0
$ ./setup_dxvk.sh install

-----------------------------

### OBS 25.03.3 
OBS can record the whole Screen with: </br>
* Screen Capture (XSHM) </br>
3D games look ok on screen, but recorded .h264 .mkv has Tearing... .mp4 untested. </br>

3D Game Requires another source with higher priority: </br>
* Window Capture (Xcomposite) </br>
[X] Lock X server when capturing BATMAN Window,</br>
Option is only visible when game is Running, Windowed. </br>
and/or Turn-Off Screen Capture (XSHM) </br>

--------------------------------

<img width="3440" height="1440" alt="Screenshot_20261124_215736" src="https://github.com/user-attachments/assets/e1d3c32a-1e08-495e-b6a2-05fc37e495fc" />
<img width="3440" height="1440" alt="Screenshot_20261124_222921" src="https://github.com/user-attachments/assets/c4b183a0-2ef6-4eca-b92b-1e9e388afe7c" />
<img width="3440" height="1440" alt="Screenshot_20261124_220657" src="https://github.com/user-attachments/assets/9ab534a5-0e80-4261-bcb5-e07443d46d5b" />
<img width="3440" height="1440" alt="Screenshot_20261124_214843" src="https://github.com/user-attachments/assets/5e2c1f64-c3fa-4538-be16-4e0b594ed84e" />

