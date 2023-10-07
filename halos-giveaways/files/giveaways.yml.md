---
description: Our giveaways config. This is where all the magic happens.
---

# 🎁 giveaways.yml



```yaml
giveaways:
  example: # id
    giveaway-duration: 300 # in seconds
    broadcast-message:
      start:
        enabled: true
        sound: 'ENTITY_PLAYER_LEVELUP;2.0;2.0' # sound;volume;pitch
        message:
          - ''
          - '&6&l GIVEAWAYS! &fA new giveaway has started!'
          - '&7 Check it out now at /giveaways.'
          - ''
      end:
        enabled: true
        sound: 'ENTITY_PLAYER_LEVELUP;2.0;2.0' # sound;volume;pitch
        message:
          - ''
          - '&6&l GIVEAWAYS! &fThe giveaway has ended!'
          - '&7 Winner: &f%winner%'
          - ''
          - '&f Rewards:'
          - '&8 - &716x Diamonds'
          - '&8 - &71x Rare Key'
          - ''
    rewards:
      1:
        name: '16x Diamonds'
        command: 'give %player% diamond 16'
      2:
        name: '1x Rare Key'
        command: 'crates give %player% rare 1'
    auto-start:
      enabled: true
      schedules:
        - '08:00 AM'
        - '10:00 AM'
        - '01:00 PM'
        - '05:00 PM'
        - '10:00 PM'
        - '01:00 AM'
  example2: # id
    giveaway-duration: 300 # in seconds
    broadcast-message:
      start:
        enabled: true
        sound: 'ENTITY_PLAYER_LEVELUP;2.0;2.0' # sound;volume;pitch
        message:
          - ''
          - '&6&l GIVEAWAYS! &fA new giveaway has started!'
          - '&7 Check it out now at /giveaways.'
          - ''
      end:
        enabled: true
        sound: 'ENTITY_PLAYER_LEVELUP;2.0;2.0' # sound;volume;pitch
        message:
          - ''
          - '&6&l GIVEAWAYS! &fA new giveaway has started!'
          - '&7 Check it out now at /giveaways.'
          - ''
    rewards:
      1:
        name: '16x Emeralds'
        command: 'give %player% emerald 16'
      2:
        name: '5x Epic Keys'
        command: 'crates give %player% epic 1'
    auto-start:
      enabled: false
      schedules: []
```
