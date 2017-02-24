# LiveSASS fails to start when using Zurb Foundation 5.5.3 SASS 

This project reproduces the bug reported in [Chromium DevTools LiveSASS #695056](https://bugs.chromium.org/p/chromium/issues/detail?id=695056).
Template based on [Foundation libsass template](http://foundation.zurb.com/sites/docs/v/5.5.3/sass.html#cli).

## Requirements

You'll need to have the following items installed before continuing.

  * [Node.js](http://nodejs.org): Use the installer provided on the NodeJS website.
  * [Grunt](http://gruntjs.com/): Run `[sudo] npm install -g grunt-cli`
  * [Bower](http://bower.io): Run `[sudo] npm install -g bower`

## Quickstart

```bash
npm install
```
```bash
bower install
```
```
grunt
```

## How to reproduce the bug
1. Setup LiveSASS in DevTools
2. Open DevTools console and note the error message below


```
LiveSASS failed to start: http://localhost/livesass-bug/css/app.css.map
SourceMap is misaligned: right != #{$opposite-direction}
compiled: http://localhost/livesass-bug/css/app.css:1:16193
source: http://localhost/livesass-bug/bower_components/foundation/scss/foundation/components/_alert-boxes.scss:86:3
``
