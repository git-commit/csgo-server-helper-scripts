# csgo-server-helper-scripts
These scripts help you run mathes with the esl config on your server.

## Starting a match
Be connected to your server and authenticated with your rcon:

1. `rcon exec warmup` a warmup config with more money and easier bunny hopping
2. `rcon exec knife` optional, if you want a knife round
3. `rcon exec swap` optional, if the winning team of the knife round decided to swap
4. `rcon exec live` Start the game!

# Tips
## Adjust your rates for 128 Tick gaming

Add to you launch options: `-tickrate 128`

Create an `autoexec.cfg` in `<steam>\steamapps\common\Counter-Strike Global Offensive\csgo\cfg` with the following contents:

```
// optimised network settings for good connections
rate "128000"
cl_cmdrate "128"
cl_updaterate "128"
cl_interp "0"
cl_interp_ratio "1"
```
