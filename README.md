# 10 Man Bot
This is a bot that facilitates a 10 man lobby (for Valorant or other games) with auto moving features.

It requires a config.yaml file with the fields `team_a`, `team_b`,`lobby`, `scheme`, and `maps`, which signify the channel names for each team, drafting scheme, and map pool.

You must also save your Discord Bot API key in the `DISCORD_KEY` environment variable.

## Installation

Verify that you have Python 3.7 or later and run the following

```python -m pip install -r requirements.txt```

and then run the bot with

```python main.py```

## Setup

If you would like to prevent any user from being captain, simply add their name to `blacklist.txt`.

You should configure the maps and channel names in config.yaml if the provided ones do not match your channel setup.

## Commands

`!help` : Lists all commands

`!new`  : Starts new game, but does not select captain

`!nc`    : Starts new game and selects captains

`!setcaps @<cap1> @<cap2>` : Manually sets the captains to specified users

`!ban <map_name>` : Bans provided map from map pool

`!draft @<player_name>` : Drafts user to your team (you must be captain to use this command)


`How to set the token` : $env:YOUR_BOT_TOKEN="GET_THE_TOKEN_FROM_DISCORD_BOT_IN_THE_NEW_APP"
`In the end just run the main file` : python main.py
`Download and Install python first` : https://www.python.org/ftp/python/3.12.6/python-3.12.6-amd64.exe
`Remember there will be 2 checkboxes when you open the .exe file check them both they are important or your code wont work in other terminals`
`Install discord.py` : pip install discord.py>=1.3.3
`Install yaml` : pip install pyyaml>=4.2b1

