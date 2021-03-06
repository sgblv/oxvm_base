# Changelog

All notable changes to this project will be documented in this file.
The format is based on [Keep a Changelog](http://keepachangelog.com/)
and this project adheres to [Semantic Versioning](http://semver.org/).

## [Unreleased] 

### Added
- Add PHP extension sqlite3 to installation defaults
- Introduce MySQL version setting and set '5.7' as default

### Changed
- Use Firefox version 31.6.0 ESR instead of 31.0

### Fixed

- Elasticsearch installation [PR-25](https://github.com/OXID-eSales/oxvm_base/pull/25)

## [2.1.2] - 2018-12-07

### Changed
- Remove exact version number from hirak/prestissimo requirement
- Replace with_items syntax for apt tasks with new packages syntax
- Always use the present state for apt installation roles except for system packages
- Add ca-certificates to system packages
- Introduce timeout of 60 seconds for get_url tasks (overwriting default of 10 seconds)
- Add 5 retries to get_url tasks

## [2.1.1] - 2018-11-12

### Added
- Config option for gitlab tokens [PR-23] (https://github.com/OXID-eSales/oxvm_base/pull/23)
- Config option for http authentication [PR-23] (https://github.com/OXID-eSales/oxvm_base/pull/23)

### Changed
- Limit the doxygen uninstall action to just uninstall doxygen

## [2.1.0] - 2018-09-13

### Added
- Doxygen role

### Changed
- Increased composer timeout to 15 minutes by default
- Install git by default

## [2.0.1] - 2018-09-07

### Changed
- Update Vagrantfile for changes in plugin loading [PR-22](https://github.com/OXID-eSales/oxvm_base/pull/22)

## [2.0.0] - 2018-07-18

### Changed
- PHP installation process improved [PR-21](https://github.com/OXID-eSales/oxvm_base/pull/21)
- PHP 7.1 is installed by default.

### Removed
- phpbrew and phpswitch functionality was removed, as it was giving unstable results. 

## [1.1.3] - 2018-07-12

### Changed
- Change permissions of `/vagrant` share only for Windows ([ansible issue](https://github.com/ansible/ansible/issues/42388))

## [1.1.2] - 2018-07-11

### Changed
- Set permissions for shared directory since Ansible's behaviour changed in 2.6.1

## [1.1.1] - 2018-05-15

### Changed
- Remove triggers plugin requirement if Vagrant version is >= 2.1.0

## [1.1.0] - 2017-11-22

### Added
- Selenium role
- Landing page with installation role

### Changed
- Switched packages source to german sources by default
- README now contains configuration information
- Varnish setup information

[Unreleased]: https://github.com/OXID-eSales/oxvm_base/compare/v2.1.2...master
[2.1.2]: https://github.com/OXID-eSales/oxvm_base/compare/v2.1.1...v2.1.2
[2.1.1]: https://github.com/OXID-eSales/oxvm_base/compare/v2.1.0...v2.1.1
[2.1.0]: https://github.com/OXID-eSales/oxvm_base/compare/v2.0.1...v2.1.0
[2.0.1]: https://github.com/OXID-eSales/oxvm_base/compare/v2.0.0...v2.0.1
[2.0.0]: https://github.com/OXID-eSales/oxvm_base/compare/v1.1.3...v2.0.0
[1.1.3]: https://github.com/OXID-eSales/oxvm_base/compare/v1.1.2...v1.1.3
[1.1.2]: https://github.com/OXID-eSales/oxvm_base/compare/v1.1.1...v1.1.2
[1.1.1]: https://github.com/OXID-eSales/oxvm_base/compare/v1.1.0...v1.1.1
[1.1.0]: https://github.com/OXID-eSales/oxvm_base/compare/v1.0.0...v1.1.0
