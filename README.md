## Tell us more

Currently renovate (36.92) doesn't support Gitlab's locale import with wildcard. <https://docs.gitlab.com/ee/ci/yaml/#includelocal>

Running it on this repository, the PR for updating the base elixir image will be created for `.gitlab_ci_3.yml` but not for `.gitlab_ci_2.yml` and `.gitlab_ci_1.yml` because they are included into `.gitlab_ci.yml` via widlcard.

I'd expect the wildcard to be interpreted correctly by Renovate.
