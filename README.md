A very dumb workaround to start asusd, still dont know why the asusd didn't run at startup tho  
How 2:
Step 1: Check ls -ld /etc/asusd  
Have file: skip 
Dont have file: sudo mkdir -p /etc/asusd  
Step 2: Download asusfix.service and run.sh  
Step 3: Move asusfix.service to /etc/systemd/system/  
        Move run.sh to /usr/local/bin/  
        sudo chmod +x run.sh  
        sudo systemctl enable asusfix.service  
Done
