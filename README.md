# arcomage-tournament
Arcomage game emulator for bots tournament

# Configuration format (JSON)
```json
{
    "deck" : "standard", <br />
    "send_game_session" : "false", <br />
    "hand_size" : 6,<br />
    "first_turn" : "player1|player2|random",<br />
    "turns_limit" : "number|unlimited",<br />
    "win_condition" : {<br />
        "tower" : 50,<br />
        "resources" : 150<br />
    },<br />
    "start_condition" : {<br />
        "quarries" : 2,<br />
        "magic" : 2, <br />
        "dungeon" : 2,<br />
        "bricks" : 5, <br />
        "gems" : 5,<br />
        "recruits" : 5,<br />
        "tower" : 20,<br />
        "wall" : 5<br />
    }<br />
}<br />
<br />
```
# Input format (JSON)<br />
{<br />
    "number_of_games" : "1000",<br /> 
    "bots" : [<br />
        {<br />
            "name" : "EasyBot",<br />
            "type" : "web|local",<br />
            "path" : "URI"<br />
        }<br />
    ]<br />
}<br />
<br />
# Message format for bot (JSON)
{<br />
    "deck" : "standard",<br />
    "hand_size" : 6,<br />
    "session" : "number" (optional),<br />
    "win_condition" : {<br />
        "tower" : 50,<br />
        "resources" : 150<br />
    }<br />
    "player_turn" : "1|2",<br />
    "player1_state" : {<br />
        "quarries" : 2,<br />
        "magic" : 2,<br /> 
        "dungeon" : 2,<br />
        "bricks" : 5, <br />
        "gems" : 5,<br />
        "recruits" : 5,<br />
        "tower" : 20,<br />
        "wall" : 5<br />
    },<br />
    "player2_state" : {<br />
        "quarries" : 2,<br />
        "magic" : 2, <br />
        "dungeon" : 2,<br />
        "bricks" : 5, <br />
        "gems" : 5,<br />
        "recruits" : 5,<br />
        "tower" : 20,<br />
        "wall" : 5<br />
    },<br />
    "hand" : [<br />
        {<br />
            "id": 1,<br />
            "name": "Mondo Wall"<br />
        }, <br />
        {<br />
            "id": 2,<br />
            "name": "Friendly Terrain"<br />
        }<br />
    ]<br />
}<br />