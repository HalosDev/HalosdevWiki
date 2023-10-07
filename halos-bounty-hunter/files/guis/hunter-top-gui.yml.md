# 🍍 hunter-top-gui.yml

```yaml
title: "&6&lHunter Top"
size: 36
fill_item:
  display_name: ""
  material: BLACK_STAINED_GLASS_PANE
# Here you can set the items of the leaderboard.
# Each item inside this section must have the 'rank' option.
# The id of each item doesn't matter.
top_players_items:
  top_player:
    display_name: "&6&l#1 &8- &5%player%"
    material: PLAYER_HEAD
    rank: 1
    slot: 4
    lore:
      - ""
      - "&7Claimed bounties: &e%claimed_bounties%"
  top_player_2:
    display_name: "&6&l#%rank% &8- &5%player%"
    material: PLAYER_HEAD
    rank: 2
    slot: 11
    lore:
      - ""
      - "&7Claimed bounties: &e%claimed_bounties%"
  top_player_3:
    display_name: "&6&l#%rank% &8- &5%player%"
    material: PLAYER_HEAD
    rank: 3
    slot: 15
    lore:
      - ""
      - "&7Claimed bounties: &e%claimed_bounties%"
  top_player_4:
    display_name: "&6&l#%rank% &8- &5%player%"
    material: PLAYER_HEAD
    rank: 4
    slot: 20
    lore:
      - ""
      - "&7Claimed bounties: &e%claimed_bounties%"
  top_player_5:
    display_name: "&6&l#%rank% &8- &5%player%"
    material: PLAYER_HEAD
    rank: 5
    slot: 25
    lore:
      - ""
      - "&7Claimed bounties: &e%claimed_bounties%"
others:
  info_item:
    display_name: "&b&lINFO"
    # Can be player_head and it will be the player who is seeing the inventory's head.
    material: BOOK
    slot: 31
    lore:
      - ""
      - "&bThis is the hunter top leaderboard."
      - "&7Players who claimed the MOST bounties "
      - "&7have higher ranks."
      - ""
      - "&eClaim more bounties to earn rewards"
      - "&eAnd be one of the top players!"
      - ""
      - "&e&lYour position %player_rank%"


```
