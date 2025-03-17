# template

## Description

This is a template for a README.md file. It is a markdown file that is used to
describe a project. It is used to provide information about the project to the
users and contributors. It is a good practice to have a README.md file in your
project repository.

## Usage

You can use this template to create a README.md file for your project. You can

- Clone this repository
- Copy the README.md file to your project repository
- Edit the file to add information about your project

### Environment Variables

There are three environment variables that need to be set for this project to
work correctly:

- `PAT` - Your GitHub Personal Access Token
- `GPG_PRIVATE_KEY` - Your GPG Private Key
- `GPG_PRIVATE_KEY_PASSPHRASE` - Your GPG Private Key Passphrase

The `PAT` environment variable is used by MegaLinter to authenticate with the
GitHub API. The `GPG_PRIVATE_KEY` and `GPG_PRIVATE_KEY_PASSPHRASE` environment
variables are used to sign the commits that MegaLinter creates when
`APPLY_FIXES` is set to `true`.

If the MegaLinter action is disabled, none of these environment variables are
required.

### Conventional Commits

This project uses Conventional Commits. Conventional Commits is a specification
for adding human and machine readable meaning to commit messages. It is a
lightweight convention on top of commit messages. The specification can be
found at [conventionalcommits.org](https://www.conventionalcommits.org/).

Specifically, this project uses the
[bitshifted/git-auto-semver](https://github.com/bitshifted/git-auto-semver)
action to automatically increment the version number based on the commit
messages:


- `build`, `chore`, `ci`, `docs`, `fix`, `perf`, `refactor`, `revert`,
  `style`, `test`: bump micro (patch) number
- `feat`: bump minor version number
- `BREAKING CHANGE`: bump major version number

## License

This project is licensed under the Creative Commons License 1.0 Universal
License - see the [LICENSE](LICENSE) file for details.

## Contributing

Contributions are welcome. Please read the [CONTRIBUTING.md](CONTRIBUTING.md)
file for details.

### Code of Conduct

Please read the [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md) file for details on
the code of conduct.  Long story short, be nice to each other and treat each
other with respect, compassion, and empathy, especially when you disagree.

## Authors

- Wes Dean
