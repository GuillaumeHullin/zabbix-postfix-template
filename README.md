# Zabbix Postfix Monitoring
Zabbix template for Postfix SMTP server

Works for Zabbix 5.x Active Agent

## Deploy Commands

Everything is executed by only a few basic deploy scripts. 

```bash 
./deploy.sh 
# Main deploy script

./deploy-update.sh -b main
# This script will automatically pull the latest version of the branch ("main" in the example) and relaunch itself if a new version is found. Then it will run deploy.sh. Also note that any additional arguments given to this script will be passed to the deploy.sh script.
```

Finally import the template XML in Zabbix Server and attach it to your host.

## Credits

Forked from http://admin.shamot.cz/?p=424
