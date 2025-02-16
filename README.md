**Pipe PoP Cache Node Documentation**


**GUIDE FOR PIPE NODE DEPLYMENT**


As we prepare for the testnet launch, we're introducing a new node architecture. 

DevNet 2 serves as an alpha testnet, and after maintaining stability for 40 days, the testnet will be launched.



**System Requirements**  

- **Operating System:** Linux  
- **Memory:** Minimum 4GB RAM (configurable); higher RAM may yield better rewards  
- **Storage:** At least 100GB of free disk space (configurable); 200-500GB is ideal  
- **Network:** 24/7 internet connectivity required

**Check Your Disk Space:**

**Run the following command to verify available storage:**

	df -h

Ensure you have at least 500GB of free space if you're setting --max-disk 500.
		

**INSTALL (Copy each prompt one after the other)**


	curl -L -o pop "https://dl.pipecdn.app/v0.2.5/pop"

	chmod +x pop

	mkdir download_cache




**Configuration (ADD YOUR SOLANA PUBLIC ADDRESS, CONFIGURE BASED ON YOUR OPERATING SYSTEM SPECS)**

	     ./pop \
  		--ram 8 \
  		--max-disk 500 \
		--cache-dir /data \
 		--pubKey "public key"
	

**Create new terminal and continue**


**Add Ref**

	./pop --signup-by-referral-route 39c3bfb0765b7dff




**Monitor**

View metrics

	./pop --status

Check points

	./pop --points

