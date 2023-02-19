# OHD-Pterodactyl
This is a pterodactyl egg for the game Operation Harsh: Doorstop report any bugs in the issues tab.



## Ports

7777 - Game Port (Inbound UDP; in the command line argument this is represented as “-Port=”)

7778 - Steam Client Port (Outbound UDP; this is always the Game Port +1)

7779 - RCON Port (Inbound TCP; the “ListenPort” in Game.ini)

27005 - Steam Query Port (Inbound UDP; in the .bat command line argument this is represented as “-QueryPort=”)
## Configure
Once server is installed check the HarshDoorstopServer.sh you need to set the ports that you have assigned to the server manually for map settings i reccomend using [Map Query Generator](https://hub.afocommunity.com/OHDTools/QueryGenerator) made by afo.
This is an example startup
```
"$UE4_PROJECT_ROOT/HarshDoorstop/Binaries/Linux/HarshDoorstopServer-Linux-Shipping" HarshDoorstop khafji_P?BluforFaction=DEFAULT?OpforFaction=DEFAULT?MinPlayers=0?MaxPlayers=64?BluforNumBots=0?OpforNumBots=0?BluforNumTickets=500?OpforNumTickets=500 -SteamServerName="Harsh Doorstop Dedicated Server" -Port=7777 -QueryPort=27005 -RCONPort=7779  $@ 
```

## Credits
rehlmgaming@gmail.com - Used his egg "Satisfactory" as a base since Satisfoctory is a UE Game.
