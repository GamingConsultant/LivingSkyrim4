# Upscaling LS4

Choose only one of the following two methods

[SSE Display tweaks Upscale](#sse-display-tweaks-upscale)  
[NVIDIA Upscale](#nvidia-upscale)

## SSE Display tweaks Upscale

**AMD+Nvidia supported**

In this section we will be modifying the list to run at a lower resolution while outputting the game at full screen. This will lower the quality (depending on your setup it may or may not be noticeable)

1. Navigate to where you installed Living Skyrim
2. Run ModOrganizer
3. Search for SSE Display tweaks  
	![alt text](https://github.com/GamingConsultant/LivingSkyrim4/blob/main/Images/Performance/per1.PNG)
4. Right-click the mod and select Open in Explorer  
	![alt text](https://github.com/GamingConsultant/LivingSkyrim4/blob/main/Images/Performance/per2.png)
5. Navigate inside SKSE\Plugins and Edit SSEDisplayTweaks.ini  
	![alt text](https://github.com/GamingConsultant/LivingSkyrim4/blob/main/Images/Performance/per3.png)
6. Make the following changes  
	- Set Resolution to your monitors resolution
	- Set ResolutionScale to what you want the game to be rendered at (Resolution x ResolutionScale)
		- In this example the game will render at 1920x1080
	```
	BorderlessUpscale=true
	Resolution=2560x1440
	ResolutionScale=0.75
	```
	To revert:
	```
	BorderlessUpscale=false
	#Resolution=2560x1440
	#ResolutionScale=0.75
	```


## NVIDIA Upscale

**Only Nvidia supported**

In this section we will be modifying the list to run at a lower resolution while outputting the game at full screen. This will lower the quality (depending on the your setup it may or may not be noticeable). The difference between this way and the above is that here the driver is doing the upscaling instead of windows.
Also you get the option to sharpen the image.

1. Open Nvidia Control Panel, navigate to Manage 3D Settings > Program Settings and Select Add, then choose skyrim that's located in the folder you installed LS4

	![alt text](https://github.com/GamingConsultant/LivingSkyrim4/blob/main/Images/Performance/per5.png)
2. Select Image Scaling and choose On (GPU Scaling & Sharpening) and Apply

	![alt text](https://github.com/GamingConsultant/LivingSkyrim4/blob/main/Images/Performance/per6.png)
3. Navigate to Change Resolution and see which resoltions are available (this will be needed in step 7)

	![alt text](https://github.com/GamingConsultant/LivingSkyrim4/blob/main/Images/Performance/per7.png)
5. Navigate to where you installed Living Skyrim
6. Run ModOrganizer
7. At the top toolbar (the larger icons), select Tools then INI editor

	![alt text](https://github.com/GamingConsultant/LivingSkyrim4/blob/main/Images/Performance/per4.png)
7. Set the following values in SkyrimPrefs.ini
	- Set iSize H and iSize W to one of the Scaling Resolutions seen in step 3
	```
	[Display]
	bFull Screen = 1
	iSize H = 1108
	iSize W = 1969
	```
