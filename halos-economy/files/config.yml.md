---
description: Our main configuration file.
---

# 📃 config.yml

```yaml
# # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
#   _____    ____    ___    _   _    ___    __  __  __   __   #
#  | ____|  / ___|  / _ \  | \ | |  / _ \  |  \/  | \ \ / /   #
#  |  _|   | |     | | | | |  \| | | | | | | |\/| |  \ V /    #
#  | |___  | |___  | |_| | | |\  | | |_| | | |  | |   | |     #
#  |_____|  \____|  \___/  |_| \_|  \___/  |_|  |_|   |_|     #
#                                                             #
#                           WIKI                              #
#                    wiki.halosdev.com                        #
#                                                             #
# # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #

database:
  type: 'sqlite' # sqlite, mysql
  address: 'localhost:3306'
  database: 'database'
  username: 'username'
  password: 'password'

vault:
  enabled: false
  linked-currency: 'tokens'

accounts-save:
  save-delay: 120 # in seconds
  log-in-console: true

ranking-update:
  update-time: 300 # in seconds
  log-in-console: true

```
