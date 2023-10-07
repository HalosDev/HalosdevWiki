# 🍍 example.yml

```yaml
display-name: '2x Sell Multiplier'

# available types: PERSONAL, GLOBAL
booster-type: 'PERSONAL'

booster-settings:
  duration: 3600 # time in seconds
  # available boosts: money, jobs, skills, economy-id (in HalosEconomy plugin)
  boosts:
    - 'money;2.0' # boost-id;multiplier
  effects:
    - 'SPEED;1' # effect type;amplifier

actions:
  activation:
    commands: []
    message:
      enabled: true
      sound: 'ENTITY_PLAYER_LEVELUP;2.0;2.0' # sound;volume;pitch
      message:
        - ''
        - '&f You have activated a &a%display-name%'
        - '&f booster for &a1 hour&f!'
        - ''
  expiration:
    commands: []
    message:
      enabled: true
      sound: '?' # ? = sounds disabled
      message:
        - ''
        - '&f Your &a%display-name% &fbooster has ended!'
        - ''

shop:
  price: 10000.0
  # available economies: money, economy-id (in HalosEconomy plugin)
  economy: 'money'
  inventory-slot: 13
  item:
    material: 'PLAYER_HEAD'
    head-texture: '87d885b32b0dd2d6b7f1b582a34186f8a5373c46589a273423132b448b803462'
    display-name: '&6%display-name%'
    lore:
      - '&fPrice: &a$10,000'
      - '&fDuration: &a1 hour'
      - ''
      - '&6&oRight click to buy!'

gui:
  inventory-slot: 22
  items:
    activate:
      material: 'PLAYER_HEAD'
      head-texture: '87d885b32b0dd2d6b7f1b582a34186f8a5373c46589a273423132b448b803462'
      display-name: '&6%display-name%'
      lore:
        - ''
        - '&f Gives you a &a%display-name%'
        - '&f booster to make money faster!'
        - ''
        - '&f Duration: &a1 hour'
        - ''
        - '&fYou have &a%amount% boosters.'
        - '&6&oClick to activate!'
    deactivate:
      material: 'PLAYER_HEAD'
      head-texture: '87d885b32b0dd2d6b7f1b582a34186f8a5373c46589a273423132b448b803462'
      display-name: '&6%display-name%'
      lore:
        - ''
        - '&f Gives you a &a%display-name%'
        - '&f booster to make money faster!'
        - ''
        - '&f You still have &a%time%'
        - '&f of booster duration!'
        - ''
        - '&c&oClick to deactivate!'
```
