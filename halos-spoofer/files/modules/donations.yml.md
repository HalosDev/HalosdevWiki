# 💸 donations.yml

```yaml
# + ----------------------------------- + #
# | DONATION MODULE                     | #
# | Run command and send messages when  | #
# | a spoofed player 'donates'.         | #
# + ----------------------------------- + #
enabled: false
max_interval: 12000 # Maximum interval in ticks between donations
min_interval: 6000 # Minimum interval in ticks between donations
donations: # List of donations. Picked at random.
  - messages: # List of messages to broadcast when a spoofed player donates.
      - "&e%player_name% bought a round for everyone!"
    commands: # List of commands to execute when a spoofed player donates.
      - "give %player_name% minecraft:milk_bucket"
```
