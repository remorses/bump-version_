# bump-version

## Usage with circle-ci
```yaml
version: 2
jobs:
    bump_version:
        docker:
            - image: xmorse/bump-version
        environment:
            GITHUB_TOKEN: xxx
            REPOSITORY: username/repository
        steps:
            - checkout
            - run: /bump
```
