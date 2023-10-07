---
description: Our custom items file.
---

# 🪁 custom-items.yml



```yaml
# CUSTOM ITEMS CONFIG
# HERE YOU CAN SETUP ITEMS TO SELL IN BOUNTY SHOP
# YOU CAN ALSO SET NBT TAGS. (String/boolean/int)
my_custom_item:
  display_name: "&bSuper Cool Item"
  material: LAPIS_BLOCK
  lore:
    - "&5Super cool!"
    - ""
    - "&eYou can sell your own custom items,"
    - "&eAnd integrate them with other plugins!"
  # The NBT tags of item to integrate with other plugins.
  NBT:
    - key: "CUSTOM_KEY"
      # Possible types: string/int/boolean
      type: "string"
      value: "CUSTOM VALUE"
```
