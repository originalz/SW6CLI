## Shopware 6 CLI
### Plesk Server Information
```bash
/opt/plesk/php/7.4/bin/php -d memory_limit=-1 bin/console
```
### General
```bash
about
```
```bash
help
```
```bash
list
```
### Theme
```bash
theme:compile
```
```bash
theme:create
```
### Cache
```bash
cache:clear
```
```bash
cache:warmup
```
### Plugin
```bash
plugin:refresh
```
```bash
plugin:list
```
```bash
plugin:install [--clearCache] [--activate]
```
```bash
plugin:uninstall [--clearCache]
```
```bash
plugin:activate pluginname [--clearCache]
```
```bash
plugin:deactivate pluginname [--clearCache]
```
```bash
plugin:update
```
### User
```bash
user:create username [--admin] [--email=name@domain.de] [--firstName="name"] [--lastName="name"] [--password=pwd]
```
```bash
user:change-password username
```
### Database Migrations
```bash
database:create-migration -p pluginname [--name examplename]
```
```bash
database:migrate [pluginname] [--all]
```
```bash
database:migrate-destructive [pluginname] [--all]
```
### Messenger
```bash
messenger:consume
```
### Tasks
```bash
scheduled-task:run
```
### Refresh SEO Index
```bash
dal:refresh:index
```
### Generate Media Thumbnails
First of all you need to activate the different thumbnail sizes for your media folders.
After that you need to generate those thumbnails via a command
```bash
media:generate-thumbnails
```
If you change the thumbnail sizes or add new ones you need to clear the media_thumbnail table.
Shopware doesnt check for differences in the thumbnails, just for the first addition
