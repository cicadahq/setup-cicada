# setup-cicada

Set up your GitHub Actions workflow with the latest version of Cicada

Currently, you need to provide a token to access cicada release repo with GH_TOKEN

## Usage

### Latest

```yaml
- uses: cicadahq/setup-cicada@v1
  env:
    GH_TOKEN: ${{ secrets.GH_TOKEN }}
```