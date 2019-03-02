# PMEssentials
A collection of PMMP commands, features and more. Heavily inspired by Essentials
[![HitCount](http://hits.dwyl.io/pmessentials/PMEssentials.svg)](http://hits.dwyl.io/pmessentials/PMEssentials)

## Commands:
List of commands:
- [x] /break
- [x] /feed  
- [x] /gamemode *(custom)*
- [x] /gma
- [x] /gmc
- [x] /gms
- [x] /gmv
- [x] /god
- [x] /heal
- [x] /i
- [x] /nick
- [x] /nuke
- [x] /ping
- [x] /powertool
- [x] /realname
- [x] /size
- [x] /smite
- [x] /speed
- [x] /thru
- [x] /tpa
- [x] /tpaccept
- [x] /tpahere
- [x] /tpdeny
- [x] /tphere
- [x] /tree
- [x] /usage
- [x] /vanish
- [x] /xyz
- [ ] /afk
- [ ] /delhome
- [ ] /delwarp
- [ ] /home
- [ ] /server
- [ ] /sethome
- [ ] /setspawn
- [ ] /setwarp
- [ ] /spawn
- [ ] /tp *(custom)*
- [ ] /tpo
- [ ] /tpohere
- [ ] /warp

## API:
**PMEssentials** has an API for developers can tweak a lot of features and improve them. You can access the UserMap to get users and externally enable things like godmode or vanish. The plugin also has quite a few events you can use to for instance modify command behaviour.

If you want to get the API instance, all you need to do is this:
```php
$api = API::getAPI();
```
You can get the main file too, but you probably won't need it.

Now, let's say you're creating a command and you want it to work on vanished platers. You can use these functions:
```php
//get ALL vanished players
$vplayers = $api->getVanishedPlayers();

//get vanished player from name
$vplayer = $api->getVanishedPlayer("myplayer");
```
It's not hard to use the PME API. If you want something changed in the API you can always open an issue with the API request template.
