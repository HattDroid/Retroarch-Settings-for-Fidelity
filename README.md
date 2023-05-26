# Retroarch-Settings-for-Fidelity
List of settings aiming to reproduce the original video game console experience... ...even if it means degrading the image a bit! 😉
This guide is currently the Miyoo Mini Plus with onionos and its implementation of RetroArch menus.
If you are missing overlays or filters, download them on onionos repository here: https://github.com/OnionUI/Onion

My setup at emulating consoles
---
	GameBoy
	---
		First make sure to follow the guide I wrote here, else you'll have settings not saving properly:
		https://www.reddit.com/r/MiyooMini/comments/13aotng/overrides_not_saving_this_might_be_the_fix/
		
		Overlays
		---
			Quick Menu
				On-Screen Overlay
					Overlay Preset
						-> GB_great.cfg

		Screen Settings
		---
			Settings
				Video
					Scaling
						-> Integer Scale	X
						-> Keep Aspect Ratio	X
					Video Filter
						-> Dot_Matrix_3x_GB_Greenscale_Grid.filt

		(Optional) Gambatte core specific
		---
			Quick Menu
				Core Options
					Color Correction
						-> GBC Only
---
	GameBoy Color
	---
		Overlays
		---
			Quick Menu
				On-Screen Overlay
					Overlay Preset
						-> GBCL.cfg

		Screen Settings
		---
			Settings
				Video
					Scaling
						-> Integer Scale	X
						-> Keep Aspect Ratio	X
					Video Filter
						-> Dot_Matrix_3x_GB_DMG_Grid.filt
---
	GameBoy Advance
	---
		Overlays
		---
			Quick Menu
				On-Screen Overlay
					Overlay Preset
						-> GBA_3x_pixel.cfg

		Screen Settings
		---
			Settings
				Video
					Scaling
						-> Integer Scale	-
						-> Keep Aspect Ratio	X
---
	Playstation
	---
		Dithering
		---
			Some games relied heavily on dithering to stylize their graphics. While reducing actual color depth, it truly looks more original to real hardware when enabled.

			Quick Menu
				Core Options
					Video
						-> Dithering Patterns	X

		Overlays
		---
			Quick Menu
				On-Screen Overlay
					Overlay Preset
						-> CRT_Scanlines_2x.cfg or Scanlines_2px_100.cfg

		Screen Settings
		---
			Settings
				Video
					Scaling (no way to formally respect scaling since every game had multiple resolutions, luckily the 640x480 screen here is doing the magic of having perfect scaling anyway in this case)
						-> Integer Scale	-
						-> Keep Aspect Ratio	-
					No way to put filters, emulation would simply be too slow.
---
	SNES
	---
		Overlays
		---
			Quick Menu
				On-Screen Overlay
					Overlay Preset
						-> bezels/SNES/default.cfg

		Screen Settings
		---
			Settings
				Video
					Scaling
						-> Integer Scale	X
						-> Keep Aspect Ratio	-
					Video Filter
						-> Scanline2x.filt	(if perf issues, this is likely the reason, watch out with Starfox, Yoshi's Island and such)
---
	NES
	---
		Screen Settings
		---
			Settings
				Video
					Scaling
						-> Integer Scale	X
						-> Keep Aspect Ratio	-
					Video Filter
						-> Scanline2x.filt
---
	Sega Mega Drive / Genesis
	---
		Overlays
		---
			Quick Menu
				On-Screen Overlay
					Overlay Preset
						-> bezels/genesis/default.cfg
		
		Screen Settings
		---
			Settings
				Video
					Scaling
						-> Integer Scale	X
						-> Keep Aspect Ratio	X
					Video Filter
						-> Scanline2x.filt
---
	Sega Game Gear
	---
		Overlays
		---
			Quick Menu
				On-Screen Overlay
					Overlay Preset
						-> GG/GG-480p-final.cfg
		
		Screen Settings
		---
			Settings
				Video
					Scaling
						-> Integer Scale	X
						-> Keep Aspect Ratio	X
---
	NeoGeo / Arcade all other home consoles
	---
		Overlays
		---
			Quick Menu
				On-Screen Overlay
					Overlay Preset
						-> CRT_Scanlines_2x.cfg
						-> CRT_Scanlines_2x.cfg or Scanlines_2px_100.cfg

		Screen Settings
		---
			Settings
				Video
					Scaling
						-> Integer Scale	? (try to activate it but depends a lot on what was the OG resolution, this could be too small or simply broken)
						-> Keep Aspect Ratio	X (most of the time, it's a mistake, since games were meant to be slightly stretched horizontally)
					
