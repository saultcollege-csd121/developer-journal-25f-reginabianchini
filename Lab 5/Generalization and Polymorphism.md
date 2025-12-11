1. Why can you change the type of the returned value in promptForPlayer without changing the return type in the function signature?

    >Because HumanPlayer is a type of player, this way it can do everything a player does and more.
    
1. Explain why the error occurred initially and why adding the abstract method signature fixes the error. (HINT: What is the type of the ‘whoseTurn’ variable in TicTacToeGame.doNextTurn?)
    > The type of whoseTurn is a Player. Meaning that the function was not created in Player. After fixing it I told the code that the function actually already existed.
   
1. Explain in detail (using the terminology we have discussed in class) how it is possible that neither our main method nor our TicTacToeGame class need change at all when adding new Player types to our game. Your discussion must include an explanation of how the single call to pickNextMove in TicTacToeGame.doNextTurn works correctly no matter whose turn it is or which types the players are.
    > It is possible because the Player class is a parent, the other players are the child of it. Meaning that the other Players are like branches of Players, they can be Player. The call to pickNextMove in TicTacToeGame.doNextTurn works correctly, because the other players when created where given the same properties of Player.