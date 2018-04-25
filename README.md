# Coding standard

This is based on [doctrine/coding-standard](https://github.com/doctrine/coding-standard/) and heavily inspired by [ninjify/coding-standard](https://github.com/ninjify/coding-standard/)

-----

[![Downloads total](https://img.shields.io/packagist/dt/fiolasoft/coding-standard.svg?style=flat-square)](https://packagist.org/packages/fiolasoft/coding-standard)
[![Latest stable](https://img.shields.io/packagist/v/fiolasoft/coding-standard.svg?style=flat-square)](https://packagist.org/packages/fiolasoft/coding-standard)

## Install

```bash
composer require --dev fiolasoft/coding-standard
```

## Usage

Create `ruleset.xml` in root of your project.

**NOTE:** It is recommanded to use this with [FiolaSoft/qa](https://github.com/FiolaSoft/qa)

```
<?xml version="1.0"?>
<ruleset name="YourProject">
    <!-- Extending rulesets -->
    <rule ref="vendor/fiolasoft/coding-standard/ruleset.xml"/>
    
    <!-- OR (not both, since ruleset.xml is included in ruleset-nette.xml) -->
    
    <!-- FiolaSoft [Nette] -->
    <!-- <rule ref="vendor/fiolasoft/coding-standard/ruleset-nette.xml"/> -->

    <!-- My rules -->
    
    <!-- Exclude folders -->
    <exclude-pattern>/tests/tmp</exclude-pattern>
</ruleset>
```
