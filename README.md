# hack-the-left

To Do's: Create a rtl-sdr (JAVA) driver for P25 scanning.


Vision: Once an rtl-sdr driver is written, anyone can set up a police recording station for the cheap price of $19 (an rtl-sdr).  The recordings will be databased into an archive which can be used for evidence in police-related violence cases.  There is also some talk of later on running the recordings through a text-processing engine and perhaps adding some automatic functionality when search-words are found- like dropping pins on addresses, or warning people if they're near an addres.... But first, we just need a simple rtl-sdr driver. 


Repository created for Cop Radio project for <a href=https://noisebridge.net/wiki/HackTheLeft#Tentative_Schedule>hack-the-left<a> hackathon, happening this weekend Feb. 5-7 @ Noisebridge.

Props to <a href='https://github.com/rhodey'>rhodey</a> for writing the code-base we're going to hack on. 



In order to write a driver for the RTL-SDR, use the USRP driver rhodey wrote as an example.....<br>
The USRP Driver : <a href= 'https://github.com/rhodey/dsp-usrp-source/search?utf8=%E2%9C%93&q=tunable&type=Code'>HERE</a>
<br><br>
Step 1. Extend the TunableSampleSource class like in the Usrp module <br>
So the code I believe you'll be hacking on is written: <a href='https://github.com/rhodey/dsp-usrp-source/blob/a8a546435a7d5d5d903dc6c6b1cadfdf7556692f/src/main/java/org/anhonesteffort/usrp/Usrp.java'>Here</a>
<br>
Trace-back resource:
The above USRP driver imports TunableSampleSource from <a href= 'https://github.com/rhodey/dsp-common/blob/master/src/main/java/org/anhonesteffort/dsp/sample/TunableSamplesSource.java'>Here</a>
<br>

Step 2. Implement TunableSampleSourceProvider like in UsrpProvider<br>
So the code you'll be hacking on is UsrpProvider which is defined: <a href='https://github.com/rhodey/dsp-usrp-source/blob/a8a546435a7d5d5d903dc6c6b1cadfdf7556692f/src/main/java/org/anhonesteffort/usrp/UsrpProvider.java'>HERE</a>
