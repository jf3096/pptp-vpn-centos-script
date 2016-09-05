pptp-vpn-centos-script
=====================
> This is a fork from https://raw.githubusercontent.com/viljoviitanen/setup-simple-pptp-vpn/master/README.md

Since the original is not support centos due to unrecogize command of apt-get, so I instead of fork it, copy it and update it to suit my needs, as well as save it as my backup for future VPS server use.

Command
----------------------

    wget https://raw.github.com/jf3096/pptp-vpn-centos-script/master/startup.sh
    sudo sh startup.sh

Default Settings
---------------------------

Once it's installed, you will obtain a default password which are <b>username =vpn</b> <b>password = Uu8-KBb-QYd</b>

Remove it if you want it. If this gets popular, it will be a potential security loophole. Please keep in mind.

Add Account
---------------------------

    cd /etc/ppp/chap-secrets
    
Screenshot
----------------------------
![alt tag](/sample.png)

Where client is the username, server is type of service – pptpd for our example, secret is the password, and IP addresses specifies which IP address may authenticate. By setting ‘*’ in IP addresses field, you specify that you would accept username/password pair for any IP.
