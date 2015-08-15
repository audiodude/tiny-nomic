Any person with a Github account is eligible to play the game (become a player).
However, a single person shall only ever constitute a single player in the game,
regardless of the number of Github accounts he or she has.

To become a player in the game, a candidate player shall send a Github Pull
Request to the master branch of the repository where the game is being recorded.
The Pull Request shall modify the players/ directory of the repository by adding
a single file whose name is exactly in the Name Format.

For the purposes of this rule, the Name Format means a string which:
 
    * Starts with a zero-padded number that must contain 3 digits and be equal
      in numerical value to the number of files that were present in the
      directory before the candidate player's file was added. So if the
      candidate player's file is the 4th, the number would be 003.
    * This is followed by a hyphen, then ends with the Github username of the
      candidate player, ie audiodude.
    * For example, the file could be named `003-audiodude`.

Each player's file must at all times contain the numeric score of the player.

The Pull Request to add a player (as described in this rule) can be
approved/merged by any existing player. Only one player's approval is required.