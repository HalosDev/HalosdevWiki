# 🍍 bounties-gui.yml

```yaml
title: "&b&lBounties (%current_page%/%pages%)"
size: 54

bounties_per_page: 24
#If true bounties in each page will ignore borders, borders will be empty or filled with fill_item. and boutnies will start at slot 10
# If false bounties will start at slot 0.
is_boxed: true

fill_item:
  display_name: ""
  # Whether it should only fill the borders of the menu with this item.
  # If false it will fill all the menu with it.
  fill_borders_only: true
  material: GRAY_STAINED_GLASS_PANE
self_item:
  slot: 46
  display_name: "%player%"
  material: PLAYER_HEAD
  lore:
    - "&fHeads Collected: &e%heads_collected%"
    - "&fClaimed Bounties: &e%claimed_bounties%"
    - "&fWanted level: &e%wanted_level%"
    - ""
    - "&4Active Bounties:"
    - "%active_bounties%"
    - ""
    - "&fMade Bounties:"
    - "%made_bounties%"
  # for %active_bounties% placeholder above, config each line for each bounty.
  active_bounties_placeholder: "&8- &cBounty from &4%maker% &cfor &b%reward%."
  # for %made_bounties% placeholder above, config each line for each bounty.
  made_bounties_placeholder: "&8- &eBounty on &b%target% &efor &b%reward%."
bounty_shop:
  slot: 51
  display_name: "&6Bounty Shop"
  material: Compass
  lore:
    - ""
    - "&bBuy bounty compass & more!"
next_item:
  slot: 53
  display_name: "&6Next Page"
  material: ARROW
previous_item:
  slot: 45
  display_name: "&bPrevious Page"
  material: Arrow
bounty_item:
  material: "PLAYER_HEAD"
  display_name: "%target%"
  # Values for %status% placeholder.
  status:
    offline: "&8&lOFFLINE"
    active: "&b&lACTIVE"
  lore:
    - "&7Reward: &f%reward%"
    - "&7There is &f%tracking% &7players tracking it."
    - ""
    - "&7By &f%maker%"
    - "&cKill the player to claim the bounty."
    - "&9&lRIGHT CLICK &9to track"
    - ""
    - "&7Status: %status%"
  # The lore to show for target player.
  lore_target:
    - "&7Reward: &f%reward%"
    - "&7There is &f%tracking% &7players tracking it."
    - ""
    - "&7By &f%maker%"
    - ""
    - "&9&lDon't let them kill you!"
  # Lore to show when player is tracking this bounty.
  lore_tracking:
    - "&7Reward: &f%reward%"
    - "&7There is &f%tracking% &7players tracking it."
    - ""
    - "&7By &f%maker%"
    - "&cKill the player to claim the bounty."
    - "&aYou are tracking this bounty."
    - "&4&lRIGHT CLICK &cto untrack"
    - ""
    - "&7Status: %status%"
# Other items that is not bind to an action by default.
# You can add item at in slot, it will override the above items if the slot intersects with one of them.
others:
  info_item:
    slot: 48
    display_name: "&bInfo"
    material: BOOK
    lore:
      - "&aHow to create a bounty?"
      - "&eDo /bounty create <player> <reward>"

```
