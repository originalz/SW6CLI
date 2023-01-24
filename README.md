### Plesk Memory Limit and PHPCli Location
```bash
remote server  > /opt/plesk/php/7.4/bin/php -d memory_limit=-1 bin/console
```
### Create Shopware Admin User
```bash
remote server  > bin/console user:create --admin --email=first.lastname@connectiv.de --firstName="firtName" --lastName="lastName" --password=pwd1423 --no-interaction userName
```
