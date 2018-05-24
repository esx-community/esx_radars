# esx_radars
Original script: 
- https://github.com/DreanorGTA5Mods/StationaryRadar
- https://forum.fivem.net/t/release-vrp-stationary-radars/70605 - mostly taken from here edited it for ESX. 


## DISCORD

https://discord.me/fivem_esx

## SCREENSHOT

![screenshot](https://i.gyazo.com/27ef5d91e30193948ca01e83bfd571d9.png)

## DESCRIPTION

Speed radar, tickets speeders. 

## To do

~~- Based on speed, how much over the speed limit tickets X amount~~ *DemonReborn
- Sends a bill, instead of automatically taking the money out. 
- The ability to add more spots with different speed limits
- Add vehicle hash list, so cops/ems can get fined when RPing as a civilian

## Requirements

- **pNotify** => https://forum.fivem.net/t/release-pnotify-in-game-js-notifications-using-noty/20659

## Download

**2) Manually**

- Download https://github.com/ESX-PUBLIC/esx_radars/archive/master.zip
- Put it in resource/[esx] directory

**3) Using git**

```
cd resources/[esx]/
git clone https://github.com/ESX-PUBLIC/esx_radars esx_radars
```

## Installation

1) Add folder esx_radars to your [esx] dir
2) Add this in your server.cfg :
```
start esx_radars
```
3) Modify your fine ammounts inside the config.lua
```
Config.Fine 	= 300 -- 10mph over (default: $300)
Config.Fine2 	= 400 -- 20mph over (default: $400)
Config.Fine3	= 500 -- 30mph over (default: $500)
Config.Fine4 	= 600 -- 40mph over (default: $600)
```

4) Add/Remove new radar zones inside client.lua
```
local radares = {
    {x = 379.68807983398, y = -1048.3527832031, z = 29.250692367554},
    {x = -253.10794067383, y = -630.20385742188, z = 33.002685546875},
	
}
```
