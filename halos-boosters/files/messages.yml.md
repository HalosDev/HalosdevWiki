---
description: Take a look at our messages config.
---

# 👽 messages.yml

```yaml
# {prefix} = return 'messages-prefix' value
# other placeholders: %player%, %booster%, %amount%

messages-prefix: '&6&l[Boosters]'

general:
  not-for-console:
    - '{prefix} &cThis command is exclusive for players!'
  command-usage:
    - '{prefix} &cUsage: /%usage%'
  no-permission:
    - "{prefix} &cYou don't have enough permissions."
  subcommand-does-not-exist:
    - '{prefix} &cThis subcommand does not exist!'
  player-not-found:
    - '{prefix} &cThe user %player% is not online.'
  booster-not-found:
    - "{prefix} &cThe booster '%booster%' does not exist."

commands:
  help:
    - ''
    - '&5&l Boosters Commands'
    - ''
    - '&f /boosters &8▶ &7&oOpen boosters GUI.'
    - '&f /boosters shop &8▶ &7&oOpen booster shop GUI.'
    - '&f /booster give <player> <booster> <amount> &8▶ &7&oGive a player a booster.'
    - '&f /booster remove <player> <booster> &8▶ &7&oRemove a booster from player.'
    - '&f /booster reload &8▶ &7&oReload all configurations.'
    - '&f /booster help &8▶ &7&oShow plugin commands.'
    - ''
  give:
    - '{prefix} &aYou have given %amount%x %booster% Booster to %player%.'
  remove:
    - '{prefix} &aYou have removed %amount%x %booster% Booster from %player%.'
  reload:
    - '{prefix} &aConfigurations successfully reloaded!'

boosters:
  insufficient-funds:
    - '{prefix} &cYou need $%price% money to buy this booster!'
  successfully-purchased:
    - '{prefix} &aYou bought a &6%display-name% Booster&a for $%price%!'
  insufficient-boosters:
    - '{prefix} &cYou do not have a booster to use.'
  booster-deactivated:
    - '{prefix} &cSuccessfully deactivated your &6%display-name% Booster&c.'
```
