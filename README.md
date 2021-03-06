# tern-tabris

[![Build Status](https://secure.travis-ci.org/angelozerr/tern-tabris.png)](http://travis-ci.org/angelozerr/tern-tabris)

[tern-tabris](https://github.com/angelozerr/tern-tabris) is a plugin which adds support for [tabris](https://github.com/eclipsesource/tabris-js) to the JavaSript code intelligence system [Tern](http://ternjs.net/).

## Demo

You can play with [online demo](http://codemirror-java.opensagres.eu.cloudbees.net/codemirror-javascript/demo/tabris.html) which uses CodeMirror ((inside Web Browser).

You can see demo in this git ptoject with CodeMirror in  [demos/tabris.html](https://github.com/angelozerr/tern-tabris/blob/master/demos/tabris.html) :

Here a screenshot with completion with CodeMorror tabris completion :
 
![CodeMirror & TernTabris](https://github.com/angelozerr/tern-tabris/wiki/images/TernTabrisWithCodeMirror.png)

Here a screenshot with completion with Eclipse IDE tabris completion :

![Eclipse & TernTabris](https://github.com/angelozerr/tern-tabris/wiki/images/TernTabrisWithEclipse.png)

If you wish to use Eclipse as IDE, see Eclipse support for [tabris](https://github.com/angelozerr/tern.java/wiki/Tern-&-tabris-support).

## Installation

tern-tabris works with the NodeJS [Tern Server][tern-server], and within a browser.

The easiest way to install tern-tabris is to use a recent version of
[npm][npm]. In the directory where you installed the [tern package][tern-npm],
simply run

```
$ npm install tern-tabris
```

## Configuration

`tabris` support tabris.

### With Node.js

In order for Tern to load the tern-tabris plugin once it is installed, you must
include `tabris` in the `plugins` section of your [Tern configuration
file][tern-config].

Here is a minimal example `.tern-project` configuration file:

```json
{
  "plugins": {
    "tabris": {}
  }
}
```

### With WebBrowser (CodeMirror)

See [demos/tabris.html](https://github.com/angelozerr/tern-tabris/blob/master/demos/tabris.html)

## Structure

The basic structure of the project is given in the following way:

* `tabris.js` the tern plugin.
* `demos/` demos with tabris tern plugin which use CodeMirror.
* `test` test of the tern plugin.
