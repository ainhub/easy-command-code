# easy-command-code
SSH Easy Login SET UP
---------------------

ssh -i ~/.ssh/KEY-PAIRS USER@IP_ADDRESS

Make it simple: So the just simple code 
ssh NAME 
can access the server

Step 1:  	Create a config file in user .ssh directory 

nano ~/.ssh/config

Step 2:		Write these line of code in the file and save:

Host  NAME
	Hostname 		HOST_NAME
	User			USER_NAME
	IdentityFile	~/.ssh/NAME OF KEY-PAIRS

	eg: 

	Host  server1
	Hostname 		10.22.123.4
	User			ec2-user
	IdentityFile	~/.ssh/mekey.pem


Step 3. Simply now able to access typing

ssh NAME
