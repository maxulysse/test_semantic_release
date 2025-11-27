# test_semantic_release

A test repository for [semantic-release](https://semantic-release.gitbook.io/) and [conventional commits](https://www.conventionalcommits.org/).

## Features

- **Automated versioning**: Uses semantic-release to automatically determine the next version number based on commit messages
- **Changelog generation**: Automatically generates a changelog from commit messages
- **Conventional commits**: Uses commitlint to enforce conventional commit message format

## Commit Message Format

This project follows the [Conventional Commits](https://www.conventionalcommits.org/) specification:

```
<type>[optional scope]: <description>

[optional body]

[optional footer(s)]
```

### Types

- `feat`: A new feature (triggers a minor release)
- `fix`: A bug fix (triggers a patch release)
- `docs`: Documentation only changes
- `style`: Changes that do not affect the meaning of the code
- `refactor`: A code change that neither fixes a bug nor adds a feature
- `perf`: A code change that improves performance
- `test`: Adding missing tests or correcting existing tests
- `chore`: Changes to the build process or auxiliary tools

### Breaking Changes

Add `BREAKING CHANGE:` in the commit footer or append `!` after the type/scope to trigger a major release:

```
feat!: remove deprecated API endpoints

BREAKING CHANGE: The /v1/users endpoint has been removed.
```

## Setup

```bash
npm install
```

## License

MIT