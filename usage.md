# Usage !

This is the guide for using devopsark cli on your server !

# Authentication 

Step 1 : Open Terminal and type `devopsark user init devopsark.ai abcdefghijkl`
Step 2 : Open Terminal and type `devopsark switch org`
Step 3 : Open Terminal and type `devopsark switch project`

		That's It ! - CLI is now ready to use

# Agent Setup (Automated)

Step 1 : Complete Authentication 
Step 2 : Open Terminal and type `devopsark worker --autosetup`

		That's It ! - Agent is ready to use
		

# Agent Setup (Manual)

Step 1 : Complete Authentication 
Step 2 : Register Agent on devopsark portal ( https://devopsark.ai/servers/agents )
Step 3 : Open Terminal and type `devopsark switch worker`

		That's It ! - Agent is ready to use
		

# Start Agent ( foreground )

Step 1 : Once authentication and agent setup is completed
Step 3 : Open Terminal and type `devopsark worker --start-agent`

		That's It ! - Agent is up		

# Start Agent ( Background )
 
		MacOS : `nohup bash -c "devopsark worker --start-agent" > out.log 2>&1 &`
		Windows : `start "" /B cmd /c "devopsark worker --start-agent > out.log 2>&1"`
		Linux : `nohup bash -c "devopsark worker --start-agent" > out.log 2>&1 &``
		
				That's It ! - Agent will continue to run till your stop machine
				
## Note
We recommend adding agent background script to os startup execution so that you do not have to start it always manually after reboot !