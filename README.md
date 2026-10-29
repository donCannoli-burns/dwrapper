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
