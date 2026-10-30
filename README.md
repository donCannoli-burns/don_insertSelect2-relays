# insertSelect2-relays

Some KoLmafia relay override scripts which use [don_insertSelect2](https://github.com/donCannoli-burns/don_insertSelect2) to modify pages to make the drop-down menus searchable in the relay browser. Currently supported pages:

* [Decorate Your Eternity Codpiece](https://wiki.kingdomofloathing.com/Decorate_Your_Eternity_Codpiece) ([The Eternity Codpiece](https://wiki.kingdomofloathing.com/The_Eternity_Codpiece) choice adventure)
* [Reminiscing About Those Monsters You Fought](https://wiki.kingdomofloathing.com/Reminiscing_About_Those_Monsters_You_Fought) ([combat lover's locket](https://wiki.kingdomofloathing.com/Combat_lover%27s_locket) choice adventure)

Note that there can only exist one relay script per page, so if you are using any other script that modifies the above listed pages, don't use this repo. Instead, you can install just [insertSelect2](https://github.com/C2Talon/insertSelect2) and manually edit that other script to make use of insertSelect2 to effectively use both at the same time.

## Installation

Can be installed from KoLmafia's CLI via:

```
git checkout https://github.com/donCannoli-burns/don_insertSelect2-relays.git
```

## Additions

Feel free to submit PRs to support additional pages to this repo. Note that there is already a relay script for the [Chest Mimic](https://wiki.kingdomofloathing.com/Chest_Mimic) choice adventures that makes those drop-down menus searchable here: [https://github.com/C2Talon/c2t_megg](https://github.com/C2Talon/c2t_megg)

## Fork provenance and integration

This fork is based on [C2Talon's insertSelect2-relays](https://github.com/C2Talon/insertSelect2-relays) and uses the [insertSelect2 helper](https://github.com/donCannoli-burns/don_insertSelect2) (originally by [C2Talon](https://github.com/C2Talon/insertSelect2)). Credit and original upstream documentation remain with the upstream authors. The installation example above deliberately installs **this fork**, not the upstream checkout.

The related [don_custom_functions](https://github.com/donCannoli-burns/don_custom_functions) project includes a `don_relay_select2.ash` integration helper, but its HTML class-tagging function is **not** a complete substitute for a Select2 browser frontend or these relay overrides.

## Related maintained KoLmafia / ASH projects

- [don-ash-lib](https://github.com/donCannoli-burns/don-ash-lib) — reusable import-safe ASH utilities.
- [don_custom_functions](https://github.com/donCannoli-burns/don_custom_functions) — runnable KoLmafia ASH commands and related relay integration.

These are **separate repositories**, not implicit dependencies installed by this fork. The standalone retirement program for `boneFarm`, `boneTrack.ash`, and `codMaster` is documented at [Retired-KOL-Scripts](https://github.com/donCannoli-burns/Retired-KOL-Scripts). This fork is **not** one of those three retiring scripts.
