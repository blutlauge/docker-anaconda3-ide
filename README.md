# Docker container including a python IDE based on ANACONDA3

This IDE is intended for use on a NAS system. It provides

- ANACONDA3.
- vim with appropriate plugins. 
- Zsh with the oh-my-zsh framwork.
- tmux.
- An SSH server and a MOSH server to be able to use this container from an iPad using the Blink shell.
- My dotfiles which ca be found at [GitHub](https://github.com/marcschlienger/dotfiles.git).
- And other mandatory stuff.

## Run
docker run -d -p 22:22 -p 60001:60001/udp --name \<container name\> -v \<source\>:\<target\> marcps/docker-anaconda3-ide:latest

## Connect

 - Using mosh: mosh <dev@server>; Password: screencast
 - Using ssh: ssh <dev@server>; Password: screencast
