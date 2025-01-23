# Welcome to Chess!

This version of chess is built using Haskell and displays an interactive chess board with ASCII characters.

### Instructions:

In order to run the game, you need to have Cabal and Haskell installed on your machine. To do so follow these steps:
1. Install GHCup: 
For Mac/Linux, you can run the command in your terminal: "curl -sSL https://get-ghcup.haskell.org | sh"
For Windows users, you can download GHCup from their website at https://www.haskell.org/ghcup/.
2. After running the installer, the script will guide you through installing GHC, Cabal, and HLS. Accept the default versions unless you have specific requirements.
3. Verify that everything is working by running these three commands:
    - "ghc --version"
    - "cabal --version" and
    - "haskell-language-server --version"
4. Now that you have all three, run these commands to get the project dependencies:
    - "cabal update"
    - "cabal v1-install happy" and
    - "cabal v1-install"
5. You should now be able to run "make" to build the project
6. Finally, you can actually play the game. Run the command "./gambit -h" to see all the different flag options you can use. If you just want to play against the bot then just use "./gambit -i" 

### Notes:

- You make moves using the format <start-colum><start-row>,<end-colum><end-row> like "e2,e4"
- Pawns automatically promote to queens
- You can castle by inputting the king's start and desired end position
- 50 move rule has been replaced by a 200 move limit which draws the game when it hits 0
- Three fold repetition results in a draw as well as every other standard draw rule besides the 50 move rule
- Terminate a game using cmd-c or ctrl-c

## Good luck and have fun!