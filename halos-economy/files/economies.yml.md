---
description: Main config to configure each economy.
---

# 🤑 economies.yml

```yaml
economies:
  tokens: # id
    currency-type: 'VIRTUAL' # PHYSICAL, VIRTUAL
    display-name: 'Tokens'
    initial-amount: 100.0 # players will start with this balance
    command:
      base: 'tokens'
      aliases:
        - 'token'
        - 'etoken'
        - 'etokens'
    physical-item:
      material: 'GOLD_NUGGET'
      display-name: '&6&lTokens'
      lore:
        - '&fAmount: &6%amount% tokens'
      glow: true
    bank:
      enabled: true # show currency in /bank
      display-item:
        material: 'GOLD_NUGGET'
        display-name: '&6&lTokens'
        lore:
          - '&fYour balance: &6%balance% %economy%'
          - ''
          - '&7Click to manage the bank!'
        glow: false
        slot: 13
    settings:
      tradeable: true # enable '/<currency> pay' command
      ranking: true # enable '/<currency> top' command
    convertor:
      enabled: true
      convert-to: 'gems' # economy-id
      exchange-rate: 10.0 # percentage %
    loans:
      enabled: true
      values:
        min-loan: 10000.0
        max-loan: 1000000.0
      loan-interest: 15.0 # percentage %
  gems: # id
    currency-type: 'PHYSICAL' # PHYSICAL, VIRTUAL
    display-name: 'Gems'
    initial-amount: 0.0 # players will start with this balance
    command:
      base: 'gems'
      aliases:
        - 'gem'
    physical-item:
      material: 'DIAMOND'
      display-name: '&d&lGems'
      lore:
        - '&7&oCustom economy'
      glow: true
    bank:
      enabled: false # show currency in /bank
      display-item:
        material: 'DIAMOND'
        display-name: '&d&lGems'
        lore:
          - '&fYour balance: &6%balance% %economy%'
          - ''
          - '&7Click to manage the bank!'
        glow: false
        slot: 13
    settings:
      tradeable: true # enable '/<currency> pay' command
      ranking: true # enable '/<currency> top' command
    convertor:
      enabled: false
      convert-to: '?' # economy-id
      exchange-rate: 10.0 # percentage %
    loans:
      enabled: false
      values:
        min-loan: 500.0
        max-loan: 10000.0
      loan-interest: 25.0 # percentage %
```
