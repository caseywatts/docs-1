---
title: "JavaScript"
slug: "getting-started-with-javascript"
category: "languages"
ordinal: 1000
---

**Windows and OS X users**: Install [Node.js](http://nodejs.org/) [via package manager](https://github.com/joyent/node/wiki/Installing-Node.js-via-package-manager).

**Linux users**: [Joyent maintains a document][linstall] that details how to get Node.js installed for a wide range of distributions and package managers.

[linstall]: https://github.com/joyent/node/wiki/Installing-Node.js-via-package-manager

Install `jasmine-node`:

```bash
$ npm install jasmine-node -g
```

Depending on your setup, you may need super user privileges to install an NPM module globally. This is the case if you've used the official installer linked to above. If NPM gives you an error saying you don't have access, add `sudo` to the command above:

```bash
$ sudo npm install jasmine-node -g
````

If you've used the official installer, your `PATH` should have been automatically configured, but if your shell has trouble locating your globally installed modules—or if you build Node.js from source—update your `PATH` to include the `npm` binaries by adding the following to either `~/.bash_profile` or `~/.zshrc`:

```bash
$ export PATH=/usr/local/share/npm/bin:$PATH
```

## Running Tests

Execute the tests with:

```bash
$ jasmine-node bob_test.spec.js
```

## Making Your First Node Module

To create a module that can be loaded with `var Bob = require('./bob');`, put this code in `bob.js`:

```javascript
var Bob = function() {};
module.exports = Bob;
```

You can find more information about modules in the [node documentation](http://nodejs.org/api/modules.html#modules_module_exports).

## Recommended Learning Resources

Exercism provides exercises and feedback but can be difficult to jump into for those learning JavaScript for the first time. These resources can help you get started:

* [Mozilla JavaScript Guide](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide)
* [Mozilla JavaScript Reference](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference)
* [Mozilla Recommended Resources](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
* [StackOverflow](http://stackoverflow.com/)
