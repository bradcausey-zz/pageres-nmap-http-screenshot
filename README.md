# pageres nmap http screenshot
 modification of the http-screenshot NSE (nmap script) to use pageres on Windows.
 
Original credit, I think: Trustwave
 
 
Installation
----

First you need to install node.js 

	https://nodejs.org/en/download/package-manager/#windows

Next, run the installation for pageres-cli: 

	npm install -g pageres-cli

Then place the NSE file "http-screenshot.nse" into the scripts directory:

	c:\program files\nmap\scripts\
	
Run the update command as administrator:
	
	nmap --script-updatedb


Usage
----

include the script in your nmap command parameters:

    nmap -A --script=default,http-screenshot 192.168.1.0/24 -oA nmap-local


Links
----

* Nmap: https://nmap.org/
* NodeJS: https://nodejs.org/en/download/package-manager/#windows
* pageres: https://github.com/sindresorhus/pageres

