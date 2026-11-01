# Changelog

All notable changes to avocado-ext-jtop are documented in this file.
The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [0.1.1]

### Fixed
- Targets use the Jetson names both feeds now share, `jetson-orin-nano` and
  `jetson-agx-orin`, instead of the `-devkit` names only the 2024 feed had. The
  2026 release leg named `jetson-orin-nano-devkit`, which 2026 does not have, so
  it published to a repo no device resolves. meta-avocado scarthgap now uses
  the same names on 2024.
- `test.yml` gains the 2026 leg.

## [0.1.0]

### Added
- Initial release: Jetson system monitoring via jtop (jetson-stats).
- CI via the shared `avocado-linux/actions` reusable workflows: PR build check
  (`test.yml`) and tag-driven package + publish to the Avocado feed (`release.yml`).
