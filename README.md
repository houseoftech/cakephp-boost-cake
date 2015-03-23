# BoostCake

BoostCake is a plugin for CakePHP using Bootstrap

For original version see http://slywalker.github.io/cakephp-plugin-boost_cake/

This version makes some changes to the paginator helper and setting default options when using Form::create(). The differences should not cause any incompatibilities in your project. See a [comparison](https://github.com/slywalker/cakephp-plugin-boost_cake/compare/master...houseoftech:master) for more details.

* [Bootstrap(2.3.2)](http://getbootstrap.com/2.3.2/)
* [Bootstrap(3.0.0)](http://getbootstrap.com/)

## Requirements

* CakePHP >= 2.3
* Bootstrap >= 2.3 (3.0 support)

## Installation

Ensure require is present in composer.json. This will install the plugin into Plugin/BoostCake:

	{
		"require": {
			"houseoftech/cakephp-boost-cake": "*"
		},
		"repositories": [
			{
				"type": "vcs",
				"url": "https://github.com/houseoftech/cakephp-boost-cake"
			}
		]
	}

### Enable plugin

You need to enable the plugin in your app/Config/bootstrap.php file:

`CakePlugin::load('BoostCake', array('bootstrap' => true));`

If you are already using `CakePlugin::loadAll();`, then this is not necessary.

## Documentation

[BoostCake - Bootstrap Plugin for CakePHP](http://slywalker.github.io/cakephp-plugin-boost_cake/)

## Development Policy

More Simple! Simple! Simple!

* Develop only those that method's $options in FormHelper unable to solve.
* Don't develop ajax/js helper

If you want to simplify the options, you can develop WrapBoostCake plugin.

### What this plugin solves

* Replaces the `label` of checkboxes and radios
* Adds a wrapping `div` to inputs
* Adds content before and after `input`
* Adds error class in outer `div`
* Changes pagination tags
* Changes SessionHelper::flash()'s template

## License

The MIT License (MIT)

Copyright (c) 2014 Yasuo Harada

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
