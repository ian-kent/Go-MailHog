MailHog [ ![Download](https://img.shields.io/github/release/mailhog/MailHog.svg) ](https://github.com/mailhog/MailHog/releases/tag/v0.1.0) [![GoDoc](https://godoc.org/github.com/mailhog/MailHog?status.svg)](https://godoc.org/github.com/mailhog/MailHog) [![Build Status](https://travis-ci.org/mailhog/MailHog.svg?branch=master)](https://travis-ci.org/mailhog/MailHog)
=========

Inspired by [MailCatcher](http://mailcatcher.me/), easier to install.

MailHog is a rewritten version of [MailHog](https://github.com/ian-kent/MailHog), which was born out of [M3MTA](https://github.com/ian-kent/M3MTA).

Go was chosen for portability - MailHog runs without installation on multiple platforms.

### Requirements

* None!

### Getting started

1. Either:
  * [Download the latest release](/docs/RELEASES.md) of MailHog for your platform
  * [Read the deployment guide](/docs/DEPLOY.md) for other deployment options
2. [Configure MailHog](/docs/CONFIG.md), or use the default settings:
  * the SMTP server will start on port 1025
  * the HTTP server will start on port 8025
  * in-memory message storage will be used.

### Features

* ESMTP server implementing RFC5321
* Support for SMTP AUTH (RFC4954) and PIPELINING (RFC2920)
* Web interface to view messages (plain text, HTML or source)
  * Supports RFC2047 encoded headers
* Real-time updates using EventSource
* Release messages to real SMTP servers
* Chaos Monkey for failure testing
  * See [Introduction to Jim](/docs/JIM.md) for more information
* HTTP API to list, retrieve and delete messages
  * See [APIv1 documentation](/docs/APIv1.md) for more information
* Multipart MIME support
* Download individual MIME parts
* In-memory message storage
* MongoDB storage for message persistence
* Lightweight and portable
* No installation required

![Screenshot of MailHog web interface](/docs/MailHog.png "MailHog web interface")

### Contributing

Clone this repository to ```$GOPATH/src/github.com/mailhog/MailHog``` and type ```make deps```.

See the [Building MailHog](BUILD.md) guide.

Requires Go 1.2+ to build.

Run tests using ```make test``` or ```goconvey```.

If you make any changes, run ```go fmt ./...``` before submitting a pull request.

### Licence

Copyright ©‎ 2014, Ian Kent (http://iankent.uk)

Released under MIT license, see [LICENSE](LICENSE.md) for details.


[![Bitdeli Badge](https://d2weczhvl823v0.cloudfront.net/mailhog/mailhog/trend.png)](https://bitdeli.com/free "Bitdeli Badge")

