---
description: Changelog
---

# Changelog

## 5.0.1-beta

### Fixed

* No more infinite loops

### Changed

* Now you don't need IDs, or ending block tokens.

## 4.0.1

### Changed

* Squirrelly now precompiles by default
* Major syntax changes

## 6.0.1

### Changed

* Added `load`, fixed `__express`, added `renderFile`, added `caching`
* Custom delimeters \(these actually came out in 5.0.0\)

## 7.0.0

### Changed

* Fixed an issue with `$` signs in references
* Fixed an issue where a helper opening block or self-closing helper on the same line as a reference would cause an error
* If a newline directly follows a closing tag, such as `}}` , it will be removed. This makes minification a lot easier

