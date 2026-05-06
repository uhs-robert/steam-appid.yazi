# ✨ What's New / 🚨 Breaking Changes

Please skim using the icons below for quick navigation, focus on what matters most to you:

- **(🚨) BREAKING CHANGE:** Breaking changes, respect the siren
- **(✨) Feat:** New features, follow the sparkles
- **(🔧) Internal:** Internal architectural changes, maintains a wrench

> [!NOTE]
> This file tracks user-facing changes across releases: new features, breaking changes, and internal architectural shifts.
>
> Because this is a small, focused plugin, most future entries will be compatibility updates for new Yazi versions rather than feature additions.
>
> See the [README](./README.md) for full setup and configuration docs.

## v1.0.0 — Initial Release

**(✨) Feat:** Linemode plugin that resolves Steam AppIDs to game names in Yazi.

- Reads `appmanifest_<id>.acf` files from your `steamapps` directory and displays the `name` field inline
- Activates automatically for `appmanifest_*.acf` files and numeric ID folders inside `steamapps/downloading/`, `compatdata/`, `shadercache/`, and `temp/`
- In-session memory cache, repeated lookups don't re-read disk
- Configurable `steamapps_paths` for multiple Steam libraries
- Configurable icon (defaults to Nerd Font steam icon `󰓓`, set to `""` to disable)
- Requires Yazi 0.25+
