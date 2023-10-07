---
description: Our menu config.
---

# 📄 menus.yml



```yaml
giveaways-menu:
  title: '&lAvailable Giveaways'
  size: 36
  paginated-layout: # O = content, < = previous page, > = next page and X = empty
    - 'OOOOOOOOO'
    - 'OOOOOOOOO'
    - 'OOOOOOOOO'
    - '<XXXXXXX>'
  items:
    join-giveaway:
      material: 'PAPER'
      display-name: '&aGiveaway'
      lore:
        - '&8Ending in %end_at%'
        - ''
        - '&f Rewards:'
        - '&8 - &f%rewards%'
        - ''
        - '&7%participants% participants'
        - '&a&lCLICK TO JOIN'
    leave-giveaway:
      material: 'PAPER'
      display-name: '&aGiveaway'
      lore:
        - '&8Ending in %end_at%'
        - ''
        - '&f Rewards:'
        - '&8 - &f%rewards%'
        - ''
        - '&7%participants% participants'
        - '&c&lCLICK TO LEAVE'
    empty-item:
      material: 'COBWEB'
      display-name: '&cNo giveaways found!'
      lore:
        - '&7There is no giveaways'
        - '&7occurring now.'
    previous-page:
      material: 'SPECTRAL_ARROW'
      display-name: '&c&lPrevious Page'
      lore:
        - '&7Click to go to the'
        - '&7previous page.'
      slot: 27
    next-page:
      material: 'SPECTRAL_ARROW'
      display-name: '&e&lNext Page'
      lore:
        - '&7Click to go to the'
        - '&7next page.'
      slot: 35
    fill-items:
      material: 'GRAY_STAINED_GLASS_PANE'
      display-name: '&f'
      slots:
        - 27
        - 28
        - 29
        - 30
        - 32
        - 33
        - 34
        - 35
    close-inventory:
      material: 'BARRIER'
      display-name: '&c&lClose Inventory'
      lore:
        - '&7Click to close!'
      slot: 31
      actions:
        CLOSE_INVENTORY: true
        PLAY_SOUND: 'BLOCK_CHEST_CLOSE;1.0;1.0' # sound;volume;pitch
```
