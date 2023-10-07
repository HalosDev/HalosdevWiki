# 🗒 votes.yml



```yaml
# + ----------------------------------- + #
# | VOTES MODULE                        | #
# | Run command and send messages when  | #
# | a spoofed player 'votes  '.         | #
# + ----------------------------------- + #
enabled: false
max_interval: 12000 # Maximum interval in ticks between votes
min_interval: 6000 # Minimum interval in ticks between votes
votes: # List of votes. Picked at random.
  - messages: # List of messages to broadcast when a spoofed player votes.
      - "&e%player_name% voted for the server! Golden Apple for everyone!"
    commands: # List of commands to execute when a spoofed player votes.
      - "give %player_name% minecraft:golden_apple"
```
