pptp-vpn-centos-script
=====================
> This is a fork from https://github.com/viljoviitanen/setup-simple-pptp-vpn

Since the original is not support centos due to unrecogize command of apt-get, so I instead of fork it, copy it and update it to suit my needs, as well as save it as my backup for future VPS server use.

Command
----------------------

    wget https://raw.github.com/jf3096/pptp-vpn-centos-script/master/startup.sh
    sudo sh startup.sh

Default Settings
---------------------------

Once it's installed, you will obtain a random password such as: <b>username =vpn</b> <b>password = Uu8-KBb-QYd</b>

Add Account
---------------------------

    vi /etc/ppp/chap-secrets
    
Screenshot
----------------------------

Simply add accounts to /etc/ppp/chap-secrets :

![alt tag](/sample.png)

Where client is the username, server is type of service – pptpd for our example, secret is the password, and IP addresses specifies which IP address may authenticate. By setting ‘*’ in IP addresses field, you specify that you would accept username/password pair for any IP.
