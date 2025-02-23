# Pipe PoP Cache Node Documentation


# GUIDE FOR PIPE NODE DEPLYMENT

As we prepare for the testnet launch, we're introducing a new node architecture. 

DevNet 2 serves as an alpha testnet, and after maintaining stability for 40 days, the testnet will be launched.

# System Requirements 

- **Operating System:** Linux  
- **Memory:** Minimum 4GB RAM (configurable); higher RAM may yield better rewards  
- **Storage:** At least 100GB of free disk space (configurable); 200-500GB is ideal  
- **Network:** 24/7 internet connectivity required

# You will need a VPS, you can get from PQ hosting or Contabo. Buy your VPS from any of these two below
*https://contabo.com*
*https://pq.hosting/en/*


# Check Your Disk Space:

# Run the following command to verify available storage:

	df -h

Ensure you have at least 500GB of free space if you're setting --max-disk 500.

# Create new screen

	sudo apt install git -y

	sudo apt install screen

	screen -S pipe
		

# INSTALL (Copy each prompt one after the other)


	curl -L -o pop "https://dl.pipecdn.app/v0.2.8/pop"

	chmod +x pop

	mkdir download_cache




# Configuration (ADD YOUR SOLANA PUBLIC ADDRESS, CONFIGURE RAM AND DISK BASED ON YOUR OPERATING SYSTEM SPECS)

	     ./pop \
  		--ram 8 \
  		--max-disk 500 \
		--cache-dir /data \
 		--pubKey "public key"
 	        --enable-80-443
   		Restart=always
		RestartSec=5
		LimitNOFILE=65536
		LimitNPROC=4096
		StandardOutput=journal
		StandardError=journal
		SyslogIdentifier=pop-node
		WorkingDirectory=/var/lib/pop
	
# Exist Screen use ( ctrl AD) simultaneously

# Create new terminal and continue


# Add Ref

	./pop --signup-by-referral-route 91636a9cd3a3608a
# Generate your Ref
	./pop --gen-referral-route
 
# Use referral
	./pop --signup-by-referral-route <CODE>

# Monitor

# View metrics

	./pop --status

# Check points

	./pop --points

# Generate referral

	./pop --gen-referral-route
