# .travis-ci

Repository of [reusable configuration](https://docs.travis-ci.com/user/build-config-imports)
for Travis CI

<!-- status badges -->
[![Build Status][ci-badge]][ci-link]

## Usage

<!-- consumer badges -->
[![MIT license][license-badge]][license-link]

### Importing into other form8ion projects

All configs in this repository can be [imported](https://docs.travis-ci.com/user/build-config-imports)
into the configuration of projects within the `form8ion` organization. This
includes the configs prefixed with `authenticated-` because the
[shared encrypted secrets](https://docs.travis-ci.com/user/build-config-imports#sharing-encrypted-secrets)
are accessible across the organization.

### Importing into projects outside of the form8ion organization

Many of the configs in this repository are intended for use beyond the
`form8tion` organization and are even assumed to be available by the
[travis-scaffolder-javascript](https://github.com/travi/travis-scaffolder-javascript).

:warning: The configs prefixed with `authenticated-` are not available for use
outside of the `form8ion` organization because the
[shared encrypted secrets](https://docs.travis-ci.com/user/build-config-imports#sharing-encrypted-secrets)
are not accessible outside the organization. However, it is recommended that
you make configs available with the same name in your own `.travi-ci`
repository in order to align with the assumption by the
[travis-scaffolder-javascript](https://github.com/travi/travis-scaffolder-javascript)
that these are available.

## Contributing

<!-- contribution badges -->
[![Conventional Commits][commit-convention-badge]][commit-convention-link]
[![Commitizen friendly][commitizen-badge]][commitizen-link]
[![PRs Welcome][PRs-badge]][PRs-link]

### Dependencies

```sh
$ nvm install
$ npm install
```

### Verification

```sh
$ npm test
```

[license-link]: LICENSE
[license-badge]: https://img.shields.io/github/license/form8ion/.travis-ci.svg
[ci-link]: https://travis-ci.com/form8ion/.travis-ci
[ci-badge]: https://img.shields.io/travis/com/form8ion/.travis-ci/master.svg
[commit-convention-link]: https://conventionalcommits.org
[commit-convention-badge]: https://img.shields.io/badge/Conventional%20Commits-1.0.0-yellow.svg
[commitizen-link]: http://commitizen.github.io/cz-cli/
[commitizen-badge]: https://img.shields.io/badge/commitizen-friendly-brightgreen.svg
[PRs-link]: http://makeapullrequest.com
[PRs-badge]: https://img.shields.io/badge/PRs-welcome-brightgreen.svg
