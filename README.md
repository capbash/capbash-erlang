capbash-erlang
==============

Scripts for installing [erlang](http://www.erlang.org/) a functional language for
building massively scalable soft real-time systems.  These scripts are best used in
conjunction with capbash

# How to Install #

Install capbash first, more details at:
https://github.com/capbash/capbash

```
curl -s https://raw.githubusercontent.com/capbash/capbash/master/capbash-installer | bash
capbash new YOUR_REPO_ROOT
cd YOUR_REPO_ROOT
```

Now you can install erlang into your project

```
capbash install erlang
```

# Configurations #

The available configurations include:

```
ERLANG_VERSION=${ERLANG_VERSION-17.5-1}
ERLANG_LAUNCHER_DIR=${ERLANG_LAUNCHER_DIR-/var/local/erlang/$ERLANG_VERSION}
```

# Deploy to Remote Server #

To push the erlang script to your server, all you need if the IP or hostname
of your server (e.g. 192.167.0.48) and your root password.

```
capbash deploy <IP> erlang
```

For example,

```
capbash deploy 127.0.0.1 erlang
```
