# Randomly Occuring Upsets Let Even Trailing Troublemakers Excel

In a game played on GitHub, an _upset_ occurs when the merge commit hash for a recently accepted rule-change begins with `0`.

In an offline game, flip a fair coin four times after every accepted rule-change proposal. An _upset_ occurs if it shows heads for all four flips.

When an upset occurs, each player's score becomes their successive player's score. 

The last player's successive player is the first player.

The score rotation occurs _before_ application of any score changes for that turn or pull request.

(This rule only applies to merge commits created by clicking "Merge" on a successful pull request to this repository. Merge commits created with a local git client and pushed to the repository, for example, do not invoke this rule.)

(The score updates for all players may be performed by any player, submitted by pull request, and merged by any player.)

(A change to update a player's score for the turn may be combined with the change to rotate all players' scores in a single pull request.)

(It is possible that this PR will result in a merge commit that re-triggers this rule, possibly more than once.)
