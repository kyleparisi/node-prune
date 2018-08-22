<img src="http://tjholowaychuk.com:6000/svg/title/NODE/PRUNE">

## What?

node-prune is a small tool to prune unnecessary files from ./node_modules, such as markdown, typescript source files, and so on. Primarily built for [Up](https://github.com/apex/up) which lets you deploy serverless web applications in seconds.

## Installation

```
$ go get github.com/kyleparisi/vendor-prune/cmd/vendor-prune
```

## Usage

In your app directory:

```
$ vendor-prune

files total 27,330
files removed 3,990
size removed 13 MB
   duration 200ms
```

Somewhere else:

```
$ vendor-prune path/to/vendor

files total 27,330
files removed 3,990
size removed 13 MB
   duration 200ms
```

Or add to the ``package.json`` scripts field

```
  "scripts": {
    "postinstall": "vendor-prune"
  }
```

## Why?

![huge](https://pbs.twimg.com/media/DEIV_1XWsAAlY29.jpg)

---

[![GoDoc](https://godoc.org/github.com/tj/node-prune?status.svg)](https://godoc.org/github.com/tj/node-prune)
![](https://img.shields.io/badge/license-MIT-blue.svg)
![](https://img.shields.io/badge/status-stable-green.svg)

<a href="https://apex.sh"><img src="http://tjholowaychuk.com:6000/svg/sponsor"></a>
