# 🙀 chat\_reactions.yml



```yaml
# + ----------------------------------- + #
# | CHAT REACTION MODULE                | #
# | Let spoofed players talk in chat    | #
# + ----------------------------------- + #
enabled: false
chat_format: "<{player}> {message}" # Format of chat messages, {player} and {message} are required. {prefix} & {suffix} optional
reactions: # List of chat reactions
  # Regex-based reaction
  - trigger: "ca{1,}t" # matches [cat, caat, caaat, ...]
    chance: 0.5 # Chance to react to a message that matches the trigger, 0.5 = 50%.
    responses:
      - "meow"
      - "purr"
      - "i love cats"
  - trigger: "\\bdog\\b" # matches "dog" but not "dogs"
    chance: 1 # Always react to messages that match the trigger.
    responses:
      - "woof"
      - "bark"
      - "i love dogs"
  # Text-based reaction
  - trigger: "i love dogs" # Spoofed players can respond to other spoofed players
    chance: 1
    responses:
      - "i love dogs too, %player_name%!"
      - "dogs are the best"
      - "i love cats more"
```
