# 🍍 bounty-shop.yml

```yaml
title: "&6&lBounty Shop"
size: 27
fill_item:
  display_name: ""
  # Whether it should only fill the borders of the menu with this item.
  # If false it will fill all the menu with it.
  fill_borders_only: true
  material: GRAY_STAINED_GLASS_PANE
back_item:
  display_name: "&cGo back"
  material: BARRIER
  slot: 22
bounty_compass:
  slot: 10
  display_name: "&bBounty Compass"
  material: Compass
  lore:
    - ""
    - "&bTrack down your targets"
    - "&bwith cool particle effects!"
    - ""
    - "&9Price: &e$100 per item"
    - "&9&lRIGHT CLICK &9to buy"
  price: 100
# here you can add custom items (from custom-items.yml)
# Every item inside this section must have a 'id' field that points to section id in custom-items.yml.

custom_items:
  my_shop_item:
    # If true it will use display name,lore,material set in custom-items.yml
    # and what you set here is ignored.
    # NOTE: you must set slot and price and id regardless.
    use_give_item: true
    slot: 11
    id: 'my_custom_item'
    price: 120
# You can set non-sellable items.
others:




```
