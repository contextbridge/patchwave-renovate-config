# patchwave-renovate-config

A [Renovate](https://docs.renovatebot.com/) preset for repositories that use [PatchWave](https://patchwave.ai).

## Usage

Add the preset to the `extends` list in your Renovate config:

```json
{
  "extends": ["config:recommended", "github>contextbridge/patchwave-renovate-config"]
}
```

## Settings

| Option | Value | Reason |
| ------ | ----- | ------ |
| [`commitBodyTable`](https://docs.renovatebot.com/configuration-options/#commitbodytable) | `true` | Renovate lists each updated package with its old and new version in the commit message. PatchWave reads the updates of a pull request from that table. |

Renovate adds the table the next time it rewrites a branch. For an open pull request, tick the rebase checkbox in the pull request body to get the table sooner.
