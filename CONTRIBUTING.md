# Contributing to Expressive Code

Thank you for your interest in contributing to this project! We welcome all contributions, big or small. Before you get started, please take a moment to review our guidelines.

## Getting Started

To get started, please fork the repository and clone it to your local machine. Then, create a new branch for your changes:

```sh
git checkout -b my-new-feature
```

Make your changes and commit them with a descriptive commit message:

```sh
git commit -m "Add new feature"
```

Push your changes to your fork:

```sh
git push origin my-new-feature
```

Finally, open a pull request against the `main` branch of the original repository.

## Development Process

We use [GitHub Flow](https://guides.github.com/introduction/flow/) for our development process. This means that all changes should be made in a feature branch and submitted as a pull request against the `main` branch.

## Package Manager

We use [pnpm](https://pnpm.io/) as our package manager. Please make sure to install pnpm and update it to the latest version before working on this project.

## Code Style

We use ESLint and Prettier to enforce a consistent code style across all packages. Please make sure that your changes pass the linter before submitting a pull request:

```sh
pnpm lint
```

## Testing

All changes should be tested before submitting a pull request. Please make sure that all tests pass before submitting your changes.

If you're adding a new feature, please also add tests for it. If you're fixing a bug, please add a test that reproduces the bug.

The root package includes a helpful shortcut that you can use to build all packages, run all tests, and lint your code:

```sh
pnpm validate
```

## Changesets

We use [Changesets](https://github.com/changesets/changesets) to manage our releases. Unless your changes only affect the documentation or internal packages, please make sure to add a changeset for your changes before submitting a pull request:

```sh
pnpm changeset
```

When asked about the packages to be included in the changeset, please select the packages that you've changed. Regarding the type of change, please select `minor` for new or changed features and `patch` for bug fixes. Major releases will be handled by the maintainers.

If you have made changes that should be visible to users of the high-level integration packages, please also add `expressive-code`, `remark-expressive-code` and `astro-expressive-code` to the changeset. This will ensure that the full description of your changes is included in these public-facing CHANGELOG.md files as well, instead of only appearing as a dependency update.

## Documentation

Please make sure that all changes are properly documented. This includes code comments and updates to the README.md files of the affected packages (in case of user-facing changes).

## Issues and Bugs

If you find a bug or issue, please report it on our [issue tracker](https://github.com/expressive-code/expressive-code/issues).

## License

By contributing to this project, you agree to license your contributions under the [MIT License](LICENSE).