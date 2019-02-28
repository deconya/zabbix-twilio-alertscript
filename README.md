# zabbix-twilio-alertscript
Zabbix alertscript for Twilio SMS

This is simple bash script that uses the Twilio messaging service to send alert messages. Since the script uses curl it could be easily adopted to use other SMS service providers. 

The script is based on the Slack alert script by [Eric OC](https://github.com/ericoc).

Installation
------------

The script was tested on Zabbix 3.0

Place the script in the `AlertScriptsPath` specified in your `/etc/zabbix/zabbix_server.conf`. Usually `/usr/lib/zabbix/alertscripts` and make it `chmod 750`

Only remains to setup variables in your zabbix panel in scripts section how https://www.zabbix.com/documentation/3.0/manual/config/notifications/media/script

*Phone numbers needs to start with "+" character