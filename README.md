ofxKinectV2-OSC
===============
Easily get the [Kinect V2 sensor](http://www.microsoft.com/en-us/kinectforwindows/purchase/)'s realtime skeleton data into openFrameworks on a Mac.

![A Kinect V2 sensor](kinect.jpg)

If you are used to using openFrameworks on a Mac, **and all you want is skeletal data**, this addon is for you.

You still need Windows
----------------------
For the foreseeable future, the Kinect V2 sensor runs only on Windows 8.1 using a USB3 port. There's no way around that, but what you can do is have a small, simple program on your Windows computer, which broadcasts to a Mac.

Then you can just leave Windows running and get back to doing the rest of your coding on a Mac. The Windows and Mac computers will of course have to be on the same network.

Instructions
------------
- On your Windows machine, follow the instructions to clone and run this repo: [KinectV2-OSC](https://github.com/microcosm/KinectV2-OSC)
- That's a little WPF app which broadcasts the Kinect's skeletal data across the network
- On your Mac, clone and run ofxKinectV2-OSC (this repo)
- Once you fire up the example, you should see a skeleton that looks a bit like you!

Screenshots
-----------
This is what you'll see on your Windows machine:

![KinectV2-OSC running on Windows](screenshot-win.png)

This is what you'll see on your Mac:

![ofxKinectV2-OSC running on Mac](screenshot-mac.png)

See the red and green hands? That's showing detection of open or closed hand states.

And the thin lines on the legs? That's where the bones are inferred (low confidence).

Project dependencies
--------------------
- [ofxOSC](https://github.com/openframeworks/openFrameworks/tree/master/addons/ofxOsc) to recieve messages - it's part of the openFrameworks core
- Tested against [openFrameworks 0.8.4](http://openframeworks.cc/download/)