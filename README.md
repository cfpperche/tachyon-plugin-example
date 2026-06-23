# tachyon-plugin-example (`hello-guard`)

A minimal [Tachyon](https://github.com/cfpperche/tachyon) plugin, for trying the **Plugins View** end to end.
It wires a single, harmless `SessionStart` hook for **claude** and **codex** that prints a greeting — no side effects.

## Install
In the Tachyon **Plugins** panel, add by source: `github:cfpperche/tachyon-plugin-example@v1.0.0`

## Layout
- `tachyon-plugin.json` — manifest (name, version, runtimes, block paths)
- `claude/hooks.json` + `claude/greet.sh` — claude SessionStart hook
- `codex/hooks.json` + `codex/greet.sh` — codex SessionStart hook

`${TACHYON_PLUGIN_ROOT}` in a hook command is rewritten to the plugin's materialized payload root on install.
