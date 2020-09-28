# Changelog

All notable changes to this project will be documented in this file.

The format is based on
[Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to
[Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [2.0.0](https://www.github.com/terraform-google-modules/terraform-google-cloud-storage/compare/v1.7.1...v2.0.0) (2020-09-28)


### ⚠ BREAKING CHANGES

* The resource state locations have changed to use for_each, please see the upgrade guide for details.

### Features

* Use for_each instead of count to create resource ([#86](https://www.github.com/terraform-google-modules/terraform-google-cloud-storage/issues/86)) ([af73533](https://www.github.com/terraform-google-modules/terraform-google-cloud-storage/commit/af735332c091c6fe5de082562c8d59f979421611))


### Bug Fixes

* Fix deprecation of is_live lifecycle rule ([#91](https://www.github.com/terraform-google-modules/terraform-google-cloud-storage/issues/91)) ([f73041b](https://www.github.com/terraform-google-modules/terraform-google-cloud-storage/commit/f73041b904d8f5c7020efb84737d54869e394738))

### [1.7.1](https://www.github.com/terraform-google-modules/terraform-google-cloud-storage/compare/v1.7.0...v1.7.1) (2020-09-21)


### Bug Fixes

* Constrain minimum Google provider version to 3.38 ([#84](https://www.github.com/terraform-google-modules/terraform-google-cloud-storage/issues/84)) ([ebc1916](https://www.github.com/terraform-google-modules/terraform-google-cloud-storage/commit/ebc19161e2b9c24ef41c2c5898b2d65eae81ee1e))

## [1.7.0](https://www.github.com/terraform-google-modules/terraform-google-cloud-storage/compare/v1.6.0...v1.7.0) (2020-09-16)

### ⚠ BREAKING CHANGES

* Minimum Google provider version increased to [3.38.0](https://github.com/hashicorp/terraform-provider-google/blob/master/CHANGELOG.md#3380-september-08-2020)


### Features

* Add is_live field to simple_bucket lifecycle ([#76](https://www.github.com/terraform-google-modules/terraform-google-cloud-storage/issues/76)) ([a16305d](https://www.github.com/terraform-google-modules/terraform-google-cloud-storage/commit/a16305dfad12ef06881a73a6c2a33fe7fe569bfb))


### Bug Fixes

* Use uniform_bucket_level_access flag instead due to deprecation ([#80](https://www.github.com/terraform-google-modules/terraform-google-cloud-storage/issues/80)) ([f287581](https://www.github.com/terraform-google-modules/terraform-google-cloud-storage/commit/f287581701bdcb0af996a26a8b922788cf686f57))



## [1.6.0](https://www.github.com/terraform-google-modules/terraform-google-cloud-storage/compare/v1.5.0...v1.6.0) (2020-05-26)


### Features

* Add support for cors and website config in variables ([#63](https://www.github.com/terraform-google-modules/terraform-google-cloud-storage/issues/63)) ([69dafb3](https://www.github.com/terraform-google-modules/terraform-google-cloud-storage/commit/69dafb3b3c532013919f4da416fa72aa009621a3))
* Add support for creating folders in buckets with folders variable ([#59](https://www.github.com/terraform-google-modules/terraform-google-cloud-storage/issues/59)) ([0fa0689](https://www.github.com/terraform-google-modules/terraform-google-cloud-storage/commit/0fa068980e4d01b66f5f0f2d923f6fae730b1151))


### Bug Fixes

* convert lifecycle action object to map ([#52](https://www.github.com/terraform-google-modules/terraform-google-cloud-storage/issues/52)) ([f2e6ea3](https://www.github.com/terraform-google-modules/terraform-google-cloud-storage/commit/f2e6ea3e1954c8311ff326d7c512756db1dd5ae9))

## [1.5.0](https://www.github.com/terraform-google-modules/terraform-google-cloud-storage/compare/v1.4.0...v1.5.0) (2020-04-22)


### Features

* add support for lifecycle rules in simple bucket ([#49](https://www.github.com/terraform-google-modules/terraform-google-cloud-storage/issues/49)) ([b39e2cd](https://www.github.com/terraform-google-modules/terraform-google-cloud-storage/commit/b39e2cdf0848b59d00dd7fe65c917a5bf4a1176a))

## [1.4.0](https://www.github.com/terraform-google-modules/terraform-google-cloud-storage/compare/v1.3.0...v1.4.0) (2020-03-04)


### Features

* add outputs for simple bucket module ([#38](https://www.github.com/terraform-google-modules/terraform-google-cloud-storage/issues/38)) ([f93bf5d](https://www.github.com/terraform-google-modules/terraform-google-cloud-storage/commit/f93bf5d88842018f8421be61af5a0f4afd947487))


### Bug Fixes

* Adding type constraints to variables ([#43](https://www.github.com/terraform-google-modules/terraform-google-cloud-storage/issues/43)) ([45d42a1](https://www.github.com/terraform-google-modules/terraform-google-cloud-storage/commit/45d42a1d7f73f8c4ad77d1455de77ce88ab0e8ad))

## [1.3.0](https://www.github.com/terraform-google-modules/terraform-google-cloud-storage/compare/v1.2.0...v1.3.0) (2020-02-13)


### Features

* Add simple bucket submodule ([#35](https://www.github.com/terraform-google-modules/terraform-google-cloud-storage/issues/35)) ([e75114a](https://www.github.com/terraform-google-modules/terraform-google-cloud-storage/commit/e75114a5770d8aab65764d4c04a36c52bde4f073))
* Add support for customer encryption keys ([#34](https://www.github.com/terraform-google-modules/terraform-google-cloud-storage/issues/34)) ([32eff9b](https://www.github.com/terraform-google-modules/terraform-google-cloud-storage/commit/32eff9b9330e6c9bb683cfd75d0baf9d9798b7eb))
* replace dot on a dash in label value ([#31](https://www.github.com/terraform-google-modules/terraform-google-cloud-storage/issues/31)) ([8875ebb](https://www.github.com/terraform-google-modules/terraform-google-cloud-storage/commit/8875ebbc645e1a6196c61a9f4d0cfaf3fa0f6569))

## [Unreleased]

## [1.2.0] - 2019-12-06

### Added

- Added support for setting lifecycle rules [#19](https://github.com/terraform-google-modules/terraform-google-cloud-storage/pull/19)

## [1.1.0] - 2019-11-20

### Added

- Include name of bucket as label for cost analysis [#20]

### Fixed

- Error from the `names` and `urls` outputs caused by removing elements from the `names` variable. [#23]

## [1.0.0] - 2019-08-14

### Changed

- Upgraded for usage with terraform-0.12.x [#9]
- Added support for `force_destroy` attribute [#9]

## [0.1.0] - 2019-05-22

### Added

- Initial release

[Unreleased]: https://github.com/terraform-google-modules/terraform-google-cloud-storage/compare/v1.2.0...HEAD
[1.2.0]: https://github.com/terraform-google-modules/terraform-google-cloud-storage/compare/v1.1.0...v1.2.0
[1.1.0]: https://github.com/terraform-google-modules/terraform-google-cloud-storage/compare/v1.0.0...v1.1.0
[1.0.0]: https://github.com/terraform-google-modules/terraform-google-cloud-storage/compare/v0.1.0...v1.0.0
[0.1.0]: https://github.com/terraform-google-modules/terraform-google-cloud-storage/releases/tag/v0.1.0

[#23]: https://github.com/terraform-google-modules/terraform-google-cloud-storage/pull/23
[#20]: https://github.com/terraform-google-modules/terraform-google-cloud-storage/pull/20
[#9]: https://github.com/terraform-google-modules/terraform-google-cloud-storage/pull/9
