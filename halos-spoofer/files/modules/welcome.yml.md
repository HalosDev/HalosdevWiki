# 🙉 welcome.yml





```yaml
# + ----------------------------------- + #
# | WELCOME MODULE                      | #
# | Send a welcome message from spoofed | #
# | players when a player joins the     | #
# | server for the first time.          | #
# + ----------------------------------- + #
enabled: false
welcome_chance: 0.5 # Chance to send a welcome message when a new player join, 0.5 = 50%.
chat_format: "<{player}> {message}" # Format of chat messages, {player} and {message} are required. {prefix} & {suffix} optional
messages: # Messages picked at random, supports PlaceholderAPI and built-in placeholder {player}
  - welcome :)
  - hi {player}!
  - o/
```
