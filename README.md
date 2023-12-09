# SamsungInternetAnalyserNodeDupePoC
WebAudio API AnalyserNode duplicate data

Hello,
Calling `AnalyserNode.getFloatFrequencyData` or `AnalyserNode.getByteFrequencyData` in a loop using `requestAnimationFrame` results in a lot of duplicate data or "frames", since I'm using it to create a visualization of an audio file's frequencies.
The same works smoothly on Chrome/Chromium based browsers on Android and PC.
Here's a PoC I made:<br/>
code: https://github.com/sickl8/samsungInternetPoC<br/>
demo on vercel: https://si-analysernode-dupe-poc.vercel.app/<br/>
Here's a another website that also shows the issue: https://webaudioapi.com/samples/visualizer/
