# hack-the-left

Repository created for Cop Radio project for <a href=https://noisebridge.net/wiki/HackTheLeft#Tentative_Schedule>hack-the-left<a> hackathon, happening this weekend Feb. 5-7 @ Noisebridge.

Props to <a href='https://github.com/rhodey'>rhodey</a> for writing the code-base we're going to hack on. 

To Do's: Create a rtl-sdr driver for P25 scanning.


In order to write a driver for the RTL-SDR, use the USRP driver rhodey wrote as an example.....<br>
Step 1. Extend the TuneableSampleSource class like in the Usrp module <br>
Step 2. Implement TuneableSampleSourceProvider like in UsrpProvider

