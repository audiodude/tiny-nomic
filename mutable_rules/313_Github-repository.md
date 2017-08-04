# Github repository

Each rule shall be represented by a file in the git repository where the game
is being recorded.

Mutable rules must be located in the `mutable_rules/` directory.

Immutable rules must be located in the `immutable_rules/` directory.

No other files in the repository shall be constituted to represent a rule or
have the force of a rule.

The master branch of the repository will serve as the canonical representation
of the current game state.

No commits are allowed to be made to the master branch except through the
mechanism of a Github Pull Request.

The changes made by a Pull Request must perform one of the following actions:

1. Add a rule file, when the corresponding rule is enacted.
2. Remove a rule file, when the corresponding rule is repealed.
3. Modify a rule file, when the corresponding rule is amended.
4. Move a rule file to another directory, when the corresponding rule is transmuted.
5. Add a player file, when a player joins the game
6. Modify a player file, when a player's score changes
7. Remove a player file, when a player leaves the game
8. Perform some administrative task on the repository, at the discretion of the
   players.
9. Some other action, except that the action must be outlined in a current,
   valid rule other than this one.

When a rule file is modified or transmuted, it may also be renamed to satisfy
rules governing the names of rules.

When a rule change is proposed (items 1--4 above), in addition to the one
action performed above, a pull request may also perform modifications to any
number of other files, including mutable rules files but excluding immutable
rules files, which affect or are affected by the proposal.
These modifications are not considered "amendments," but instead
"administrative edits."
Administrative edits must be in the service of keeping the rules coherent in
their reference to other rules and avoidance of self-contradiction, and may not
change the spirit of any rules other than that being proposed.
Whether any given administrative edit corrects the letter of some rule without
changing its spirit is left to voters and judges to decide.
An administrative edit does not cause a rule's number to be updated.

Examples of administrative edits include but are not limited to:
- Changing other rules to update how they refer to a rule whose number or name
  has changed, or which has been revoked.
- Removing language from rules which is no longer consistent or applicable due
  to its being overridden by precendence rules.

Administrative pull requests (item 8 above) may be merged outside of the normal
turn order, must be approved by the same mechanism as rule change proposals,
and cannot materially affect the operation of the rules or the game.
An example of an administrative pull request include but are not limited to:
- editing, removing, or replacing the LICENSE or README files
- cleaning up damage from an incorrect merge

Rule changes are proposed only by the creation of a Pull Request.
Players vote on proposals only by commenting on its Pull Request, and including
in their comment either :+1: (for an affirmative vote) or :-1: (for a negative
vote).  Any comment that does not contain one of these emoji is not a valid
vote.
Only the most recent such vote is valid, unless explicitly stated otherwise by
the voter.
