# Custom config for support bash or zsh :computer:

1. Aliasas
1. Function

Copy all files on `config` directory to your home directory: `$HOME/.config`

Then you can rename or copy file `.env.example` to `.env`

Add script to load `functions` and `aliases` to ZSH or BASH config `(.zshrc or bashrc)` on the bottom.

``` bash
source $HOME/.config/aliases
source $HOME/.config/functions
```

## Note:

> Change your environment variables config on `.env`

example:

``` bash
NGINX_VHOST_LOCATION=$HOME'/.config/vhosts'
PROJECT_LOCATION=$HOME'/projects/www'
```

For change Nginx vhost TLD for local use on `functions` method `create_nginx_virtual_host`:

Depends on the last domain name you will use, for example local, test and others  from environment key `TLD_DOMAIN`

it can change server name and append to hosts file

``` bash
server_name $2.test;
```

If any issue please contact me @asapdotid :point_left:
