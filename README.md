# bump-version

## Usage with circle-ci
```yaml
version: 2
jobs:
    bump_version:
        docker:
            - image: xmorse/bump-version
        environment:
            REPOSITORY: username/repository
        steps:
            - checkout
            - run: GITHUB_TOKEN=$GITHUB_TOKEN /bump
```
