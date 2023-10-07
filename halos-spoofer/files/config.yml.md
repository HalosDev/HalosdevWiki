# 📄 config.yml

```yaml
# + ----------------------------------- + #
# | PLUGIN SETTINGS                     | #
# | General plugin settings.            | #
# + ----------------------------------- + #

plugin_info: # Modify plugin information
  name: "HalosPlayerSpoof" # Name that appears when using /plugins
  authors: [ "HalosDev" ] # Author that appears when using /version
  version: "1.0.0" # Version that appears when using /version
  command_proxy: "spoof" # Change the name of the main plugin command

messaging: # Plugin Messaging Settings, only for multi-server setups
  server_id: server1 # Server ID, MUST be unique for each server
  method: "none" # Messaging method, can be 'redis', 'pluginMsg' or 'none'
  # Redis Messaging Settings - Only for 'redis' method
  host: "localhost" # Redis host
  port: 6379 # Redis port
  username: "default" # Redis username, leave blank if none
  password: "" # Redis password, leave blank if none
  ssl: false # Whether to use SSL

general_settings: # Main plugin settings
  max_players: 1000 # Max players displayed on server list
  visibility_chance: 0.5 # Chance to spawn a spoofed player that's visible to other players, 0.5 = 50%
  show_in_tab: true # Show spoofed players in the tab list
```
