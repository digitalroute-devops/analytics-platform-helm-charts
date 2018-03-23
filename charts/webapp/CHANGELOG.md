# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).


## [1.3.7] - 2018-03-23
### Changed
- Use [auth-proxy `v0.1.2`](https://github.com/ministryofjustice/analytics-platform-auth-proxy/releases/tag/v0.1.2) which fixes
  a syntax error and adds a proper healthcheck endpoint
- Use `/healthz` endpoint added by above version of auth-proxy


## [1.2.0] - 2017-08-31
### Added
- webapps can assume an IAM role passed via `AWS.IAMRole` value, see README
- `CHANGELOG.md`


### Removed
- Unused AWS values: `AccessKeyId`, `SecretAccessKey` and `DefaultRegion`
