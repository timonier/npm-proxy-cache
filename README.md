# README

## Installation

Pull the image `timonier/npm-proxy-cache`:

```sh
# Get the latest image (version 0.4.2)
docker pull timonier/npm-proxy-cache

# Or get a specific version

# Get the version 0.4.2
docker pull timonier/npm-proxy-cache:0.4.2
```

## Usage

Run the application via `docker run`. The [npm-proxy-cache options](https://github.com/runk/npm-proxy-cache#usage) can be passed as arguments:

```sh
docker run \
    -i \
    -t \
    --net host \
    timonier/npm-proxy-cache --version
# 0.4.2

docker run \
    -i \
    -t \
    --net host \
    timonier/npm-proxy-cache -p 8082 -v
# ->> /tmp/mitm.sock
# [2016-03-27 13:54:43.270] [INFO] proxy - Listening on localhost:8082 [8]
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

* [command "docker pull"](https://docs.docker.com/reference/commandline/pull/)
* [command "docker run"](https://docs.docker.com/reference/run/)
* [image "timonier/npm-proxy-cache"](https://hub.docker.com/r/timonier/npm-proxy-cache/)
* [npm-proxy-cache](https://github.com/runk/npm-proxy-cache)
* [npm-proxy-cache options](https://github.com/runk/npm-proxy-cache#usage)
