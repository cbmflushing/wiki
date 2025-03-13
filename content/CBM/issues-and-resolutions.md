---
modified: 2025-03-13
---

#### Zoom unresponsive on main computer

date: 2023/09/03  
symptoms: Multiple issues, Zoom unresponsive, video feed not working  
solution: Restarting the computer. In this case, killing Zoom via task manager did not work so a computer reboot was necessary. Video issues can typically be resolved by toggling the camera in Zoom, but not this time.  
cause: Computer turned off, Tim reported Windows update then started running when computer was turned on in the morning which caused the slowdowns 

#### OpenLP display not showing up for display capture in Zoom/OBS

FYI I think I found a workaround for OBS not capturing OpenLP output. However OpenLP does the projection as of v3.0.2 now lends it to be invisible to display capture via Zoom or OBS, so the workaround is to use a browser source (e.g. use the browser song display that we're using for Zoom screensharing). See screenshot for details  
I've set up the Sunday (fullscreen webcam) with screenshare already, so everything should just work  
![[assets/openlp-display-workaround-in-obs.png]]

**References:**   
https://discuss.openlp.org/d/5661-openlp-and-obs-best-set-up-solved  
https://sites.google.com/site/anvilsoup/downloads/openlp-and-obs-integration  
[https://streamgeeks.us/dock-individual-sources-in-obs/](https://streamgeeks.us/dock-individual-sources-in-obs/)

#### Chrome window does not refresh in the background (OpenLP sharing)

**Date:** 2023/12/19

**Description:** This is an issue if using sharing the OpenLP page `http://192.168.0.66:4316/stage` on Zoom, and using `http://192.168.0.66:4316/slides` to advance the slides. If the chrome tab does not refresh in the background, then the screenshare will simply display the old slide.

**Solution:** There is a chrome flag that can be set to turn this behavior off, and allow it to refresh in the background.

1. Go to [[chrome://flags/|chrome://flags]]
2. Set the `calculate-native-win-occlusion` flag to false/off

https://support.google.com/chrome/thread/76386937?hl=en&sjid=10679465673187630674-NA