# PremiumMenuActions
These are the actions that occur inside the PremiumMenus plugin.

[close] - closes the menu

[open] (menu) - opens the certain menu

[console] (command) - dispatches the command

[player_chat] (message) - has the player chat a message

[player] (command) - has the player dispatch a command

[message] (message) - Messages the player

[play_sound] (sound) - Plays a sound

[play_sound] (sound) (volume) (pitch)

[open_parent] - opens the parent menu, if there is a parent menu, it automatically opens on close of the current menu

[status_item] (item) - Pulls a status item from the config.yml


# PremiumMenuConditions
This is how to setup conditional values for the conditional check.

```
        Items:
          '1':
            Priority: 1
            Condition: '%player_name%.equalsIgnoreCase("Warring")'
            Item:
              Material: "BOOK;0" # For 1.13 and above, use BOOK
              Name: "&e&lCondition check"
              Lore:
                - "&7You are cool"
            Actions:
              - "[close]
```

Conditions can be met through placeholders from placeholder API. If these conditions are not met, it will throw an error, because the conditional values are enabled. If you have an error please join my plugin support discord: https://discord.gg/9Z5SZCr
