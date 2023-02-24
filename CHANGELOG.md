# Change Log

All notable changes to the "pulpscript-syntax" extension will be documented in this file.

Check [Keep a Changelog](http://keepachangelog.com/) for recommendations on how to structure this file.

## [Unreleased]

## [0.3.3] - 2023-02-23

### Added

- Added support for `.txt` filename extensions

## [0.2.3] - 2023-02-10

### Added

- Added missing `>` and `<` to `comparisons`

## [0.2.2] - 2023-02-10

### Added

- Added missing `!=` to `controls`

## [0.2.1] - 2023-02-09

### Added

- Added `in` to `controls`

### Updated

- Moved `to` from `functions` to `controls`

## [0.2.0] - 2023-02-07

### Added

- Added supported pattern `coords`

### Changed

- Updated `comparisons` to support all possible variations (integers, floats, variables, strings, with & without spaces)
- Updated `numeric` to be `floats`

### Removed

- Removed extra `patterns` that aren't necessary

## [0.1.1] - 2023-02-07

### Changed

- Updated `comparisons` to support strings

## [0.1.0] - 2023-02-06

### Added

- Added supported pattern `datetime` and its read-only properties
- Added preview image to README

### Changed

- Updated order of `repository` objects to match `patterns`
- Updated location of objects used once to be nested
  - `string-interpolation` under `strings`
  - `config-properties` under `config`
  - `event-properties` under `event`
- Added word boundaries to `built-in-events`
- Updated `numeric` to allow numbers in variable names

### Removed

- `do`/`end` and `then`/`end` from `autoClosingPairs`

## [0.0.1] - 2023-02-02

### Added

- Initial release
- Supported patterns
  - comments
  - strings
  - decrement
  - increment
  - numeric
  - comparisons
  - augmented assignments
  - spaces
  - assignment
  - functions
  - built-in events
  - controls
  - colons
  - commas
  - config
  - event
  - variables
