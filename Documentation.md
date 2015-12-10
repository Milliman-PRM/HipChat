
<head>
	<link href="css/documentation.css" rel="stylesheet">
</head>
<body>
	<a name="top"></a>
	<a name="#top"></a>
	



<p align="center">
	<b>Table of Contents</b><br>
		<a href="#usage">Usage Notes</a> |
		<a href="#resources">Resources</a> |
		<a href="#req">Requirements</a> |
		<a href="#license">License</a> |
		<a href="#ldap">LDAP Settings</a> |
		<a href="#add">More Info</a>
	<br><br>
</p>


-----------------------------------------------------------------------------------
##Usage Notes<a name="usage"></a>
Seems to be more responsive in *Chrome*


##Resources<a name="resources"></a>

Overview: 
>https://confluence.atlassian.com/hc/hipchat-server-security-648218032.html

Download: 
>https://www.hipchat.com/server/get-it

Configure:
>https://confluence.atlassian.com/hc/configuring-hipchat-server-608731851.html

Security:
>https://confluence.atlassian.com/hc/hipchat-server-security-648218032.html

When the owner account is lost by HipChat(has happened three times on me):
>https://confluence.atlassian.com/display/HIPCHATKB/Locked+out+of+the+HipChat+Server+Web+UI

##Requirements<a name="req"></a>
######Certificate
>Uses 256-bit SSL 

>May need to use root cert for integrations

######Supports VMWare
>OVA autoconfigured with the following:

>64bit Ubunutu 12.04 base OS
>4GB RAM
>74GB HDD



##License<a name="license"></a>
The License currently in use is a 30 day Trial license. 

License Manager: Alex Pegg

><a href="mailto:alex.pegg@milliman.com">Email</a>

##LDAP Settings
<a name="ldap"></a>


>Authentication User:
cn=servIndyHipchat,ou=users,ou=Indianapolis,dc=milliman,dc=com

>Base DN:
ou=Indianapolis,dc=milliman,dc=com

>Addional Users
ou=Users


>User Schema Settings:
*Only listing changes from default config
User Object Filter: (&(objectCategory=Person)(sAMAccountName=*)(memberOf=cn=Indy_HipChat,ou=Groups,ou=Indianapolis,dc=milliman,dc=com))


##Additional Settings<a name="add"></a>
>IP: 10.3.200.21
>Host name: indy-hipchat.milliman.com

<p align="center">
	<a href="#top">Top of Page</a>
</p>
</body>


