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

If any issue please contact me @asapdotid :point_left:
