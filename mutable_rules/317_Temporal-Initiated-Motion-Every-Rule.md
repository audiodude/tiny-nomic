# Temporal Initiated Motion Every Rule

To ensure the progression of rule acceptance, and allow for rule acceptance to fail and advance to the next turn, the process of rule acceptance (the "turn") is metered by certain time periods.

## Definitions

Herein, language within parenthesis is given for clarification and exposition, but it is not part of the rule; the behavior described within parentheses is assumed to be governed by other rules, which may or may not remain in play.

Herein, the meaning of **proposal** is limited to proposed changes which enact, amend, rescind, or transmute rules. (So this rule does not govern PRs for e.g. "administrative tasks" mentioned in _Github repository_.)

The **age** of a proposal is the lesser of:

- the time since the proposal was proposed (the time since its PR was opened), or
- the time since the proposal was changed (the time since the most recent commit was pushed to the PR).

An **acceptable** proposal is one which meets the acceptability criteria, defined below.

A proposal is **accepted** when it becomes part of the game rules. (When it is merged.)

The **first acceptable proposal** is the earliest proposed (lowest PR number) of the current player's acceptable proposals. (The state of being the _first acceptable proposal_, like the state of being _acceptable_, may change at any time.)

## Rules

Votes on proposals are _continuously tallied_; proposals whose votes cause them to become _acceptable_ may be merged during their proponent's turn, while those that have not reached this state remain open for discussion and improvement.

Players may prepare proposals at any time. (By opening a PR on GitHub.)

Players may discuss proposals at any time. (By commenting on the PR.)

Players may vote on proposals at any time. (By commenting with a :+1: or :-1: on the PR.)

Players may change their vote at any time. (By modifying their comment, or adding a new comment with an updated vote.)

A player may have any number of proposals in play at once.

Players may modify their proposals at any time. (By pushing commits to an open PR)

Modified proposals invalidate any earlier votes on the same proposal, unless declared otherwise by the voter.

Players may withdraw any of their own proposals at any time. (By closing the PR unmerged.)

Only one proposal may be _accepted_ (merged) per turn. (Others remain in play.)

Only _acceptable_ proposals may be accepted.

This rule takes precedence over any conflicting language in _Facilitating Accerlerated Submission Timelines_.

## Determining acceptability

A proposal is _acceptable_ under any of the following three criteria:

1. _All players have voted_ and a majority of them have voted in favor.

2. A majority _of the players who voted so far_ did so in favor, and the proposal is _older than 48 hours_.

    - Players who have not declared their vote give an implicit vote of "abstain".
    - For the purpose of calculating reward given in _Parts of a turn_: "the fraction of favorable votes" is the number of favorable votes over the number of voting players. (I.e. implicit abstain votes are _not_ included in the denominator.)

Otherwise, a proposal is unacceptable.

## During a turn

Herein, _The Player_ refers to the player of the turn.

The Player's _first acceptable proposal_ (see definitions) is accepted (merged).

Any player may accept (merge) The Player's first acceptable proposal.

When a proposal is accepted (merged), the turn ends.

When the turn ends, the next turn begins immediately.

(New proposals may be made, and unacceptable proposals may become acceptable, at any time, including during the course of a turn.)

If no proposals are acceptable after 48 hours (including if none become acceptable), then (for the purpose of interpreting _Defeated proposals_,) "their proposed rule-change is defeated." (This means that The Player suffers a 10 point penalty for the turn. Not 10 points penalty per active proposal, nor point loss for withdrawing a proposal, nor a penalty-free turn simply because unacceptable proposals remain in play.)

## Retroactive turn resolution

If a turn has exceeded 48 hours, any player may resolve that turn, by accepting (merging) the first acceptable proposal as described above, if it exists. The turn should be considered to have ended exactly 48 hours after it was begun, though proposals accepted in this manner do not retroactively apply.

(The next player's turn begins at that point, but if sufficient time has passed, may already be in the same greater-than-48-hours state, and this process may be repeated.)

(In the case of several unresponsive players, this enables any motivated player to ratchet gameplay forward to their own turn, which may itself have passed the 48 hour limit, without skipping the acceptance of any pending accepted proposals, and take their turn actions immediately.)
