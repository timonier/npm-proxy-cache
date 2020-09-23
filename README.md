# README

HTTP/HTTPS caching proxy for work with npm utility

⚠️ This project is no longer maintained. ⚠️

## Installation

```sh
# Define installation folder

export INSTALL_DIRECTORY=/usr/bin

# Use local installation

sudo bin/installer install

# Use remote installation

curl --location "https://gitlab.com/timonier/npm-proxy-cache/raw/master/bin/installer" | sudo sh -s -- install
```

__Note 1__: If you do not define `INSTALL_DIRECTORY`, `installer` will use in `/usr/local/bin`.

__Note 2__: `docker-for-mac` users have to configure [native NFS server](https://medium.com/@sean.handley/how-to-set-up-docker-for-mac-with-native-nfs-145151458adc).

## Usage

Run the command `npm-proxy-cache`:

```sh
# See all npm-proxy-cache options

npm-proxy-cache --help

# Run npm-proxy-cache

npm-proxy-cache --port 8082 --verbose
# [2017-04-15 11:53:28.383] [INFO] proxy - Listening on localhost:8082 [9]
# ...
```

## Links

* [image "timonier/npm-proxy-cache"](https://hub.docker.com/r/timonier/npm-proxy-cache/)
* [runk/npm-proxy-cache](https://github.com/runk/npm-proxy-cache)
* [set up docker for mac with native nfs](https://medium.com/@sean.handley/how-to-set-up-docker-for-mac-with-native-nfs-145151458adc)
