---
description: Take a look at our messages config.
---

# 👽 messages.yml

```yaml
prefix: '&6&l[HalosBounty] '
no_permission: '&cYou don''t have the required permission.'
invalid_player: '&cInvalid player.'
player_not_online: '&cThis player is not online.'
correct_usage: '&cCorrect usage: %usage%'
player_bounty_set_self: '&cYou can''t set a bounty on yourself.'
player_bounty_set_fail_target_cooldown: '&cYou can''t set a bounty on that player!
  They are on a cooldown.'
player_bounty_set_fail_self_cooldown: '&cYou can''t set a bounty, you are on a cooldown.
  please wait %cooldown_remaining%.'
player_bounty_set_fail_already_has_bounty: '&cYou can''t set a bounty on that player!
  They already got a bounty.'
player_bounty_set_fail_target_has_too_many_bounties: '&cYou can''t set a bounty on
  that player! They already got a lot of bounties.'
player_bounty_set_fail_target_in_restricted_region: '&cYou can''t set a bounty on
  that player! They are setting on a restricted bounty region.'
bounty_set_reward_too_high: '&cThe reward is too high. max allowed value is %max%'
bounty_set_reward_too_low: '&cThe reward is too low. min allowed value is %min%'
player_bounty_set_success: '&aYou''ve put a bounty on %target% for %reward%.'
# Message sent when bounty increased to maker.
player_bounty_increase_maker: '&aYou increased the bounty on %target% to %reward%'
# Message sent when bounty increased to target.
player_bounty_increase_target: '&cYour bounty has been increased to %reward%'
server_broadcast_bounty_create: '&a%maker% &7has put a bounty on &c%target% &7for
  &b%reward%!'
player_bounty_target_notify: '&c%maker% has put a bounty on you for %reward%. &4&lwatchout!'
auto_bounty_placed: '&cYou killed a player without a bounty! &cA bounty has been put
  on you for &b%reward%.'
bounty_claim_deny_worldguard: '&cYou are not allowed to claim bounties in this region.'
bounty_claim_deny_towny: '&cYou are not allowed to claim bounties from this player.
  they are a member of you town.'
bounty_claim_deny_self_claim: '&cYou didn''t claim that bounty! &cyou are not allowed
  to claim your own bounties.'
bounty_claim_deny_must_target: '&cYou only allowed to claim bounties you are targeting!'
bounty_claim_success: '&aYou claimed a bounty from %target% with total reward of &b%reward%'
wanted_level_increase_player: '&cYour wanted level increased by %increase% because
  you killed a player.'
bounty_track: '&aYou tracked %target%''s bounty for %reward%.'
bounty_untrack: '&cUntracked %target%''s bounty for %reward%.'
bounty_set_command_invalid_player: '&cThis player is not online %target%.'
bounty_set_command_invalid_reward: '&cInvalid reward number %reward%.'
bounty_set_command_insufficient_funds: '&cInsufficient funds, you only have %player_balance%,
  amount needed %needed% to %reward%.'
# This message is set sent when a player runs the remove command, while it searches for bounty data.
bounty_remove_pending: '&eRemoving bounty, please wait.'
# Message sent to player when removing a bounty.
bounty_removed_maker: '&cBounty of %target% has been removed.'
# Message sent to target when a bounty has been removed.
bounty_removed_target: '&c%maker% has dropped the bounty on you.'
bounty_remove_no_bounty_found: '&cYou don''t have any bounties set on %target%'
player_commands_help:
- ''
- '  &5&lBounty Commands'
- ''
- '&f/bounty &8▶ &7&oOpen bounties GUI.'
- '&f/bounty set <reward> <player> &8▶ &7&oSet a bounty on a player.'
- '&f/bounty remove <player> &8▶ &7&oDrops bounty on a player.'
- '&f/bounty help &8▶ &7&oshow this list.'
- ''
bounty_set_help:
- '&cUsage: /bounty set <reward> <player>'
bounty_remove_help:
- '&cUsage: /bounty remove <player>'
wanted_level_increase_mob: '&cYour wanted level increased by %increase% because you
  killed a mob.'
wanted_level_kill_reward: You received %reward% because you killed a player with wanted
  level %level%.
wanted_level_killed: '&cYou were killed so your wanted level was reset.'
# Message sent to player when their wanted level was changed by an admin using /hb setwanted <wanted> <player> true.
wanted_set_admin_command_notification: '&cYour wanted level has been set to %wanted%
  by %admin%'
target_kill_maker_reward: '&aYou claimed x%multi% %reward% bounty reward because you
  killed the bounty maker!'
target_kill_else_reward: '&aYou claimed x%multi% %reward% bounty reward because you
  killed someone while you have a bounty!'
shop_buy_insufficient_funds: '&cInsufficient funds, you only have %player_balance%,
  amount needed %needed% to buy %item%.'
shop_buy_success: '&aSuccessfully bought x1 of %item% for %price%.'

```
