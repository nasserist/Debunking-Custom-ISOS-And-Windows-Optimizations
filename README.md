# Debunking-ISOS-&-Windows-Optimizations

W10 VS W11?
- This has already been debunked, no difference
- https://github.com/fr33thytweaks/W10-W11-Admin-Benchmarks
- Because of this, w11 has been chosen for most custom ISO'S tested

ISOS TESTED
- FR33THY W11 23h2 & Opti Guide https://github.com/fr33thytweaks/Ultimate-Windows-Optimization-Guide
- AtlasOS W11 23h2 https://atlasos.net/
- ReviOS W11 23h2 https://revi.cc/
- KirbyOS W11 23h2 https://x.com/NPKirbyy
- GhostSpectreOS W11 23h2 Superlite https://docs.google.com/document/d/15tvRU9Bs_7qcHr0kb5E603A7PsZYYBtKOfc71Rmjbv4/edit
- FoxOS W11 23h2 https://discord.com/invite/4Gg8n6WhPN
- XoxOS W11 23h2 https://discord.com/invite/XTYEjZNPgX
- KernelOS W11 23h2 https://discord.com/invite/kernelos
- GgOS W10 20h2 (MW2, MW3, Fortnite Not Supported) https://discord.com/invite/A5BHSQV
- XLiteOS W11 24h2 https://windowsxlite.com/ultralight/
- W10Stock 22h2 (HAGS ON, VBS OFF, UAC OFF, LOCAL ACT) https://www.microsoft.com/en-au/software-download/windows10
- W11Stock 23h2 (HAGS ON, VBS OFF, UAC OFF, LOCAL ACT) https://www.microsoft.com/en-au/software-download/windows11
- 2025Server W11 24h2 (Converted to full version & activated) https://www.microsoft.com/en-us/evalcenter/download-windows-server-2025
- 2022Server W10 21h2 (Converted to full version & activated) https://www.microsoft.com/en-us/evalcenter/evaluate-windows-server-2022

Testing LTSC is unnecessary since it's essentially a branch of standard Windows builds with some bloat removed and only security updates.

CONSIDER BENCHMARK VARIATION
- insert benchmarks here

CONCLUSION <br>
When considering benchmark variations, it's clear that custom ISOs are obsolete. Most Windows optimizations offer little to no performance gains. <br>
The exception lies with low-end hardware, where minimal background processes and disabling Windows Defender can provide noticeable improvements due to cpu usage. <br>
This likely explains the benchmark differences often seen when people promote custom ISOs—most of the time, these tests are conducted on systems with low-end CPUs. <br>
Why risk installing a custom ISO that could contain malware, spyware, keyloggers, or even bitcoin miners? <br>
A vanilla Windows installation is sufficient, safe and you can achieve optimizations using simple scripts instead (if needed).

WHAT ABOUT LATENCYMON BENCHMARKS? <br>
https://www.resplendence.com/latencymon <br>
https://learn.microsoft.com/en-us/windows-hardware/test/wpt/ <br>
LatencyMon and Xperf are only useful for diagnosing driver issues or audio dropouts related to drivers. <br>
Over the years, their purpose has been misunderstood in tweaking communities, with many mistakenly believing they measure real end-to-end latency. <br>
In reality, driver latency is just a minor part of the overall latency chain, so obsessing over LatencyMon or Xperf results is a waste of time. <br>
https://www.nvidia.com/en-au/geforce/guides/system-latency-optimization-guide/

Real throughput latency is what truly matters and should be the focus when comparing optimizations. <br>
NVIDIA has made it easy to measure this without the need for special tools by using Reflex-supported games and the latency stats available in FrameView or the GeForce overlay.<br>
https://youtu.be/FtWyscCu9KU

WHAT REALLY MATTERS THEN? <br>
It all boils down to the basics. Here’s my take on what truly matters when optimizing for more frames and lower latency. <br>
I'm planning to demonstrate scaling with these factors in future videos, but for now, here are my thoughts. <br>

