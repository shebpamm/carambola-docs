# CS:GO Commands
This category of commands is prefixed by **pug** or alternatively **scrim**, **cs** or **csgo**.

## Query
| Full Command   | Shorter Version |
|----------------|-----------------|
|C! pug query new|  C! cs q new    |


Start a query for a new pick-up game with this command.

## Start
| Full Command | Shorter Version |
|--------------|-----------------|
| C! pug start |     C! cs s     |

Starts the pick-up game when there are 10 participants.

## Cancel/Stop
| Full Command  | Shorter Version |
|-------------- |-----------------|
| C! pug cancel |    C! cs cls    |

*Restores almost everything back to a state where no game or query is active.*

Stops currently running pick-up game or query and stops the game server.

## Link
| Full Command  | Shorter Version |
|-------------- |-----------------|
|  C! pug link  |   C! cs link    |

*This is required for participating in a pick-up game. Only needs to be run once.*

Carambola will send you a link where you can connect your Steam ID to Carambola.

## Resume
| Full Command    | Shorter Version |
|-----------------|-----------------|
|  C! pug resume  |   C! cs res     |

If a pick-up game is starting but all players haven't linked yet Carambola will pause until this command is ran.

## Config
| Full Command    | Shorter Version |
|-----------------|-----------------|
|  C! pug config  |   C! cs cfg     |

This command is used to configure the proper settings for Carambola to run pick-up games.

|   Name      | Description                                                                                   |      Full Command                 |
|-------------|-----------------------------------------------------------------------------------------------|-----------------------------------|
|   Role      | Role that should be given to players<br> that want to participate in pugs.                    | C! cs cfg role @example           |
|   Channel   | Channel where Carambola posts the query messages and does the game setup .                    | C! cs cfg channel \<ex-channel\>  |
|useActiveRole| When **true** a role is assigned to everyone <br>who is interested in participating in a pug. | C! cs cfg useActiveRole **false** |
| activeRole  | Role that is given to players when useActiveRole is **true**.                                 | C! cs cfg activeRole @example     |
| pingOnQuery | When **true**, pings the role assigned above when creating a new query.                       | C! cs cfg pingOnQuery **false**   |

<br><br>

# Utility/Management
|             Full Command          | Shorter Version |
|-----------------------------------|-----------------|
|  C! utility query *title* *count* |   C! util q     |

Creates a new query with a given title and optionally an target player count.<br>
Queries expire after a day and there can be multiple running at the same time.
