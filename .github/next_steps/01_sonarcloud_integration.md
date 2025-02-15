---
title: 'Next step: Sonarcloud integration'
---

Continuous code quality can be handled by [Sonarcloud](https://sonarcloud.io/). This repository is configured to use Sonarcloud to perform quality analysis and code coverage report on each push.

In order to configure Sonarcloud analysis [GitHub Action workflow](https://github.com/NPLinker/nplinker/blob/main/.github/workflows/sonarcloud.yml) you must follow the steps below:

1. go to [Sonarcloud](https://sonarcloud.io/projects/create) to create a new Sonarcloud project
1. login with your GitHub account
1. add Sonarcloud organization or reuse existing one
1. set up a repository
1. go to [new code definition administration page](https://sonarcloud.io/project/new_code?id=NPLinker_nplinker) and select `Number of days` option
1. To be able to run the analysis:
   1. a token must be created at [Sonarcloud account](https://sonarcloud.io/account/security/)
   1. the created token must be added as `SONAR_TOKEN` to [secrets on GitHub](https://github.com/NPLinker/nplinker/settings/secrets/actions)
