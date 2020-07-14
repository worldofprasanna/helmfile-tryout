# helmfile-tryout

[![standard-readme compliant](https://img.shields.io/badge/standard--readme-OK-green.svg?style=flat-square)](https://github.com/RichardLitt/standard-readme)

Use Helmfile to orchestrate the Helm charts

## Table of Contents

- [Install](#install)
- [Usage](#usage)
- [Maintainers](#maintainers)
- [Contributing](#contributing)
- [License](#license)

## Install

```
brew install kubectl
brew install helm
brew install helmfile
```

## Usage

Make sure you point to the correct kubernetes cluster.
```
# To see the diff
helmfile diff --environment dev|qa

# To apply the changes
helmfile apply --environment dev|qa
```

## Todo

Write about usage of Values folder, values.yaml.gotmpl
1. Support for multiple environments
2. Support for secrets (helm secrets) & configs
3. AWS KMS to encrypt / decrypt secrets
4. Have common configs & secrets and include that for all environments
5. Different KMS for different envs


## Maintainers

[@worldofprasanna](https://github.com/worldofprasanna)

## Contributing

PRs accepted.

Small note: If editing the README, please conform to the [standard-readme](https://github.com/RichardLitt/standard-readme) specification.

## License

MIT © 2020 Prasanna
