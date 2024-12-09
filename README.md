# DISCLAIMERS:

1.DO NOT try this if you think lower process count will definitely improve performance.

2.DO NOT try this if you want to use anything other than STEAM.

3.DO NOT try this if your CPU/GPU is from INTEL/NVIDIA.

4.DO NOT try this if you do not follow instructions thoroughly.

5.If you own a 7000 series GPU and do not care about overclocking, Linux is superior.

6.DO NOT try this if you do not have 2 SSDs or more. KEEP YOUR DATA IN ONE AND INSTALL WINDOWS ON THE OTHER ONE.

7.DO NOT try this if you do not have ETHERNET.

# Main Purpose:

I always want to game on one machine and work on the other one. But the windows is getting worse and worse with each update feature. So why not create and tweak my own iso/windows. So here is the step by step to create your own custom windows.

# Steps:

1. Download the iso file (I use Windows 10 IoT Enterprise LTSC 2021) from https://github.com/massgravel/massgrave.dev/blob/main/docs/windows_ltsc_links.md

I recommend doing this from fresh install to control variables, you can do it for win 10/11 any version. (Prefer win 10 over 11)

2. Tweaking the iso file using NTLite or other similar software. If you do not want to spend extra time on this one, it is not necessary.
https://www.ntlite.com/download/

I recommend removing all the updates you can remove(there are many it will not let you remove) and all the components, disable all the features. 

3. Donwload Rufus to install the iso to a USB drive.
https://rufus.ie/en/

4. Unplug your ethernet cable before installing windows. Go throught the normal process to the home screen(Click NO product key and DO NOT sign in your microsoft account)
5. Activate your windows using scripts from https://github.com/massgravel/Microsoft-Activation-Scripts
6. Setting up the built-in administrative account using the command line-- **net user administrator /active:yes** And swap to the administrative account
7. Install AMD chipset driver and GPU driver. Then install steam and other software you wanna use(discord,gog,epic,ea) **I have not tested any of those, only using steam and steam voice chat.**
8. Run **irm "https://christitus.com/win" | iex** from https://github.com/ChrisTitusTech/winutil to debloat windows
9. Open service and registry editor only keep these things running.
> AMD 3D V-Cache Performance Optimizer service
> 
> AMD Crash Defender Service
> 
> Bachground Tasks Infrastructure Service
>
> CoreMessaging
>
> DCOM Server Process Launcher
>
> DHCP Client
>
> Display Policy Service
>
> DNS Client
> 
> Group Policy Client
>
> Local Session Manager
>
> Network Store Interface Service
>
> Plug and Play
>
> Power
>
> Remote Procedure Call(RPC)
>
> RPC Endpoint Mapper
>
> State Repository Service
>
> System Events Broker
>
> Time Broker
>
> User Manager
>
> User Profile Service
>
> Windows Audio
>
> Windows Audio Endpoint Builder
>
> Windows Font Cache Service
>
> Winodws Managerment Instrumentation

Others need to be either set to disable/manual or delete the whole thing using regedit
