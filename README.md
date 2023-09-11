## Tell us more

Currently renovate (36.92) doesn't support Gitlab's locale import with wildcard. <https://docs.gitlab.com/ee/ci/yaml/#includelocal>

Running it on this repository, the PR for updating the base elixir image will be created for `.gitlab_the_third.yml` but not for `.gitlab_ci_2.yml` and `.gitlab_ci_1.yml` because they are included into `.gitlab-ci.yml` via wildcard.

## Expected

For the include wildcard to be interpreted correctly by Renovate and have the base image update PR to include all the yml files.
