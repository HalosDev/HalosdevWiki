---
description: >-
  This page will be the ultimate guide on to how to setup the plugin to fit your
  server.
---

# 🎙 Setup Guide

## Step 1 - Configure Security Features

First thing that I highly recommend that you do to keep the plugin hidden is change the plugins details. The configuration option can be found in the config.yml .&#x20;

```yaml
plugin_info: # Modify plugin information
  name: "HalosPlayerSpoof" # Name that appears when using /plugins
  authors: [ "HalosDev" ] # Author that appears when using /version
  version: "1.0.0" # Version that appears when using /version
  command_proxy: "spoof" # Change the name of the main plugin command
```

Also recommend configurating the command overrides to fit your server. This is very useful to stop players tping to fake players. The configuration can be found [here](files/command\_overrides.yml.md). &#x20;

## Step 2 - Configure Fluctuation Module

Fluctuation module will be the backbone to how the plugin works and spoofs your player counts. The configuration config may be a little tricky to get correct for your server.&#x20;

```yaml
  percentage: # Percentage of real AND target players to fluctuate by
    # WARNING - Make sure your percentages are large enough to actually fluctuate your player count
    # 10 + 2% = 10.2, which rounds down to 10, so you'll never fluctuate
    minimum: 10
    maximum: 20
```

The main thing that we will be focusing on is the percentages. There will be some trial and error to find the right sweet spot for the percent's. The default configs are good for 2-5 players. But if we are doing 10-20 I suggest min 4 and max 5.&#x20;

```yaml
threshold: # Choose how many players should consistently stay on your server
  minimum: 15
  maximum: 40
```

This field is very important. This will control min and max of spoof players on your server. The percentages will fluctuate in between and will not go under or over.

```yaml
real_player_requirement: 20 # Amount of real players required to start fluctuating
```

This setting will determine at what real player count will flucation turn on. If you have a smaller server I suggest you do 1-5. Bigger servers you can do more.&#x20;

## Step 3 - Configure Ping Module

Setting the ping will make your spoof players look more legit when looked at from the tab list. So it is make sure you set them correctly.&#x20;

```yaml
min_ping: 0 # Minimum ping
max_ping: 1200 # Maximum ping
min_interval: 1000 # Minimum interval, in ticks, between ping changes
max_interval: 2000 # Maximum interval, in ticks, between ping changes
```

The default settings I do not recommend leaving for this field. I suggest min ping 20 and max ping 120-300. You can lower the intervals for ticks to be a lower but I would not recommend lower then 500.

```yaml
show_in_tab: true # Show ping using the yellow number in the tab-list, make sure to disable TAB when using this
```

If you are you using tab and displaying the yellow numbers, you need to have this option on. If this option is true make sure you toggle it to false in the tab config. This option will act as replacement for tabs ping number display. If you are not using the yellow ping numbers in tab toggle this option to false.

## Step 4 - Configure Ranks Module

The ranks module is a very important module to have configured. So that spoofed players will have ranks to match the real players on your server.



```yaml
  name: default # Name does not have to be a set group name already
  prefix: '&7&lMember &7'
  suffix: ''
```

This field will determine the default rank that every spoof player will have. This is the rank that will show even if the module is disabled because spoofed players will need to have a rank. We suggest copying the prefix in Luckperms for your default rank and pasting it in the prefix field.

```yaml
ranks: # List of spoofable ranks. Picked at random. Includes default rank. Ordered by priority.
  - name: vip
    prefix: '&c&lVIP &7'
    suffix: '&r &aVery Swag'
```

This field will only work if the module is enabled. This is only useful if you have ranks that players can gain for free or even paid ranks that you want to promote that people are buying paid ranks. I suggest not using this at the start of a map/season of a gamemode maybe wait like 1-2 days after release.

## Step 5 - Network Player Count Sync

This step is only needed if your server runs bungeecord or velocity network setup. If you run a standalone server then this is not for you.

Start by putting the player spoofer jar on your bungeecord or velocity server. Yes.. it will work on bungeecord and velocity, Halos Player Spoofer is just insane.&#x20;

```yaml
messaging: # Plugin Messaging Settings, only for multi-server setups
  server_id: server1 # Server ID, MUST be unique for each server
  method: "none" # Messaging method, can be 'redis', 'pluginMsg' or 'none'
  # Redis Messaging Settings - Only for 'redis' method
  host: "localhost" # Redis host
  port: 6379 # Redis port
  username: "default" # Redis username, leave blank if none
  password: "" # Redis password, leave blank if none
  ssl: false # Whether to use SSL
```

On the spigot server set the server Id to what ever gamemode the server is. If you are using pluginMsg you do not need to fill out the host, port, username, and password field.&#x20;

If you are using redis you need to fill in the details of your Redis server.

```toml
[messaging] # Plugin Messaging Settings, only for multi-server setups.
method = "none" # Method to use for messaging. Options: "redis", "pluginMsg" or "none"
#Redis Messaging Settings
host = "localhost" # Redis host
port = 6379 # Redis port
username = "default" # Redis username, leave blank if none
password = "" # Redis password, leave blank if none
ssl = false # Whether to use SSL for Redis
```

This is a example of the config on the velocity proxy, It is the same on bungee.  Make sure that you set the method the same to as the sub server.&#x20;

If you are using Redis make sure to set it in the method name and that it is the same info for the Redis server info.
