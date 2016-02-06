# hack-the-left

Repository created for Cop Radio project for <a href=https://noisebridge.net/wiki/HackTheLeft#Tentative_Schedule>hack-the-left<a> hackathon, happening this weekend Feb. 5-7 @ Noisebridge.

Props to <a href='https://github.com/rhodey'>rhodey</a> for writing the code-base we're going to hack on. 

To Do's: Create a rtl-sdr driver for P25 scanning.


In order to write a driver for the RTL-SDR, use the USRP driver rhodey wrote as an example.....<br>
The USRP Driver : <a href= 'https://github.com/rhodey/dsp-usrp-source/search?utf8=%E2%9C%93&q=tunable&type=Code'>HERE</a>
<br><br>
Step 1. Extend the TunableSampleSource class like in the Usrp module <br>
The above USRP driver imports TunableSampleSource from <a href= 'https://github.com/rhodey/dsp-common/blob/master/src/main/java/org/anhonesteffort/dsp/sample/TunableSamplesSource.java'>Here</a>

Step 2. Implement TunableSampleSourceProvider like in UsrpProvider
UsrpProvider I believe is defined as TunableSampleSourceProvider in <a href='https://github.com/rhodey/dsp-common/blob/master/src/main/java/org/anhonesteffort/dsp/sample/TunableSamplesSourceProvider.java'>HERE</a>
