# chywalry

> Here comes the chywalry.

Chywalry's here to help you connect your apps together. You define a list of events, and make sure your client apps calls and listen to them.

It also provides an image writer utility via the `write-img` event.

## Installation

## Prerequisites

Chywalry uses:

* [socket.io](http://socket.io) to broadcast events

* [imagemagick-native](https://github.com/elad/node-imagemagick-native) to manipulate image before writing them to disk

* [mdns](https://github.com/agnat/node_mdns) to allow your app to connect seamlessly

It's compatible with node >= `v0.8.x`.

### Linux

```
$ sudo apt-get install avahi-daemon avahi-discover libnss-mdns libavahi-compat-libdnssd-dev curl build-essential
$ sudo apt-get install imagemagick libmagick++-dev
```

### OSX

```
$ brew install imagemagick
```

## Install dependencies

```
$ npm i
```

## Configure

```
$ cp config.example.json config.json
```

And fill it with your own settings.

## Usage

```
$ npm start
```

## Develop

You can test writing images with the [`dev/send-img.js`](/dev/send-img.js) script. Run `$ npm run send-img`.

You can test sending events with the [`dev/send-events.js`](/dev/send-events.js) script. Run `$ npm run send-events`.

Please follow [standard style](https://github.com/feross/standard) conventions.
