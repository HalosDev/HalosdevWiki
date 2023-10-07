---
description: Messages config. Customize each message.
---

# 👽 messages.yml



```yaml
messages-prefix: '&6&l[Giveaways]'

general:
  command-usage:
    - '{prefix} &cUsage: /{usage}'
  no-permission:
    - "{prefix} &cYou don't have enough permissions."
  help-command:
    - ''
    - '&6&l Giveaway Commands'
    - ''
    - '&f /giveaways &8▶ &7&oOpen giveaways GUI.'
    - '&f /giveaway start <id> &8▶ &7&oStart a new giveaway.'
    - '&f /giveaway end <id> &8▶ &7&oEnd an ongoing giveaway.'
    - '&f /giveaway join &8▶ &7&oOpen giveaways GUI.'
    - '&f /giveaway rig <id> <player> &8▶ &7&oSet the winner of the giveaway.'
    - '&f /giveaway reload &8▶ &7&oReload all configurations.'
    - ''
  reload-command:
    - '{prefix} &aConfigurations successfully reloaded!'

giveaways:
  giveaway-already-running:
    - '{prefix} &cThere is already a giveaway with this id running.'
  giveaway-not-found:
    - '{prefix} &cNo giveaway was found with this id.'
  giveaway-started:
    - '{prefix} &fYou have started a new giveaway with id %id%!'
  giveaway-ended:
    - '{prefix} &fGiveaway with id %id% have ended!'
  giveaway-rig:
    - '{prefix} &fWinner for giveaway with id %id% set to %player%.'
  giveaway-join:
    - '{prefix} &aYou entered the giveaway. The result will be in %end_at%.'
  giveaway-leave:
    - '{prefix} &fYou left the giveaway.'
```
