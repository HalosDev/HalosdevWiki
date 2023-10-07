---
description: Our main config file.
---

# 📄 config.yml



```yaml
# # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
#     ____     ___     ___    ____   _____   _____   ____    ____     #
#    | __ )   / _ \   / _ \  / ___| |_   _| | ____| |  _ \  / ___|    #
#    |  _ \  | | | | | | | | \___ \   | |   |  _|   | |_) | \___ \    #
#    | |_) | | |_| | | |_| |  ___) |  | |   | |___  |  _ <   ___) |   #
#    |____/   \___/   \___/  |____/   |_|   |_____| |_| \_\ |____/    #
#                                                                     #
#                                WIKI                                 #
#                          wiki.halosdev.com                          #
#                                                                     #
# # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #

database:
  type: 'sqlite' # sqlite, mysql
  address: 'localhost:3306'
  database: 'database'
  username: 'username'
  password: 'password'

shop-gui:
  title: '&3&lBooster Shop'
  size: 27
  border:
    enabled: false
    material: 'GRAY_STAINED_GLASS_PANE'
  fill:
    enabled: true
    material: 'GRAY_STAINED_GLASS_PANE'

boosters-gui:
  title: '&3&lBooster'
  size: 45
  border:
    enabled: true
    material: 'GRAY_STAINED_GLASS_PANE'
  fill:
    enabled: false
    material: 'GRAY_STAINED_GLASS_PANE'
```
