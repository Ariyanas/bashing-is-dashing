# Useful Bash Aliases
Some useful bash aliases ( personal use )
  - [For Common Bash Commands](#for-common-bash-commands)
  - [For Git Commands](#for-git)
  - [For Apache2](#for-apache2)
  - [For Web Directory](#for-web-directory)
  - [For Laravel](#for-laravel)

### For Common Bash Commands

```bash
alias cls='clear'
alias flush='source ~/.bashrc'
alias snano='sudo nano'
# for debian based system
alias update='sudo apt-get update'
alias upgrade='sudo apt-get upgrade'
alias install='sudo apt-get install'
alias u-install='apt-get install'
```

### For Git
```bash
alias gitit='sudo git init'
alias gd='sudo git add'
alias gda='sudo git add .'
alias gcmm='sudo git commit -m'
alias gcam='sudo git commit -am'
alias gca='sudo git commit -a'
alias gpush='sudo git push'
alias gpusho='sudo git push -u orign master'
alias gpushob='sudo git push -u origin "$1"'
alias gpull='sudo git pull'
alias gpullo='sudo git pull origin master'
alias gitstat='sudo git status'
```

### For Apache2
```bash
alias a2sites='cd /etc/apache2/sites-available'
alias a2sites-en='cd /etc/apache2/sites-enabled'
alias a2restart='sudo systemctl restart apache2' # add apache2.service instead of apache2 if it's not working
alias a2stop='sudo systemctl stop apache2'
alias a2start='sudo systemctl start apache2'
alias a2sites-edit='sudo "$1" /etc/apache2/sites-available/"$2"' # use 'set filename' first if it doesn't work directly
# use it like - 'a2sites-edit nano( or vim) default.conf(.conf file)
```

### For Web Directory
```bash
alias cdm='cd /var/www/html'
alias cdmp='cd /var/www/html/"$1"' # project dir name
```

### For Laravel
```bash
alias create-laravel='sudo composer create-project laravel/laravel'
alias create-laravel-dist='sudo composer create-project laravel/laravel --prefer-dist'

# for artisan commands
alias 'phart'='sudo php artisan'
alias 'pharts'='sudo php artisan serve'
alias 'phartsp'='sudo php artisan serve --port "$1"'
alias 'phtinker'='sudo php artisan tinker' # for using tinker
alias 'art'='sudo php artisan'

# migrations
alias phartm='sudo php artisan migrate'
alias phartmf='sudo php artisan migrate:fresh'
alias phartmr='sudo php artisan migrate:rollback'
alias phartmrs='sudo php artisan migrate:rollback --step="$1"' # rollback step
alias artmmi='sudo php artisan make:migration'
alias artmmi-create='sudo php artisan make:migration --create="$"'
alias artmmi-table='sudo php artisan make:migration --create="$"'

# models
alias artmmo='sudo php artisan make:model'
alias artmmo-mi='sudo php artisan make:model "$1" -m'
alias artmmo-c='sudo php artisan make:model "$1" -c'
alias artmmo-cr='sudo php artisan make:model "$1" -cr'
alias artmco-mcr='sudo php artisan make:model "$1" -mcr'

# controllers
alias artmco='sudo php artisan make:controller'
alias artmco-r='sudo php artisan make:controller "$1" -r'

# routes
alias artrt='sudo php artisan route'
alias artrt-list='sudo php artisan route:list'
```
