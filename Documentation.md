#Table of Contents[1]
###Usage Notes[2]
###Resources[3]
###Requirements[4]
###License[5]
###LDAP Settings[6]
[###Addional Settings][7]



-----------------------------------------------------------------------------------
[1]:#Usage Notes
Seems to be more responsive in *Chrome*


#Resources

Overview: 
https://confluence.atlassian.com/hc/hipchat-server-security-648218032.html

Download: 
https://www.hipchat.com/server/get-it

Configure:
https://confluence.atlassian.com/hc/configuring-hipchat-server-608731851.html

Security:
https://confluence.atlassian.com/hc/hipchat-server-security-648218032.html

When the owner account is lost by HipChat(has happened three times on me):
https://confluence.atlassian.com/display/HIPCHATKB/Locked+out+of+the+HipChat+Server+Web+UI

#Requirements

-uses 256-bit SSL 
-will need to use root cert

######Supports VMWare
>OVA autoconfigured with the following
>64bit Ubunutu 12.04 base OS
>4GB RAM
>74GB HDD


#License
Atlassian Account
https://id.atlassian.com/login
email: alex.pegg@milliman.com



#LDAP Settings


Authentication User:
cn=servIndyHipchat,ou=users,ou=Indianapolis,dc=milliman,dc=com

Base DN:
ou=Indianapolis,dc=milliman,dc=com

Addional Users
ou=Users


User Schema Settings:
*Only listing changes from default config
User Object Filter: (&(objectCategory=Person)(sAMAccountName=*)(memberOf=cn=Indy_HipChat,ou=Groups,ou=Indianapolis,dc=milliman,dc=com))


#Additional Settings
IP: 10.3.200.21
Host name: indy-hipchat.milliman.com





