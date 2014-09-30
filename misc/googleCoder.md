# Google Coder

Google Coder is a special code development environment. It can be downloaded, installed, and run from an SD card. These instructions are how to add and run the Google Coder project to an existing Raspberry Pi and running it on the local machine.

## Installation

Google Coder is a Javascript project that runs on node. Node (and assorted dependencies) must be installed first before the Google Coder project can be cloned from github.

1. If you haven't already done so, boot up the Raspberry Pi and log in. The Pi should be connected to the Internet.
2. At the bash prompt (the "**$**" followed by the blinking cursor) install nodejs (a server-side web server written in javascript), npm (a node package manager), and git (a tool for accessing code repositories: "**sudo apt-get install nodejs npm git**"
3. The installation will ask if the space required to install is ok. Type '**Y**'. 
4. Relax. (Lots of stuff will scroll past. This is normal. Let it do it's thing. It can take awhile.)
5. Download the Google Coder project from github. Type "**git clone https://github.com/googlecreativelab/coder**". Press enter.
6. Change the directory you're currently in. Type "**cd coder/coder-base/**"
7. Type "**npm install**". NPM will look at the list of Google Coder dependencies and attempt to download and install them. 
8. **IF THE SYSTEM THROWS AN ERROR IN REGARDS TO REDIS** it is a matter of switching which code registry npm is looking at. 
	1. Type "**npm config set registry http://registry.npmjs.org/**".
	2. Re-run step #7 (this will also take awhile). 

## Running Google Coder
Time to start Google Coder. 

1. Type '**startx**' at the terminal prompt.
2. When the Raspbian OS window loads, click on the "**LXTerminal**" to open a terminal inside the GUI.
3. Navigate to the "coder-base" directory. If the terminal is still in "coder-apps", type "**cd ..**" to go up a hierarchical level, and then back into the coder-base directory by typing "**cd coder-base**".
4. Start the node server for the local machine by typing "**nodejs localserver.js**". The terminal will appear to freeze. This is normal.
5. In the Raspbian OS GUI, open a web browser.
6. Type "**localhost:8080**" in the URL bar.
7. *The first time Google Coder is run* it will ask the user to set up a password. It needs to have at least two upper case characters. Take careful note of the password; *it will be needed each and every time one goes to use Google Coder*.
8. If the password was successful, use it to now log into Google Coder.

**Congratulations!** Your copy of Google Coder is ready to use!  