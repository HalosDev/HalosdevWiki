# 🍍 example.yml

```yaml
shop-commands:
  - 'shop example'
  - 'exampleshop'
  - 'testingshop'

shop-gui:
  title: 'Example Shop'
  size: 27
  border:
    enabled: false
    material: 'GRAY_STAINED_GLASS_PANE'
  fill:
    enabled: true
    material: 'GRAY_STAINED_GLASS_PANE'

items:
  1:
    settings:
      inventory-slot: 11
      price: 100.0
      economy: 'tokens'
      commands:
        - 'give %player% diamond 16'
    item:
      material: 'DIAMOND'
      display-name: '&b16 Diamonds'
      lore:
        - '&fPrice: &a%price% tokens'
        - ''
        - '&7&oRight click to buy!'
      amount: 16
  2:
    settings:
      inventory-slot: 15
      price: 500.0
      economy: 'tokens'
      commands:
        - 'give %player% golden_apple 1'
    item:
      material: 'GOLDEN_APPLE'
      display-name: '&d1 Golden Apple'
      lore:
        - '&fPrice: &a%price% tokens'
        - ''
        - '&7&oRight click to buy!'
```
