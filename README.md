# Coding standard

Tuned & very strict coding standards for PHP projects

-----

[![Downloads total](https://img.shields.io/packagist/dt/fiolasoft/coding-standard.svg?style=flat-square)](https://packagist.org/packages/fiolasoft/coding-standard)
[![Latest stable](https://img.shields.io/packagist/v/fiolasoft/coding-standard.svg?style=flat-square)](https://packagist.org/packages/fiolasoft/coding-standard)

## Install

```bash
composer require --dev fiolasoft/coding-standard
```

## Strictness

| File          | Strictness |
|---------------|------------|
| ruleset       | strict     |
| ruleset-nette | 90%        |

## Usage

Create `ruleset.xml` in root of your project.

```
<?xml version="1.0"?>
<ruleset name="YourProject">
    <!-- Extending rulesets -->
    <rule ref="vendor/fiolasoft/coding-standard/ruleset.xml"/>
    <!-- Ninjify [Nette] -->
    <!-- <rule ref="vendor/fiolasoft/coding-standard/ruleset-nette.xml"/> -->

    <!-- My rules -->
    
    <!-- Exclude folders -->
    <exclude-pattern>/tests/tmp</exclude-pattern>
</ruleset>
```