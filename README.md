This extension was created for http://twitch.com/mtaywools, consider following her as a thank you :)

# twitch-markers
Adobe Premiere Pro Extension to import twitch "highlight markers" .csv file as markers into a premiere pro sequence

### Why?
Twitch Streamers can add highlights markers during a stream via the [Twitch Creator Dashboard interface (quick action buttons)](https://help.twitch.tv/s/article/creator-dashboard) or methods like a [streamdeck](https://www.elgato.com/en/gaming/stream-deck).

Twitch will then display these timestamped markers in the timeline of their ["Highlighter" video editing interface](https://help.twitch.tv/s/article/creating-highlights-and-stream-markers), located in the Twitch video producer page.

For an experienced video editor, the Twitch Highlighter tool is limited in editing tools, and is unreliable in saving work [(see processing queue error)](https://twitch.uservoice.com/forums/923368-video-features/suggestions/18445678-my-video-has-been-stuck-processing-for-hours?page=2&per_page=20).

Thankfully, the Twitch Highlighter has an option to export timestamped highlight markers to .csv (located in the bottom right, nested in the "..." more menu). However, Premiere Pro surprisingly does not offer a native feature to import .csv markers (adobe After Effects can, but dynamic link transfer has other issues).

So this Premiere Pro extension simply allows you to import a .csv file, and will add them into a Premiere Pro sequence.

### Notes/limitations:
- a sequence must be selected before running the extension (so the script knows where to import)
- the extension adds the markers at the sequence level (not directly onto a video layer). This is useful if you have multiple videos. However, if cut a seciton of the video, then then the markers will be misaligned. So once you have your video imported to the sequence, it is smart to nest the markered sequence into another sequence (so the markers are on a layer instead of the sequence). (welcome suggestions on how to improve this workflow)
- the .csv format the extension reads is static and specific to the .csv structure the twitch highlighter provides as of Oct 8, 2020. If the structure changes, we will update the extension. Or consider an interface to select columns. 
- the extension is not currently in the Adobe Exchange. If you have any tips on [this process](https://helpx.adobe.com/exchange/help/getting-started-developer.html), please email me at mcgrealife@gmail.com (to avoid the manual install)

### Install instructions
- [Video version here](https://youtu.be/EwPRfyijSww)
- Download the latest.zip [here](https://github.com/mcgrealife/twitch-markers/raw/main/Twitch_Markers.zip)
- Unzip the file.
- On your local drive, locate Adobe Premiere Pro's extension folder.
  - For MacOS users: ~/Library/Application Support/Adobe/CEPServiceManager4/extensions
  - For Windows users: ?
- Move the entire "Twitch_Markers" file into this folder
- Restart Premiere Pro
- In the Premiere Pro top level menu, 

### Usage Instruciotns
- [1min tutorial video](https://www.loom.com/share/1e4d9602e2b34e9cbae7089465b17765)
