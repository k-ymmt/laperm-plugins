# Laperm Plugin Catalog

`catalog.json` is the list [Laperm](https://github.com/k-ymmt/Laperm) shows under File → Manage Plugins… →
Catalog. Listing is a pointer to where a Plugin lives, not a review of what it does: Laperm shows every
Plugin's Permissions before installing it.

To list a Plugin, open a pull request adding an entry:

```json
{ "id": "<manifest id>", "repo": "<owner>/<repository>", "name": "<name>", "description": "<one line>", "author": "<name>" }
```

The repository must publish GitHub Releases carrying `manifest.json` and `plugin.wasm` (see the
[template](https://github.com/k-ymmt/laperm-plugin-template)); `id` must equal the Manifest's `id`.
