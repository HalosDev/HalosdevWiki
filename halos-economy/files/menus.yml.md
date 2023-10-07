---
description: We allow you to config each menu.
---

# 📄 menus.yml

```yaml
bank-menu:
  title: 'Bank'
  size: 27
  items:
    gray-glass:
      material: 'GRAY_STAINED_GLASS_PANE'
      display-name: '&f'
      slots: [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26]

bank-manage-menu:
  title: 'Bank - Manage Currency'
  size: 27
  items:
    deposit-item:
      material: 'JUKEBOX'
      display-name: '&6Deposit %economy%'
      lore:
        - '&fBalance: &7%balance% %economy%'
        - ''
        - '&7Click to deposit!'
      slot: 11
      actions:
        PLAY_SOUND: BLOCK_NOTE_BLOCK_BASS;1.0;1.0
    withdraw-item:
      material: 'HOPPER'
      display-name: '&6Withdraw %economy%'
      lore:
        - '&fBalance: &7%balance% %economy%'
        - ''
        - '&7Click to withdraw!'
      slot: 15
      actions:
        PLAY_SOUND: BLOCK_NOTE_BLOCK_BASS;1.0;1.0
    current-loan-item:
      material: 'MAP'
      display-name: '&6Loans'
      lore:
        - '&7You have an active loan,'
        - '&7see details below:'
        - ''
        - '&8 - &fLoan amount: &6%amount% %economy%'
        - '&8 - &fMissing to pay: &6%missing% %economy%'
        - ''
        - '&aClick to pay off your loan.'
      hide-flags: true
      slot: 13
    enabled-loans-item:
      material: 'MAP'
      display-name: '&6Loans'
      lore:
        - '&fMin loan: &7%min-loan% %economy%'
        - '&fMax loan: &7%max-loan% %economy%'
        - ''
        - '&fLoan interest: &c%loan-interest%%'
        - ''
        - '&7Click to take a loan!'
      hide-flags: true
      slot: 13
    disabled-loans-item:
      material: 'MAP'
      display-name: '&cLoans'
      lore:
        - '&7This currency does not'
        - '&7allow loans.'
      hide-flags: true
      slot: 13
      actions:
        PLAY_SOUND: ENTITY_VILLAGER_NO;1.0;1.0
    gray-glass:
      material: 'GRAY_STAINED_GLASS_PANE'
      display-name: '&f'
      slots: [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 12, 14, 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26]

convertor-menu:
  title: 'Convert Currency'
  size: 54
  items:
    converting:
      slot: 19
    result:
      slot: 25
    confirm-item:
      material: 'CHEST_MINECART'
      display-name: '&6Confirm Exchange'
      lore:
        - '&7Exchanging %converting% for %result%.'
        - ''
        - '&fExchange rate: &a%exchange-rate%%'
        - '&fYou will receive &a%amount% %result%&f.'
        - ''
        - '&7Click to confirm!'
      slot: 4
    set-amount-item:
      material: 'OAK_SIGN'
      display-name: '&6Set Amount'
      lore:
        - '&fCurrent amount: &a%amount%'
        - ''
        - '&7Click to set the amount'
        - '&7of %converting% to convert'
      glow: true
      slot: 31
      actions:
        PLAY_SOUND: BLOCK_NOTE_BLOCK_BASS;1.0;1.0
    close-item:
      material: 'BARRIER'
      display-name: '&c&lCancel Conversion'
      lore: []
      slot: 49
      actions:
        CLOSE_INVENTORY: true
        PLAY_SOUND: BLOCK_CHEST_CLOSE;1.0;1.0
    black-glass:
      material: 'BLACK_STAINED_GLASS_PANE'
      display-name: '&f'
      slots: [0, 1, 2, 3, 5, 6, 7, 8, 12, 13, 14, 30, 32, 36, 37, 38, 39, 40, 41, 42, 43, 44, 45, 46, 47, 48, 50, 51, 52, 53]
    white-glass:
      material: 'WHITE_STAINED_GLASS_PANE'
      display-name: '&f'
      slots: [9, 10, 11, 15, 16, 17, 18, 20, 21, 22, 23, 24, 26, 27, 28, 29, 33, 34, 35]
```
