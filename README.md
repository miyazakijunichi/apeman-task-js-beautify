apeman-task-js-beautify
==========

<!---
This file is generated by ape-tmpl. Do not update manually.
--->

<!-- Badge Start -->
<a name="badges"></a>

[![Build Status][bd_travis_shield_url]][bd_travis_url]
[![Code Climate][bd_codeclimate_shield_url]][bd_codeclimate_url]
[![Code Coverage][bd_codeclimate_coverage_shield_url]][bd_codeclimate_url]
[![npm Version][bd_npm_shield_url]][bd_npm_url]

[bd_repo_url]: https://github.com/miyazakijunichi/apeman-task-js-beautify
[bd_travis_url]: http://travis-ci.org/miyazakijunichi/apeman-task-js-beautify
[bd_travis_shield_url]: http://img.shields.io/travis/miyazakijunichi/apeman-task-js-beautify.svg?style=flat
[bd_license_url]: https://github.com/miyazakijunichi/apeman-task-js-beautify/blob/master/LICENSE
[bd_codeclimate_url]: http://codeclimate.com/github/miyazakijunichi/apeman-task-js-beautify
[bd_codeclimate_shield_url]: http://img.shields.io/codeclimate/github/miyazakijunichi/apeman-task-js-beautify.svg?style=flat
[bd_codeclimate_coverage_shield_url]: http://img.shields.io/codeclimate/coverage/github/miyazakijunichi/apeman-task-js-beautify.svg?style=flat
[bd_gemnasium_url]: https://gemnasium.com/miyazakijunichi/apeman-task-js-beautify
[bd_gemnasium_shield_url]: https://gemnasium.com/miyazakijunichi/apeman-task-js-beautify.svg
[bd_npm_url]: http://www.npmjs.org/package/apeman-task-js-beautify
[bd_npm_shield_url]: http://img.shields.io/npm/v/apeman-task-js-beautify.svg?style=flat
[bd_bower_badge_url]: https://img.shields.io/bower/v/apeman-task-js-beautify.svg?style=flat

<!-- Badge End -->


<!-- Description Start -->
<a name="description"></a>

Beautify code written in javascript.

<!-- Description End -->


<!-- Overview Start -->
<a name="overview"></a>



<!-- Overview End -->


<!-- Sections Start -->
<a name="sections"></a>

<!-- Section from "doc/readme/01.Installation.md.hbs" Start -->

<a name="section-doc-readme-01-installation-md"></a>
Installation
-----

```bash
$ npm install apeman-task-js-beautify --save-dev
```


<!-- Section from "doc/readme/01.Installation.md.hbs" End -->

<!-- Section from "doc/readme/02.Usage.md.hbs" Start -->

<a name="section-doc-readme-02-usage-md"></a>
Usage
---------

1. Define a task within Apemanfile.js
2. Call the task via apeman task command.

**Apemanfile.js**
```javascript
/** This example Apemanfile to use apeman-task-js-beautify */

"use strict";

module.exports = {
    $pkg: {/*...*/},
    $tasks: {
        // Define your own task.
        'my-task-01': require('apeman-task-js-beautify')('some/pattern/**/*.js', {
            //Options
            beautifyOptions: {
                'indent_size': 4
            }
        })
    }
};

```

Then,
```bash
$ apeman task my-task-01
```


<!-- Section from "doc/readme/02.Usage.md.hbs" End -->

<!-- Section from "doc/readme/03.Options.md.hbs" Start -->

<a name="section-doc-readme-03-options-md"></a>
Options
-------

| Key | Type | Default | Description |
| --- | ---- | --- | --- |
|ignoreError|bool|false|ignore error|
|ignore|string[]&#124;string|[]|file patterns to ignore|
|beautifyOptions|object|{}|options for [js-beautify](https://github.com/beautify-web/js-beautify)|


<!-- Section from "doc/readme/03.Options.md.hbs" End -->


<!-- Sections Start -->


<!-- LICENSE Start -->
<a name="license"></a>

License
-------
This software is released under the [MIT License](https://github.com/miyazakijunichi/apeman-task-js-beautify/blob/master/LICENSE).

<!-- LICENSE End -->


<!-- Links Start -->
<a name="links"></a>

Links
------

+ [apeman](https://github.com/apeman-labo/apeman)
+ [apeman-task](https://github.com/apeman-labo/apeman-task)

<!-- Links End -->
