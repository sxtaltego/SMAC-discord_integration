# SMAC-discord_integration
An edited SMAC.sp that relays ban entry in SMAC.log to designated discord channel. An example relay in the designated discord channel is shown below:

🚨 SMAC Alert: [smac_speedhack.smx | 0.8.8.1] TU VIEJA . EXE (ID: STEAM_1:0:123456789 | IP: 1.1.1.1) is suspected of using speedhack. | Map: c5m4_quarter | Origin: -3062 3103 224 | Angles: 14 -163 0 | Weapon: weapon_autoshotgun | Team: 2 | Latency: 131ms | 🔗 Profile: https://steamcommunity.com/profiles/99999999999999


Instructions:
1. This plugin leverages the core functionality of Discord API plugin by zipcore (https://forums.alliedmods.net/showthread.php?t=292663), which requires steamworks extension (https://users.alliedmods.net/~kyles/builds/SteamWorks/)
2. Add the following field to your /configs/discord.cfg

```sourcepawn
"anticheat"
	{
		"url"	"YOUR DISCORD CHANNEL WEBHOOK"
	}
```
3. Make smac_log_verbose=1 in your /cfg/sourcemod/smac.cfg
