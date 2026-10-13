# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [4.0.0] - 2026-11-01

### Added
- Updated API symbol definitions for OpenTTD GameScript API version 15 and JGR's Patchpack `jgrpp-0.73.4`.

### Changed
- Bumped internal script version to 4 (`SELF_VERSION 4`).
- Updated OpenTTD GameScript API compatibility version target in `info.nut` from 1.3 to 15.
- Updated SuperLib dependency import from version 36 to version 41 in `main.nut`.
- Updated API binding generator script `gen_api_binding.py` to scan `*.sq.hpp` headers for `jgrpp-0.73.4`.
- Updated release archive packager script `make_tar.py` to bundle `README.md`.

### Fixed
- Fixed Squirrel argument type check for booleans in `admin_port.nut` (`typeof(arg) == "bool"` instead of `"boolean"`).
