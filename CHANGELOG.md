# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [0.2.3] - 2021-09-16

Thanks to [Matthis Holleville](https://github.com/matthisholleville) ([PR #17](https://github.com/betr-io/terraform-provider-mssql/pull/17)), and [bruno-motacardoso](https://github.com/bruno-motacardoso) ([PR #14](https://github.com/betr-io/terraform-provider-mssql/pull/14)).

### Changed

- Add string split function, which should allow the provider to work on SQL Server 2014 (#17).
- Improved documentation (#14).

## [0.2.2] - 2021-08-24

### Changed

- Upgraded to go version 1.17.
- Upgraded dependencies.
- Upgraded dependencies in test fixtures.

## [0.2.1] - 2021-04-30

Thanks to [Anders Båtstrand](https://github.com/anderius) ([PR #8](https://github.com/betr-io/terraform-provider-mssql/pull/8), [PR #9](https://github.com/betr-io/terraform-provider-mssql/pull/9))

### Changed

- Upgrade go-mssqldb to support go version 1.16.

### Fixed

- Cannot create user because of conflicting collation. ([#6](https://github.com/betr-io/terraform-provider-mssql/issues/6))

## [0.2.0] - 2021-04-06

When it is not possible to give AD role: _Directory Readers_ to the Sql Server Identity or an AD Group, use *object_id* to add external user.

Thanks to [Brice Messeca](https://github.com/smag-bmesseca) ([PR #1](https://github.com/betr-io/terraform-provider-mssql/pull/1))

### Added

- Optional object_id attribute to mssql_user

## [0.1.1] - 2020-11-17

Update documentation and examples.

## [0.1.0] - 2020-11-17

Initial release.

### Added

- Resource `mssql_login` to manipulate logins to a SQL Server.
- Resource `mssql_user` to manipulate users in a SQL Server database.

[Unreleased]: https://github.com/betr-io/terraform-provider-mssql/compare/v0.2.3...HEAD
[0.2.3]: https://github.com/betr-io/terraform-provider-mssql/compare/v0.2.2...v0.2.3
[0.2.2]: https://github.com/betr-io/terraform-provider-mssql/compare/v0.2.1...v0.2.2
[0.2.1]: https://github.com/betr-io/terraform-provider-mssql/compare/v0.2.0...v0.2.1
[0.2.0]: https://github.com/betr-io/terraform-provider-mssql/compare/v0.1.1...v0.2.0
[0.1.1]: https://github.com/betr-io/terraform-provider-mssql/compare/v0.1.0...v0.1.1
[0.1.0]: https://github.com/betr-io/terraform-provider-mssql/releases/tag/v0.1.0
