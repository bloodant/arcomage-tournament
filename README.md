# arcomage-tournament
Arcomage game emulator for bots tournament

# Configuration format (JSON)
```json
{
    "deck" : "standard", 
    "send_game_session" : "false", 
    "hand_size" : 6,
    "first_turn" : "player1|player2|random",
    "turns_limit" : "number|unlimited",
    "win_condition" : {
        "tower" : 50,
        "resources" : 150
    },
    "start_condition" : {
        "quarries" : 2,
        "magic" : 2, 
        "dungeon" : 2,
        "bricks" : 5, 
        "gems" : 5,
        "recruits" : 5,
        "tower" : 20,
        "wall" : 5
    }
}
```
# Input format (JSON)
```json
{
    "number_of_games" : "1000", 
    "bots" : [
        {
            "name" : "EasyBot",
            "type" : "web|local",
            "path" : "URI"
        }
    ]
}
```
# Message format for bot (JSON)
```json
{
    "deck" : "standard",
    "hand_size" : 6,
    "session" : "number" [optional],
    "win_condition" : {
        "tower" : 50,
        "resources" : 150
    },
    "player_turn" : "1|2",
    "player1_state" : {
        "quarries" : 2,
        "magic" : 2, 
        "dungeon" : 2,
        "bricks" : 5, 
        "gems" : 5,
        "recruits" : 5,
        "tower" : 20,
        "wall" : 5
    },
    "player2_state" : {
        "quarries" : 2,
        "magic" : 2, 
        "dungeon" : 2,
        "bricks" : 5, 
        "gems" : 5,
        "recruits" : 5,
        "tower" : 20,
        "wall" : 5
    },
    "hand" : [
        {
            "id": 1,
            "name": "Mondo Wall",
            "name_rus": "Бастион"
        }, 
        {
            "id": 2,
            "name": "Friendly Terrain",
            "name_rus": "Благодатная почва"
        },
        ...
    ]
}
```

