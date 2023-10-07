# 🧑🤝🧑 fluctuation.yml

```yaml
# + ----------------------------------- + #
# | FLUCTUATION MODULE                  | #
# | Natural Player Fluctuation          | #
# + ----------------------------------- + #
enabled: true
algorithm: # Customize the fluctuation settings to match your server
  delay: # Delay between player count changes
    minimum: 10
    maximum: 20
  percentage: # Percentage of real AND target players to fluctuate by
    # WARNING - Make sure your percentages are large enough to actually fluctuate your player count
    # 10 + 2% = 10.2, which rounds down to 10, so you'll never fluctuate
    minimum: 10
    maximum: 20
threshold: # Configure the minimum and maximum player count
  minimum: 15
  maximum: 40
real_player_requirement: 20 # Amount of real players required to start fluctuating

```
