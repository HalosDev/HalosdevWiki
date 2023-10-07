# 🍍 bounty-top-gui.yml

```yaml
title: "&6&lBounty Top"
size: 36
fill_item:
  display_name: ""
  material: BLACK_STAINED_GLASS_PANE
# Here you can set the items of the leaderboard.
# Each item inside this section must have the 'rank' option.
# The id of each item doesn't matter.
# You can use any bounty placeholder here, %target%, %maker%, %reward%
top_bounties_items:
  top_bounty:
    display_name: "&6&l#1 &8- &5%target%"
    material: PLAYER_HEAD
    rank: 1
    slot: 4
    lore:
      - ""
      - "&7Reward: &e%reward%"
  top_bounty_2:
    display_name: "&6&l#2 &8- &5%target%"
    material: PLAYER_HEAD
    rank: 2
    slot: 11
    lore:
      - ""
      - "&7Reward: &e%reward%"
  top_bounty_3:
    display_name: "&6&l#%rank% &8- &5%target%"
    material: PLAYER_HEAD
    rank: 3
    slot: 15
    lore:
      - ""
      - "&7Reward: &e%reward%"
  top_bounty_4:
    display_name: "&6&l#%rank% &8- &5%target%"
    material: PLAYER_HEAD
    rank: 4
    slot: 20
    lore:
      - ""
      - "&7Reward: &e%reward%"
  top_bounty_5:
    display_name: "&6&l#%rank% &8- &5%target%"
    material: PLAYER_HEAD
    rank: 5
    slot: 25
    lore:
      - ""
      - "&7Reward: &e%reward%"
others:
  info_item:
    display_name: "&b&lINFO"
    # Can be player_head and it will be the player who is seeing the inventory's head.
    material: BOOK
    slot: 31
    lore:
      - ""
      - "&5Bounties with the top rewards will"
      - "&5be displayed here."





```
