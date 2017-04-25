# README

HTTP/HTTPS caching proxy for work with npm utility

## Installation

Copy `bin/npm-proxy-cache` into your executable folder (like `/usr/local/bin` or `$HOME/bin`):

```sh
sudo curl --location --output /usr/local/bin/npm-proxy-cache "https://github.com/timonier/npm-proxy-cache/raw/master/bin/npm-proxy-cache"
sudo chmod +x /usr/local/bin/npm-proxy-cache
```

Linux users can use the [installer](https://github.com/timonier/npm-proxy-cache/blob/master/bin/installer):

```sh
curl --location "https://github.com/timonier/npm-proxy-cache/raw/master/bin/installer" | sudo sh -s install
```

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

## Links

* [command "docker run"](https://docs.docker.com/reference/run/)
* [image "timonier/npm-proxy-cache"](https://hub.docker.com/r/timonier/npm-proxy-cache/)
* [runk/npm-proxy-cache](https://github.com/runk/npm-proxy-cache)
* [timonier/dumb-entrypoint](https://github.com/timonier/dumb-entrypoint)
* [timonier/version-lister](https://github.com/timonier/version-lister)
