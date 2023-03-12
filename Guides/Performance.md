### Upscale (SSE Display tweaks) (AMD+Nvidia supported)

In this section we will be modifying the list to run at a lower resolution while outputing the game at full screen.

1. Navigate to where you instaleld Living Skyrim
2. Run ModOrganizer
3. Search for SSE Display tweaks

	![alt text](https://github.com/GamingConsultant/LivingSkyrim4/blob/main/Images/Performance/per1.PNG)
4. Right-click the mod and select Open in Explorer

	![alt text](https://github.com/GamingConsultant/LivingSkyrim4/blob/main/Images/Performance/per2.png)
5. Navigate inside SKSE\Plugins and Edit SSEDisplayTweaks.ini

	![alt text](https://github.com/GamingConsultant/LivingSkyrim4/blob/main/Images/Performance/per3.png)
6. Make the follwoing changes
	```
	BorderlessUpscale=true
	Resolution=2560x1440
	ResolutionScale=0.75
	```
