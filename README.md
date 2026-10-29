# dwrapper

> **Original project and credit:** [Prusias-kol/pwrapper](https://github.com/Prusias-kol/pwrapper) by Prusias-kol. This is a separate experimental fork maintained at [donCannoli-burns/dwrapper](https://github.com/donCannoli-burns/dwrapper).
>
> **EXPERIMENTAL — USE AT YOUR OWN RISK.** This fork is not guaranteed to be stable or safe. Review settings and scripts before running them, especially commands that spend turns, change inventory, use the mall, PvP, or ascend. The upstream author is not responsible for modifications in this fork.

KoLmafia script wrapper based on the original [pwrapper](https://github.com/Prusias-kol/pwrapper).

## Install, update, and remove

Run these commands in the **KoLmafia gCLI** (not your operating system's Git shell).

**Install**
```
git checkout https://github.com/donCannoli-burns/dwrapper main
```

**Update**
```
git update donCannoli-burns-dwrapper-main
```

**Remove this fork**
```
git delete donCannoli-burns-dwrapper-main
```

If you previously installed the original upstream project, use `git list` to confirm its installed project ID before optionally deleting it with `git delete Prusias-kol-pwrapper-main`. Avoid keeping upstream and fork versions installed simultaneously when they supply the same script filenames.

## Dependencies

None declared.

## Usage

This fork retains the upstream script files and entrypoint names. Consult the installed script's help or source before invoking automated gameplay; the repository name alone does not create a new `dwrapper` CLI command.

## Consolidation / safety migration (2026-10-29)

**Warning: the legacy `scripts/pwrapper.ash` in this repository has automatic retry, choice-option and combat recovery behavior that was not safe to retain unchanged.** Do not use it for unattended gameplay.

A safer, intentionally different successor is now bundled with [dLooper](https://github.com/donCannoli-burns/dLooper): `pwrapper` is read-only status, and `pwrapper run` requires explicit approval before exactly one `ploop fullday` invocation. It never makes automatic choices, auto-fights, or retries a failed run. The old preferences controlling arbitrary CLI and retries are ignored. Install/verify dLooper and then remove this legacy checkout before running the successor; do not keep two `pwrapper.ash` copies.

Experimental; runtime compilation is not yet confirmed.
