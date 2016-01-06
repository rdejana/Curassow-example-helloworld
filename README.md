# Hello World

This is a simple Swift Hello World website using the
[Curassow](https://github.com/kylef/Curassow) webserver which uses a pre-fork worker model.

## Usage

```shell
$ swift build --configuration release
$ ./.build/release/HelloWorld
Listening on 0.0.0.0:8000
```

### Deployment

This example can be deployed with my fork of the swift buidpack:
cf push <appName> -b  https://github.com/rdejana/swift-buildpack.git

### Options

```shell
$ ./.build/release/HelloWorld --help
Usage:

    $ ./.build/release/HelloWorld

Options:
    --bind
    --workers
```

```shell
$ ./.build/release/HelloWorld --bind 127.0.0.1:8080
```