- Fastest gaming CPU to spit out frames (keep up with the GPU)
- Fastest gaming GPU to spit out frames (keep up with the CPU, resolution and game settings) (help maintain lower GPU usage)
- Ram optimizations (decent ram kit, using xmp,docp or expo) (speed up the CPU)
- Fastest high refresh rate monitor (includes lower res)
- Oled instead of VA, IPS and TN
- Lowest latency mouse
- Lowest latency keyboard
- Overclocking Ram, CPU and GPU to make your components run faster
- Stability, an unstable system will cause framerate and latency issues
- Good/performance graphic driver settings
- Good/Low game config and in game settings (to achieve higher fps and lower gpu usage)
- Lowering resolution, dlss or fsr techniques (to achieve higher fps and lower gpu usage)
- Nvidia reflex on + boost, will drastically lower your latency in a gpu bound situation
- As discussed here, the conclusion is that Defender and background bloat primarily impact low-end CPUs and systems the most.
- Background programs running that use CPU, GPU usage

SYSTEM
- MSI MPG 321URX 240hz 4k QD OLED (4k tests in 4k resolution, 1080p tests in 1080p resolution. Both display scaled)
- 7950x3d (ccd1 disabled), = 7800x3d
- PBO enabled, -10 all core, +200mhz
- 4090 Gigabite OC, stock voltage, 2900mhz core, 11000 memory, 85% fan speed
- Asrock Steel Legend x670e, BIOS 3.01
- 4x16gb 6000mhz c30 m die gskill, dual rank
- Corsair ram fan, full speed
- Buildzoids basic timings, https://www.youtube.com/c/actuallyhardcoreoverclocking
- VDDIO / MVDD / MVDDQ: 1.35V
- VSOC: 1.25V
- tCL: 30
- tRCD: 38
- tRP: 38
- tRAS: 30
- tRC: 68
- tWR: 48
- tREFI: 50000
- tRFC: 500
- tRFC2: 400
- tRFC4: 300
- tRTP: 12
- tRRD_L: 8 
- tRRD_S: 4
- tFAW: 20
- tWTR_L: 16
- tWTR_S: 6
- tRDRDSCL: 4
- tRDRDSC: 1
- tRDRDSD: 8 (auto)
- tRDRDDD: 11 (auto)
- tWRWRSCL: 4
- tWRWRSC: 1
- tWRWRSD: 8 (auto)
- tWRWRDD: 11 (auto)
- tWRRD: 2
- tRDWR: 16
- FCLK: 2000
- UCLK: 3000
- MCLK: 3000
- Thermaltake 1050w
- Lian Li 011
- x6 Arctic fans, full speed
- Arctic Freezer III 360, full speed
- Samsung 970 pro 1tb

TOOLS
- Driver 560.81, https://us.download.nvidia.com/Windows/560.81/560.81-desktop-win10-win11-64bit-international-dch-whql.exe
- Frameview, measure, https://www.nvidia.com/en-au/geforce/technologies/frameview/
- Capframe X, compare, https://www.capframex.com/
- External latency end to end tool, including Logitech G303 Shroud Edition latency, build guide here soon
- Geforce in game latency flash, https://nvidia.custhelp.com/app/answers/detail/a_id/5175/~/what-is-the-%E2%80%9Cflash-indicator%E2%80%9D-or-%E2%80%9Clatency-flash%E2%80%9D-option-in-my-nvidia

BENCHMARKS
- Call Of Duty III
- Counter Strike 2, https://steamcommunity.com/workshop/filedetails/?id=3240880604
- Fortnite, https://dropnite.com/map.php?id=1682
- Forza Horizon 5
- Hitman 3
- Rainbow 6, vulkan
- Call Of Duty II

CONFIGS
- Rebar forced on for all titles, rebar forced off mw2 and mw3, via inspector https://github.com/Orbmu2k/nvidiaProfileInspector/releases
- All low, ultra textures, ultra AF
- 1080p & 4k
- Config files included here

TO KEEP IT FAIR all installs are using the same
- Graphics card overclock
- Nvidia driver settings/inspector settings
- BIOS settings
- Game configs
- Game launcher settings (hardware accel off, overlay off etc)
- Any post install optimization scripts included in the ISO's were ran (besides Nvidia driver settings/inspector settings)
- Stock W10 Pro ISO tests = HAGS on, VBS off, UAC disabled, Local Account. (HAGS off by default, VBS off by default, UAC on by default)
- Stock W11 Pro ISO tests = HAGS on, VBS off, UAC disabled, Local Account. (HAGS on by default, VBS on by default, UAC on by default)
