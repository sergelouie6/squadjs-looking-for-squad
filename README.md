# SquadJS Looking For Squad Plugin
This plugin can be used to warn squad leaders of the same team that a player is looking for a squad.

## Dependency
This plugin is dependent to the changes of [this](https://github.com/Team-Silver-Sphere/SquadJS/pull/313) pull request.

### Options
#### commands
###### Description
Command to trigger the plugin.
###### Default
```
["!lfs", "!look", "!invite"]
```
#### rateLimit
###### Description
Number of seconds that must pass before the same user can trigger the command again.
###### Default
```
60
```
#### warnLockedOnly
###### Description
Whether to warn locked squads only or both locked and unlocked squads.
###### Default
```
true
```

### Example configuration
```json
{
    "plugin": "LookingForSquad",
    "enabled": true,
    "discordClient": "discord",
    "channelID": "1167860946396528671",
    "commands": ["!lfs", "!look", "!invite"],
    "rateLimit": 15,
    "warnLockedOnly": false,
    "logToDiscord": false
}
```
