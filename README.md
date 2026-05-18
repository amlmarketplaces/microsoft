# amlmarketplaces/microsoft

Claude Code marketplace federating all `@amlplugins/microsoft-*` plugins.

## Install

Add to your project's `.claude/settings.json`:

```json
{
  "extraKnownMarketplaces": {
    "aml-microsoft": {
      "source": { "source": "github", "repo": "amlmarketplaces/microsoft" }
    }
  },
  "enabledPlugins": {
      "azure-cosmos-db@aml-microsoft": true,
      "azure-event-grid@aml-microsoft": true,
      "azure-functions@aml-microsoft": true,
      "azure-key-vault@aml-microsoft": true,
      "azure-openai@aml-microsoft": true
    }
}
```

Then launch Claude Code in the project. The marketplace is fetched from `amlmarketplaces/microsoft`, cached under `~/.claude/plugins/cache/aml-microsoft/`, and each enabled plugin is loaded from its `amlplugins` source repo.

## Plugins (13 total)

- `azure-cosmos-db` — [@amlplugins/azure-cosmos-db](https://github.com/amlplugins/azure-cosmos-db)
- `azure-event-grid` — [@amlplugins/azure-event-grid](https://github.com/amlplugins/azure-event-grid)
- `azure-functions` — [@amlplugins/azure-functions](https://github.com/amlplugins/azure-functions)
- `azure-key-vault` — [@amlplugins/azure-key-vault](https://github.com/amlplugins/azure-key-vault)
- `azure-openai` — [@amlplugins/azure-openai](https://github.com/amlplugins/azure-openai)
- `azure-service-bus` — [@amlplugins/azure-service-bus](https://github.com/amlplugins/azure-service-bus)
- `azure-storage-blob` — [@amlplugins/azure-storage-blob](https://github.com/amlplugins/azure-storage-blob)
- `microsoft-graph-calendar` — [@amlplugins/microsoft-graph-calendar](https://github.com/amlplugins/microsoft-graph-calendar)
- `microsoft-graph-drive` — [@amlplugins/microsoft-graph-drive](https://github.com/amlplugins/microsoft-graph-drive)
- `microsoft-graph-mail` — [@amlplugins/microsoft-graph-mail](https://github.com/amlplugins/microsoft-graph-mail)
- `microsoft-graph-sharepoint` — [@amlplugins/microsoft-graph-sharepoint](https://github.com/amlplugins/microsoft-graph-sharepoint)
- `microsoft-graph-teams` — [@amlplugins/microsoft-graph-teams](https://github.com/amlplugins/microsoft-graph-teams)
- `microsoft-graph-users` — [@amlplugins/microsoft-graph-users](https://github.com/amlplugins/microsoft-graph-users)

## Related

- npm packages: `@amlplugins/microsoft-*` published to GitHub Packages (`https://npm.pkg.github.com`).
- Aggregating parent: [`amlmarketplaces/aml`](https://github.com/amlmarketplaces/aml) — federates every `@amlplugins/*` plugin under a single marketplace.
- AML topology: see `.claude/rules/definitions/ageni.md` § "GitHub Topology" — this repository is a Tier-4 HUB-INSTANCE under the `amlmarketplaces/` Tier-3 HUB-ORGANIZATION.

> Built by `.claude/skills/aml/metateam/marketplace/test/cross-org-amlmarketplaces-batch.mjs`.
