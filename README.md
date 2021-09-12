# ungoogled-chromium for Gentoo

*environment for Portage to build www-client/chromium with [ungoogled-chromium](https://github.com/Eloston/ungoogled-chromium) patches*

## Features

* Finds relevant [ungoogled-chromium](https://github.com/Eloston/ungoogled-chromium) version
  by package version. If a version is not available yet in [upstream repository](https://github.com/Eloston/ungoogled-chromium),
  tries finding relevant code in [pull requests](https://github.com/Eloston/ungoogled-chromium/pulls).
  (A pull request with at least 2 approvals from contributors or collaborators is needed.)
  This is because sometimes the upstream repository takes rather a long time to merge
  updates for new versions of Chromium.
* Allows building with Profile Guided Optimizations (PGO)

## Usage

You need to put the `chromium` file into `/etc/portage/env/www-client/chromium`.

This can be done by cloning the repository and than making a symlink, for example.

Afterwards simply emerge chromium with

```
emerge chromium
```
