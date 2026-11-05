# CyberPanel

Official **PeltyCMS** `provisioning` WASM addon (`provisioning-cyberpanel`).

## Install

1. Open Pelty Admin → Addons → Marketplace
2. Set registry URL to `https://market.mythicalsystems.org/api/pelty/addons/registry.json`
3. Download **CyberPanel**

Marketplace: https://market.mythicalsystems.org/marketplace/product/provisioning-cyberpanel  
Product ID (CI): `59`

## Develop

This repository is a git submodule of [MythicalLTD/PeltyCMS](https://github.com/MythicalLTD/PeltyCMS) at `extensions/addons/prov-cyberpanel`.

```bash
# from the PeltyCMS monorepo
cargo xtask addons prov-cyberpanel
```

## Release (Mythic Marketplace)

Same flow as [featherpanel-com/PterodactylPanelApi](https://github.com/featherpanel-com/PterodactylPanelApi):

1. Repo secrets: `MYTHIC_PRODUCT_ID`, `MYTHIC_RELEASE_TOKEN`
2. Repo variable: `ADDON_DIR=prov-cyberpanel`
3. Actions → **Release Addon** → Run workflow

Publishes the packed `provisioning-cyberpanel.zip` via `MythicalLTD/.github/actions/publish-release@v1` and creates a GitHub Release.
