# README

HTTP/HTTPS caching proxy for work with npm utility

## Installation

```sh
# Define installation folder

export INSTALL_DIRECTORY=/usr/bin

# Use local installation

sudo bin/installer install

# Use remote installation

curl --location "https://github.com/timonier/npm-proxy-cache/raw/master/bin/installer" | sudo sh -s -- install
```

__Note__: If you do not define `INSTALL_DIRECTORY`, `installer` will use in `/usr/local/bin`.

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

## Contributing

1. Fork it.
2. Create your branch: `git checkout -b my-new-feature`.
3. Commit your changes: `git commit -am 'Add some feature'`.
4. Push to the branch: `git push origin my-new-feature`.
5. Submit a pull request.

__Note__: Use the script `bin/build` to test your modifications locally.

If you like / use this project, please let me known by adding a [★](https://help.github.com/articles/about-stars/) on the [GitHub repository](https://github.com/timonier/npm-proxy-cache).

## Links

* [image "timonier/npm-proxy-cache"](https://hub.docker.com/r/timonier/npm-proxy-cache/)
* [runk/npm-proxy-cache](https://github.com/runk/npm-proxy-cache)
* [timonier/dumb-entrypoint](https://github.com/timonier/dumb-entrypoint)
* [timonier/version-lister](https://github.com/timonier/version-lister)
