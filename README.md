# bash-aliases
Some useful bash aliases ( personal use )

### Common Bash Commands

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

### For Laravel
```bash
alias create-laravel='sudo composer create-project laravel/laravel'
alias create-laravel-dist='sudo composer create-project laravel/laravel --prefer-dist'
```
