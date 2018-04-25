# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).


## [0.2.3] - 2018-04-25
### Fixed
- Added permissions required to list pods and pods' metrics
- Fixes logging

### Changed
- Better handling of unhealthy pods (missing metrics data)
- See [related PR](https://github.com/ministryofjustice/analytics-platform-idler/pull/10)


## [0.2.2] - 2018-04-25
### Fixed
- Fixes Docker image missing `metrics_api` package
- See [PR](https://github.com/ministryofjustice/analytics-platform-idler/pull/9)


## [0.2.1] - 2018-04-20
### Fixed
- Fixes idler incorrectly idling RStudio instances using more CPU
  than the threshold (`RSTUDIO_ACTIVIY_CPU_THRESHOLD`).
  See [PR with fix](https://github.com/ministryofjustice/analytics-platform-idler/pull/8)
- Don't use `latest` as idler image tag as it's not predictable


## [0.2.0] - 2018-03-16
### Changed
- Add env var `RSTUDIO_ACTIVIY_CPU_THRESHOLD` to configure what counts as an
  active RStudio deployment and so whether to skip idling.
- Add permission to read from Resource Metrics API
