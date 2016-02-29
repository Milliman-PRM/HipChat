HipChat is instant messaging for businesses that aims to integrate project-management, source-control, and many other resources into one information system. Rooms can be created for specific GitHub repositories with IM's at specified triggers. Chat rooms can be private or public and contain as many people as needed. There are commands that can be used to jump between rooms, create rooms, call an individual, etc. 

##Basic Setup
* HipChat is a virtual machine running on a local VMware ESXI Host
	* Deployed using an OVA straight from Atlassian themselves
	* Uses Ubuntu 12.04.4 LTS
* Integrated within AD; a user must be a part of the correct group to login
	* Currently by design, a user must use their email address to login. This is because HipChat pulls the email address from user accounts in AD to put in its database. This aspect is currently not customizable. 
* A DNS entry for `indy-hipchat.milliman.com` is in place
* A SHA-1 SSL Certificate is in place authenticating against corporate's own Root Cert. 
	* This certificate will be updated as soon as possible
	* Chrome and Firefox will still complain about the integrity of the certificate atm
	