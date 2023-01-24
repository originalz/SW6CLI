### Plesk Server Information
```bash
/opt/plesk/php/7.4/bin/php -d memory_limit=-1 bin/console
```
### General
```bash
bin/console about
```
```bash
bin/console help
```
```bash
bin/console list
```
### Theme
```bash
bin/console theme:compile
```
```bash
bin/console theme:create
```
### Cache
```bash
bin/console cache:clear
```
```bash
bin/console cache:warmup
```
### Plugin
```bash
bin/console plugin:refresh
```
```bash
bin/console plugin:list
```
```bash
bin/console plugin:install [--clearCache] [--activate]
```
```bash
bin/console plugin:uninstall [--clearCache]
```
```bash
bin/console plugin:activate "pluginname" [--clearCache]
```
```bash
bin/console plugin:deactivate "pluginname" [--clearCache]
```
```bash
bin/console plugin:update
```
### User
```bash
bin/console user:create username [--admin] [--email=name@domain.de] [--firstName="name"] [--lastName="name"] [--password=pwd]
```
```bash
bin/console user:change-password username
```
### Messenger
```bash
bin/console messenger:consume
```
### Tasks
```bash
bin/console scheduled-task:run
```
