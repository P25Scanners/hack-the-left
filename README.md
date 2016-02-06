# hack-the-left

Repository created for Cop Radio project for <a href=https://noisebridge.net/wiki/HackTheLeft#Tentative_Schedule>hack-the-left<a> hackathon, happening this weekend Feb. 5-7 @ Noisebridge.

Props to <a href='https://github.com/rhodey'>rhodey</a> for writing the code-base we're going to hack on. 

To Do's: Create a rtl-sdr driver for P25 scanning.


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
