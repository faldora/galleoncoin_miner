# galleoncoinminer
miner for galleoncoin. Updates to support other pools coming soon
You can use this miner or follow these steps
1. Download wildrig miner
2. https://github.com/andru-kun/wildrig-multi/releases/download/0.31.2/wildrig-multi-windows-0.31.2.7z
3. Extract it and change the bat code to one of the files to this
4. "
    :loop

    wildrig.exe -a sha256csm -o stratum+tcp://stratum.galleoncoin.club:4690 -u yourgalleoncoinaddress.ryan -p c=GALE --multiple-instance --opencl-launch 30

    if ERRORLEVEL 1000 goto custom
    timeout /t 5
    goto loop

    :custom
    echo Some error happened, put custom command here
    timeout /t 5
    goto loop
    "
5.Start the bat file.
Remember to change the galleoncoin address to your address where it says "yourgalleoncoinaddress"
