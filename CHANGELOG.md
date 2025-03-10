# Changelog

## [Unreleased] - TBA
### Fixed
- Fix `FileContentProvider` to throw an exception when the file does not exist
- Add `try/catch` to `FileSymbolProvider` to continue working instead of crashing if a file could not be parsed
- Hotfix issue when attempting to parse an invalid php file, this will be caught silently and the file will not be parsed (will get reported in the future)
### Added
### Changed
### Removed

## [0.1.5] - 2022-02-03
### Fixed
### Added
### Changed
- Allow `composer-unused/contracts` in version `0.2`
### Removed

## [0.1.4] - 2022-01-05
### Added
- Added `FunctionInvocationStrategy` to find consumed symbols by function invocation
- Added possibility to parse symbols from `define()`
- Added `ConstStrategy` to parse consumed constants
- Added support for `symfony/finder` up until version `^6.0`
- Added symlink support for `autoload.files`
- Added dependency to `composer-unused/contracts`
### Changed
### Removed
- Dropped support for php `7.3`

## [0.1.3] - 2021-08-02
### Fixed
- Fix issue with parsed include expression where there could be concat operations
  resulting in wrong path usages for included files to parse

## [0.1.2] - 2021-08-01
### Added
- Added missing `symfony/finder` dependency

## [0.1.1] - 2021-08-01
### Fixed
- Fixed issue with `require` or `include` statements

## [0.1.0] - 2021-02-12
Initial release
