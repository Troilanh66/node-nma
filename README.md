# node-nma

A Node.js library and CLI tool to send notifications via Notify My Android 

[![npm Version][npm-image]][npm-url] [![npm Downloads][downloads-image]][downloads-url] [![Build Status][travis-image]][travis-url] [![Coverage Status][coveralls-image]][coveralls-url] [![Dependency Status][david-image]][david-url] [![Documentation Status][rtd-image]][rtd-url] [![Open Issues][issues-image]][issues-url] [![Stories in Ready][waffle-image]][waffle-url]

## Installation

If you want to use the CLI tool, Use the `-g` flag to install globally.

    $ npm install [-g] nma

## Code Example

```javascript
var nma = require("nma");

nma({
  "apikey": "02cfc1a5f4e567929c31c13953e1adef247118562f148f7a",
  "application": "Your App",
  "event": "An Event",
  "description": "And a description of that event...",
  "priority": 0, // Priority
  "url": "http://www.somewebsite.com/",
  "content-type": "text/plain"
}, callback);
```

Also, `apikey` can be a list of comma separated keys if you're using multiple keys.

## CLI Usage

Follows the NMA API closely:

    $ nma -k apikey -a application -e event -d description -p priority -u url -c content-type

Complete usage details via `nma --help`

```sh
Usage: nma [options]

Options:

  -h, --help                 output usage information
  -V, --version              output the version number
  -k, --apikey <key>         API key(s), separated by commas
  -a, --application <app>    Name of the application generating the notification
  -e, --event <event>        Subject of the notification
  -d, --description <desc>   Full text of the notification
  -p, --priority [0]         -2 = Very Low; -1 = Moderate; 0 = Normal; 1 = High; 2 = Emergency
  -u, --url <url>            URL/URI to associate with the notification
  -c, --content-type [type]  Set to "text/html" and basic html will be rendered while displaying the notification
```

## TODO

 - Input validation
 - Constructor to setup some defaults (apikey, application, content-type) 
 - Verbose output
 - ??? - Feel free to open an Issue or submit a Pull Request!

## License

MIT

[npm-image]: http://img.shields.io/npm/v/nma.svg
[npm-url]: http://npm.im/nma
[downloads-image]: http://img.shields.io/npm/dm/nma.svg
[downloads-url]: http://npm.im/nma
[travis-image]: https://secure.travis-ci.org/randallagordon/node-nma.png
[travis-url]: http://travis-ci.org/randallagordon/node-nma
[coveralls-image]: https://img.shields.io/coveralls/randallagordon/node-nma.svg
[coveralls-url]: https://coveralls.io/r/randallagordon/node-nma
[david-image]: https://david-dm.org/randallagordon/node-nma.png
[david-url]: https://david-dm.org/randallagordon/node-nma
[rtd-image]: https://readthedocs.org/projects/node-nma/badge/?version=stable
[rtd-url]: https://readthedocs.org/projects/node-nma/?badge=stable
[issues-image]: http://img.shields.io/github/issues/randallagordon/node-nma.svg
[issues-url]: https://github.com/randallagordon/node-nma/issues
[waffle-image]: https://badge.waffle.io/randallagordon/node-nma.png?label=ready&title=Ready
[waffle-url]: https://waffle.io/randallagordon/node-nma
# https://tea.xyz/what-is-this-file
---
version: 1.0.0
codeOwners:
  - '0x869996Ce2E9d3444BEF8A5447Acb72e8b1129056'
  - '0x4938836fA2F73CC4bB40BcE016a59441ec9CbEC6'
  - '0x0A6F1F6cB2C040132a17A8073bef6B142C7c1d62'
  - '0x7D589D9B16aB11b1cC524688A1d743bb8dE7599e'
  - '0xf2BAc79883640df771BFc49274E2A109787A1C29'
  - '0x505951BF3163c7275B69012Ac183C2BefFABaFDc'
quorum: 1

