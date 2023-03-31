# setup-cicada-action

Currently, you need to provide a token to access cicada release repo with GH_TOKEN

Example:

```yml
name: 'Cicada Action'
on: [push]

jobs:
  build:
    runs-on: ubuntu-latest
    env:
      GH_TOKEN: ${{ secrets.GH_TOKEN }}
    steps:
      - name: Checkout
        uses: actions/checkout@v3
      - uses: cicadahq/setup-cicada@v1.0.0
      - run: cicada -V
```
