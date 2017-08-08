# Github repository

## Repository organization

Each rule shall be represented by a file in either the `immutable_rules/` or
`mutable_rules/` directory of the git repository where the game is being
recorded. No other files in the repository shall be constituted to represent a
rule or have the force of a rule. To be explicit: all mutable rules must be in
the `mutable_rules/` directory and all immutable rules the `immutable_rules/`
directory.

The master branch of the repository will serve as a representation of the
current game state. No commits are allowed to be made to the master branch
except through the mechanism of a Github Pull Request.

## Pull requests

Pull Requests must perform exactly one of the following actions:

1. Add a file to one of the rules directory, when a rule is enacted.
2. Remove a file from one of the rules directories when a rule is repealed.
3. Modify an existing rule file, when an amendment is made, or repealed, or when
   an amendment to an amendment is made or repealed.
4. Move a rule from either the `immutable_rules/` directory or the
   `mutable_rules/` directory to the other one, when a rule is transmuted.
5. Create a new player file in the `players/` directory
6. Update a player's score file, the mechanism of which may be provided by any
   other rule(s), following the active precedence procedure.
7. Perform some administrative task on the repository, at the discretion of the
   players. Pull Requests of this type can happen outside of the normal turn
   order, must be approved by majority vote of all players, and cannot
   materially affect the operation of the rules or the game. An example of this
   would be removing or replacing the LICENSE or README files.
8. Some other action, except that the action must be outlined in a current,
   valid rule other than this one.

## Associated modifications for rule coherency

When a rule change is proposed (items 1--4 above), in addition to the "exactly
one" action specified, a pull request may also perform certain modifications to
any number of other files, including rules files, to make them coherent with
the proposed rule.

Modifications for coherency may adjust a rule's filename, title, references to
other rules, and modify language to avoid contradiction, in service of the
proposed rule. No modification which changes the behavior of the game beyond
that specified by the propsed rule is valid.

Modifications for coherency are neither considered "amendments" to the
modified rules nor do they cause a rule's number to be updated.

## Proposing and voting

The proper way to propose a rule-change is a Pull Request. Players vote on Pull
Requests/proposals by putting either :+1: (for an affirmative vote) or :-1:
(for a negative vote) as whole or part of a comment on the Pull Request. Any
comment that does not contain one of these emoji is not considered a proper
vote.
