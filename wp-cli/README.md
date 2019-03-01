## Content: WP CLI
WordPress Command Line Interface

- [Theming](#theming)
- [Plugins](#plugins)
- [Core - Updating](#updating)
- [Core - Installation](#installation)

## Theming
Command | Description
--- | --- 
`wp theme list status=active` | Show active theme

## Plugins
Command | Description
--- | --- 
`wp plugin list` | Get list of installed plugins
`wp plugin activate my_plugin` | Activate plugin my_plugin
`wp plugin deactivate my_plugin` | Deactivate plugin my_plugin

## Core features
### Updating
Command | Description
--- | --- 
`wp core update` | Updates core to newer version
`wp core update --minor` | Updates core to a new minor version
`wp core update --version=VERSION_NUMBER --force` | Use `--force` flag only on downgrades scenarios 

### Installation
Command | Description
--- | --- 
`wp core download --locale=es_ES [--path=myfolder --debug]` | Download WP with *(optional)* a specified locale
`wp config create --dbname=<your_db_name> --dbuser=<your_db_user_name> --dbpass=<your_db_user_password> --dbprefix=<your_prefix_>` | **Create configuration file** with base *(to me)* instructions
`wp db create` | **Create database** based on recent created configuration file
`wp core install --title=<site_title> --admin_user=<site_admin_username> --admin_password=<site_admin_password> --admin_email=<site_admin_email> --url=<site_url>` | **Install WP** *(the well known 5 minutes process now in seconds!)* ...
`wp core version` | Verified WordPress core version installed
