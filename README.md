# Foxit_PDF_Reader

This is a download for the latest (now deprecated by Foxit, unfortunately) version for Linux. 

Foxit makes a free PDF reader here: https://www.foxit.com/pdf-reader/. 

It used to be available for **Windows**, **macOS**, and **Linux**, but they've discontinued the Linux version. Here is the last Linux version I had downloaded before they quit hosting it in the last couple years.


# Tested on

1. `FoxitReader.enu.setup.2.4.5.0727.x64.run.tar.gz`:
    1. [x] Ubuntu 22.40. It works, but is flaky and tends to crash a lot the first time it is run. Run `pkill -f foxit` to kill it if it crashes, then reopen it. Repeat this cycle until it quits crashing. Once you get an open instance that doesn't crash, it tends to stay open reliably. Just drag PDFs from your file manager into the Foxit Window to open them. Do not close and reopoen the reader each time or it may crash more and you'll get back into the crash cycle again. 


# TODO

1. [ ] Try wrapping the latest (which is still old) Linux version in the proper older Ubuntu Docker container to make it run smoother with fewer crashes. Use x window forwarding out of the container or whatever to get the GUI to show up in your main OS. 
1. [ ] Try the latest Windows install on Linux via Wine. If you get that working, consider Dockerizing it for easier deployment and installation.
