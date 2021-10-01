# release-drafter template action
The template repository for [Release Drafter](https://github.com/marketplace/actions/release-drafter)

## Usage
You can use the release-drafter-run-action in a Github Actions by configuring 
a Yaml file, e.g. `.github/workflows/release-drafter.yml` with the following:

```
on: 
  push:
    branches:
      - main
  pull_request:
    types: [opened, synchronize]

jobs:
  rostest_job:
    runs-on: ubuntu-latest
    name: A job to rostest
    steps:
      - id: release-drafter
        uses: sbgisen/release-drafter-run-action@main
```
