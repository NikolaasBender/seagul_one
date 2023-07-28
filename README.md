I have grand delusions of adequacy

# Components of the project
~script gstreaner~
script and configure rfd as a network interface
~ai upscale~
gen 1 base station software 
ai compressor
gen 2 base station software


# Nifty branches to investigate
- h264 encode to dl decode and super resolve
- e2e dl compression and decompression


# Wonk
- gstreamer enormous delay with h264


# 7/28/2023
Probably the first and last of these log entries because its good practice and we know how good proace goes with personal projects... Any ways, I have demo code running with RTP and Gstreamer to get video from the orangepi to the base station. This demo used ethernet, it showed that the concept works for super resolution on a video stream. This demo also got me comfortable with gstreamer. 
Now the problem, gstreamer file src does not want to operate with a serial interface. The proposed solution is to go direct from serial to h264 decode in python then to super resolution. This should be more efficient technically but is unknown which makes it scary and slow to execute. 