# Batman™: Arkham Asylum Game of the Year Edition

[Epic store page](https://www.epicgames.com/store/en-US/product/batman-arkham-asylum/home)

[Game saves zip](./Batman.Arkham.Asylum.Saves.zip)

The saves start (`Save0 - Copy.sgd`) a bit before croc where the game got stack and I realized that sharing these saves may be valuable for some folks.

Save games are normally located at `%USERPROFILE%\Documents\Square Enix\Batman Arkham Asylum GOTY\SaveData\0000000000000000`

Save0.sgd is the first game slot, Save1.sgd is the second etc

`Save0 - Copy (3).sgd`, `Save0 - Copy (4).sgd` etc are various backups I did while playing the game. Rename them to Save0.sgd to restore from there.


## Game cheats

Replace the `%USERPROFILE%\Documents\Square Enix\Batman Arkham Asylum GOTY\BmGame\Config\BmInput.ini` file with [this one](./BmInput.ini) and make it read-only (file gets replaced when starting the game). The only difference from the vanilla file are the following lines:

``` ini
Bindings=(Name="F9",Command="TeamTalk")
Bindings=(Name="F10",Command="savegamehere")
Bindings=(Name="F11",Command="set engine.playercontroller bgodmode true")
Bindings=(Name="F12",Command="set BmGame.RBMPawnAI bBatarangCanKill true")
```

- F9: Brings up the team talk line. You can delete the TeamTalk and use that command line to pass commands like `set engine.playercontroller bgodmode true`
- F10: This doesn't seem to work. Found it from another batman but never made it work.
- F11: God mode
- F12: Batarang instantly kills opponents

There is a wide list of cheat codes available:
- `set engine.playercontroller bgodmode true`: Invincibility
- `set pawn health 0001`: loose if you get hit once
- `set BmGame.RBMPawnAI bBatarangCanKill true`: Kill opponents with one hit from batarang
- `set bmgame.rgrapplegun maxgrappleheight 999999999`: Extra Long Grapple
- `set rpawnplayerbm  bUseDamageMeshes false`: Repaired Batsuit

For infected Batman skin:
```
Set RPawnPlayerCombat AdditionalCombatAnimSet AnimSet'Joker_Combat_Anims.Anims.Joker_Combat_Anims'
Set RPawnPlayerCombat OverrideThugCombatAnimSet AnimSet'Thug_Anims.JokerSpecific_Anims.Thug_JokerSpecificCombat_Anims'
Set RPawnPlayerCombat StunMoveProp SkeletalMesh'Game_Pickups.Spraycan.SprayCan_forAnimation'
Set RPawnPlayerCombat AutoStrikeAnimSet AnimSet'Joker_Combat_Anims.Anims.Joker_Combat_Anims'
Set RPawnPlayerCombat StunMoveProp SkeletalMesh'Game_Pickups.Spraycan.SprayCan_forAnimation'
```
