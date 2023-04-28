# Event-Horizon-ES-mod

[Author profile](https://github.com/JasonWu00)

## Description

`Event-Horizon-ES-Mod` is a mod for Event Horizon (the mobile/PC game, not the movie) using assets from the open source game [Endless Sky](https://github.com/endless-sky/endless-sky). This repository contains the source files for the mod and compiled files of past versions of the mod.

## History

At around June of 2021 I decided that this project would be a good idea and started collecting assets and learning how mods for Event Horizon work. On July 14, 2021 I compiled the first version of the mod.

The first few versions were released informally on the official Discord server for Event Horizon. Later versions were released on an [itch.io page](https://404-found.itch.io/event-horizon-es-mod).

Note that the account uploading to the itch.io page uses a personal username instead of my actual name. This is because I was initially not keen on allowing random people on the Internet to know my real name.

## Questions

Q: "This isn't technically impressive. It doesn't show off any flashy or marketable skills. It won't matter for whether you get into an internship or job or not. Why are you pinning it to your profile?"

A: These statements are true and I am aware of this. I pinned this repo on my profile because it's something I put effort into and am sort of proud of.

Q: "What do all of these `.json` files do?"

A: Some helpful people over at the Event Horizon official Discord server compiled this ["Database User Manual"](https://docs.google.com/document/d/1TsxbbtUkF_OKdpotKNQEiPqvW3xi8CTUipUiFz51CZY/edit?usp=sharing) that details exactly what everything does. This manual explains everything far better than I possibly could, but it is a bit of a long read. Alternatively, you can refer to the `README.md` files in a couple of the data folders for an idea of what the `.json` files in the relevant folders mean. Note that most data folders don't have readmes.

Q: "How do I download and use this mod?"

A: To do that you will have to download Event Horizon, place the mod file into the correct location, and play the game. The steps to do this are as follows:

1. Download Event Horizon.
   - Android: from the Google Play Store.
   - PC: from [here](https://github.com/PavelZinchenko/EventHorizon-Issues/releases/tag/latest_build). Download `EventHorizon_win64.zip` to your device and extract it to a folder of your choosing.
2. Go to the location where the Event Horizon game files are stored at.
   - Android: `storage/Android/data/com.ZipasGames.EventHorizon/files`
     - Some Android devices do not allow the user to access these files through the built-in file manager. You may wish to download a file manager of your choice from the Google Play Store to aid in this step.
   - PC: wherever you placed the unzipped folder.
3. Create a folder at that location named `Mods`. Capitalization matters.
4. Download whichever version of this mod you want and move the mod file to the `Mods` folder.
5. Launch Event Horizon.
   - Android: press on the Event Horizon app icon on your device.
   - PC: Double-click on `Event Horizon.exe`.
      - Note: `Event Horizon.exe` must be in the same directory as the `Mods` folder.
6. Activate the mod.
   - Select the `"Settings"` button on the bottom right of the game's main menu.
   - Out of the six buttons on the left side of the settings menu, select the wrench and screwdriver symbol.
   - You will be shown a list of "Available modifications". Select this mod (usually titled `Endless Sky [version number]`), then select the "Yes" button on the popup warning window.
   - Wait until the game finishes activating the mod.
7. The mod is now loaded.

## Credits, Copyrights, Documentation

Specific information on credits and copyrights for this project can be found in [credits-copyright.md](../master/credits-copyright.md).  
A list of all changes to the mod can be found in [changelog.md](../master/changelog.md).  
An unorganized list of information on various mod elements can be found in [documentation.md](../master/documentation.md).  

## Licensing

Most source files in Event-Horizon-ES-Mod are licensed under a Creative Commons Attribution Share-Alike 4.0 License (see [LICENSE.md](../master/LICENSE.md)). Exceptions to this statement can be found in [credits-copyright.md](../master/credits-copyright.md).