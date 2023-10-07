---
description: Our main config file.
---

# 📄 config.yml



```yaml
# Enable or disable hooks here.
hooks:
  # If enabled it will prevent players from claiming bounties from players in the same town.
  towny: false

  # If true it will register worldguard flags 'bountyclaim', 'bountymake' flags, you can disable each one of them in worldguard section.
  worldguard: false
  vault: true
# The cooldown to set bounties on one player.
player_bounty_cooldown: 5s
# Cooldown for bounty set.
bounty_set_cooldown: 1m
# If true, it will be possible to set multiple bounties on single player; in that case the killer will claim all bounties.
# If false it will only allow one bounty to set on each player; and will send the 'already_has_bounty' fail message or will increase bounty (see increase_bounty option) if there is already a bounty on that player.
allow_multiple_bounties: true
# IF 'allow_multiple_bounties' option is true, this defines the max bounties allowed in one player.
max_allowed_bounties: 2
# Should it increase bounty if bounty command is used on a player that already has a bounty?
# If set to true, running the bounty command will make the new bounty reward: <old reward> + <new reward>
# If false it will send 'already_has_bounty' fail message or allow multiple bounties depending on 'allow_multiple_bounties' option.
increase_bounty: true
# Extra money to pay on bounty create.
# you could use fixed amount (ex: '1000')
# Or percentage (2%) of the bounty reward.
bounty_create_tax: '1000'
# Use this for placeholders in case no maker defined (e.g for automatic bounties, admin created bounties).
default_bounty_maker: "Server"
# The minimum and maximum allowed value for bounties rewards.
bounty_reward:
  min: 1000
  max: 2000000
bounty_restrictions:
  # If true it will prevent players from claiming their own bounty.
  prevent_claim_self: true
  # If true only players who is targeting a bounty will be able to claim it.
  only_targeters: true
  # Here you choose what do if there is multiple bounties on a player.
  # Valid options are:
  # claim_all: claim all bounties.
  # claim_random: claim a random bounty
  # claim_first: claim the first bounty that was set (deprecated)
  multiple_bounties: 'claim_all'
bounty_claim_actions:
  # Whether or not to drop target's head when he's killed with a bounty.
  drop_player_head_on_bounty_claim: true
  # Commands to execute on bounty claim.
  # You can execute commands as the target, killer and console.
  # To run the command as target: put 'target;' before the command with slash
  # To run the command as killer: put 'killer;' before the command with slash
  # To run the command as console: put 'console;' before the command without slash
  # Available placeholders: %killer%, %target%.
  execute_commands:
    - "target;/say i got killed"
    - "killer;/say I claimed bounty"
    - "console;say a bounty has been claimed by %killer% from %target%"
wanted_level:
  # The amount wanted level increases on mob kill. could be 0
  increase_kill_mob: 1
  # The amount wanted level increases on player kill. could be 0
  increase_kill_player: 2
  star_char: "★"
  # Range of reward per minimum wanted level.
  # usage: <from value>-<to value> (it chooses a random value in this range)
  # If a specific wanted level is not specified the value of the max wanted level before this level will be used.
  # Example: If target's level is 7 with the current configurations the range will be the range specified for level 5 which '99999-100000'
  # Example 2: If target's level is greater than or equal to 10 with the current configurations the range will be the range specified for level 10 which '100000-1000000'
  rewards:
    1: 100-1000
    2: 1000-10000
    3: 10000-50000
    4: 50000-99999
    5: 99999-100000
    10: 100000-1000000
# This section decides what happens when a player with bounty on himself kills another player.
bounty_target_kill:
  kill_bounty_maker:
    # Set to 0 if: you don't want to give bounty reward to the target.
    # Set to more than 1 if: you want to give bounty reward, the amount decides the multiplier of it.
    # Setting it to 2 will give double the bounty reward to the target if he kills the bounty maker.
    give_bounty_reward_multiplier: 1
    # Whether it should drop bounty from target if he kills the player who set the bounty.
    drop_bounty: true
  kill_else:
    # Set to 0 if: you don't want to give bounty reward to the target.
    # Set to more than 1 if: you want to give bounty reward, the amount decides the multiplier of it.
    # Setting it to 2 will give double the bounty reward to the target if he kills someone.
    give_bounty_reward_multiplier: 1
    # Whether it should drop bounty from target if he kills someone.
    drop_bounty: true
# If true: it will not show bounties (on GUIs) whose target is offline, and all players targeting it will automatically untarget it.
# If false: bounties will stay even if target is offline, and they will be still show in GUIs as offline bounties, and it will show target is offline on compass and GPS.
disable_offline_bounties: true
leaderboard:
  hunter_top_refresh_interval: 5m
  wanted_top_refresh_interval: 5m
  bounty_top_refresh_interval: 5m
GPS:
  enabled: true
  text:
    active: "%target% | %distance%"
    offline: "&5&lTarget offline"
    dead: "&c&lTarget Dead"
  boss_bar:
    color: BLUE
    style: SOLID
compass:
  enabled: true
  item:
    display_name: "&4&lBOUNTY COMPASS"
    material: COMPASS
    lore:
      - ""
      - "&5Used to track down bounties!"
      - ""
      - "&bCan be bought from bounty shop."
  # The max length of the particle line that points towards bounty.
  # 5-10 is recommended. more than 10 is discouraged.
  particle_line_length: 10
  # The interval to show compass particles in.
  # In ticks. 1 second = 20 ticks
  show_interval: 20
  # Allow holding the compass in offhand.
  allow_offhand: true
autobounty:
  enabled: true
  chance: 50
  bypass_permission: 'halosbounty.autobounty.bypass'
  # Reward range for autobounty reward, format: <from number>-<to number>
  reward_range: 10000-1000000
storage:
  type: "json"
  # The interval in which players data is saved.
  players_save_interval: 1m
  # Whether it should debug to console info about saving operations.
  debug_console_save: true
  mysql:
    host: "localhost"
    port: 3306
    database: "halosbounty"
    user: "root"
    password: "root"
    players_table: "users"
    bounty_table: "bounties"
```
