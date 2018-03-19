# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).


## [1.1.2] - 2018-03-19
### Fixed
- Fixed redirect loop caused by `nginx.ingress.kubernetes.io/force-ssl-redirect`
annotation on ingress resource


## [1.1.1] - 2018-03-16
### Changed
- Disable *silent* SSO by using `kibana-auth-proxy` `v1.1.1`

See: https://github.com/ministryofjustice/analytics-platform-kibana-auth-proxy/pull/2


## [1.1.0] - 2018-03-14
### Changed
- Fixed proxy version/tag instead of using `latest`
- Use newly added `/healthz` endpoint for healthcheck
- Proxy was updated to:
  - use Auth0 hosted login page instead of local login page
  - enabled silent SSO enabled
  - session cookies expire after 1 hour
  - Other changes, see: https://github.com/ministryofjustice/analytics-platform-kibana-auth-proxy/pull/1
