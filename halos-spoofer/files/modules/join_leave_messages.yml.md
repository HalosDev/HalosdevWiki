# 💯 join\_leave\_messages.yml

```yaml
# + ----------------------------------- + #
# | JOIN/LEAVE MESSAGE MODULE           | #
# | Send join/leave messages when       | #
# | spoofing players.                   | #
# + ----------------------------------- + #
enabled: false
chance: 0.5 # Chance to broadcast a message when a spoofed player joins, 0.5 = 50%.
join_messages: # List of messages to announce when a spoofed player joins. {player} is required.
  - "&e{player} joined the game"
leave_messages: # List of messages to announce when a spoofed player leaves. {player} is required.
  - "&e{player} left the game"
```
