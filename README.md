# Version Action

A GitHub Action to update the version of a published Action.

## Description

If you're following the GitHub Actions best practices, when publishing a new version of a GitHub Action, after the code is all complete and tested, one must:

1. If release branches are being used, merge the latest changes on the repository's default branch to the release branch
1. Create a new full semver tag for the latest version
1. Delete the old major version tag
1. Create a new major version tag

For example, let's say that the current version of `super-cool-action` is `v1.2.3` and release branches are being used. The things needed to be done would be:

1. Merge `master` into `releases/v1`
1. Create a new tag `v1.2.4` on the latest change in `releases/v1`
1. Delete the tag `v1`
1. Create a new tag `v1` on the latest change in `releases/v1`

## License

[MIT](LICENSE.md)
