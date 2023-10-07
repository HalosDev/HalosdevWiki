# 🏴󠁧󠁢󠁳󠁣󠁴󠁿 command\_overrides.yml

```yaml
# + ----------------------------------- + #
# | COMMAND OVERRIDES                   | #
# | Prevent other plugins from leaking  | #
# | the real player count.              | #
# + ----------------------------------- + #

prevent_spoof_player_commands: true # Prevent any player from running commands on spoofed players
default_fail_message: "&cUnable to execute command, please try again later..."

# - TELEPORT -
# Override the /tp command to prevent issues with spoofed players
teleport:
  allow_tp: true # Allow players to teleport to spawned spoofed players
  success_messages:
    teleported: "&aTeleported to &e{target}&a!"
    teleported_other: "&e{player} &ahas been teleported to &e{target}&a!"
  fail_message: # Messages to be sent if player cannot be teleported
    - "&cUnable to teleport teleport, please try again later"

# - LIST -
# Override the /list command to prevent revealing the real player count
list:
  allow_list: true # Override the /online command
  aliases: # Aliases for the /online command
    - "list"
  format: # Messages to be sent when using /list, supports PlaceholderAPI and built-in placeholders
    - "&6There are &c{total_online} &6out of a maximum &c{max_players} &6players online."
    - "&6Players: &c{players}"

# - CUSTOM OVERRIDES -
# Add your own custom command overrides here
# Supports PlaceholderAPI and built-in placeholders, {total_spoofed} and {total_online}
custom_overrides:
  online: # /online
    messages: # Messages to be sent when using /online
      - "&aThere are currently &e{total_online}&a players online!"


```
