summary
---

captain-rum uses boomerang, a JavaScript library (by @bluemoon) that measures the page load time experienced by real users, commonly called RUM. You can find more about this handy and excellent tool here <a href="https://github.com/lognormal/boomerang/">https://github.com/lognormal/boomerang/</a>

This git repo includes some useful files to help you get startet with collecting boomerang data. Based on one of @bluemoon's suggestions to track data via beacon.gif by fetching the GET webserver method, I added some very basic and simple scripts that could be used.

usage
---

### /boomerang
/boomerang: All boomerang files needed, referenced by boomerang.include.html 

### boomerang.include.html
Snipped of code that can be used to be plugged into your page

### /scripts
* run-captain.sh: Shell script to kick off the finding of all beacon.gif GETS from apache access files into a consolidated log file. Log file will then be parsed by run-captain.pl to export into csv
* run-captain.pl: Perl script to parse and export data into comma-separated file (csv)
* crontab.txt: Sample installation of the cron to start captain-rum





