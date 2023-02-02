# Lamplighter-game
The game is played by two players, referred to as Player 1 and Player 2. The game board consists of two bridges with lamp posts and the players are represented as lamplighters who can turn the lamps on or off as they cross the bridge.

In the initial round, the players choose their starting positions and decide which lamps should be on or off. In subsequent rounds, the players take turns making moves until Player 1 achieves the same board as Player 2 or Player 2 prevents it. A player can either turn a lamp on or off in their current position or move to one of the closest lamps.
////
To implement the lamplighter game with 4 lamps and two players on a computer, a Python code can be written to simulate the game and its rules. The code should take into account the number of lamps, the starting positions of the lamps, the starting positions of the players, and the moves that each player can make. The code should also have the ability to keep track of the state of the game, including the positions of the lamps and the players, and determine when the game has ended.

Here's a description of each function in the code:

ValidMoves: This function takes two arguments, p_p_state and n_p_state, which represent the previous player state and the new player state respectively. The function checks if the new player state is a valid move by comparing the previous and new states. If the lamplighter position has changed, the function checks if the change is by one unit only. If the lamplighter position has not changed, the function checks if a lamp has been toggled. If either of these conditions is true, the function returns True, indicating that the move is valid. If neither condition is true, the function returns False, indicating that the move is invalid.

InitialPosition: This function takes three arguments, board_length, p1_state, and p2_state, which represent the length of the game board, and the starting positions of player 1 and player 2 respectively. The function checks that all the positions entered are within the range of the game board, and returns True if they are, or False if they are not.

Win: This function takes two arguments, p1_state and p2_state, which represent the current positions of player 1 and player 2 respectively. The function checks if the two player states are equal, and returns True if they are, indicating that the game has ended and that one player has won. If the player states are not equal, the function returns False, indicating that the game is still ongoing.

get_player_move: This function gets the player's move by reading the lamplighter position and the positions of the lit lamps from the player's input. The player inputs are first read as strings, then the lamplighter variable is converted to an integer, and the lights variable is converted to a list of integers. The function returns a tuple of the lamplighter position and the list of lit lamp positions.
