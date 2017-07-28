# Temporal Initiated Motion Every Rule

To ensure the progression of rule acceptance, and allow for rule acceptance to fail and advance to the next turn, the process of rule acceptance (the "turn") is metered by certain time periods.

## Definitions

Herein, language within parenthesis is given for clarification and exposition, but it is not part of the rule; the behavior described within parentheses is assumed to be goverened by other rules, which may or may not remain in play.

The _age_ of a proposal is the lesser of:

- the time since the proposal was proposed (the time since its PR was opened), or
- the time since the proposal was changed (the time since the most recent commit was pushed to the PR).

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

Only one proposal may be accepted per turn. Others remain in play.

## Determining acceptability

A proposal is acceptable under any of the following three criteria:

1. _All players have voted_ and a majority of them have voted in favor.

    - Any player may accept (merge) such a proposal, if it has been selected, during its proponent's turn.

2. A majority _of the players who voted so far_ did so in favor, and the proposal is _older than 48 hours_.

    - Any player may accept (merge) such a proposal, if it has been selected, during its proponent's turn.
    - Players who have not declared their vote give an implicit vote of "abstain".
    - For the purpose of calculating reward given in _Parts of a turn_: "the fraction of favorable votes" is the number of favorable votes over the number of voting players. (I.e. implicit abstain votes are _not_ included in the denominator.)

Otherwise, a proposal is unacceptable.

## During a player's turn

The player may select one of their possibly multiple acceptable proposals to be accepted (PR merged). If they do not make a choice, their earliest proposal (their lowest-numbered PR) is selected by default.

Once a proposal is accepted their turn ends and the next player's begins.

(New proposals may be made, and unacceptable proposals may become acceptable, at any time, including during the course of a player's turn.)

When a player's turn ends, the next player's turn begins immediately.

If no proposals are accepted, then (for the purpose of interpreting _Defeated proposals_,) "their proposed rule-change is defeated." (This means that the player suffers a 10 point penalty for the turn. Not 10 points penalty per active proposal, nor point loss for withdrawing a proposal, nor a penalty-free turn simply because unacceptable proposals remain in play.)

## Retroactive turn resolution

If a player's turn has exceeded 48 hours, any player may resolve that turn, by accepting (merging) the selected proposal, if any. The player's turn should be considered to have ended exactly 48 hours after it was begun, though proposals accepted in this manner do not retroactively apply.

(In the case of several unresponsive players, this enables any motivated player to ratchet gameplay forward to their own turn, which may itself have passed the 48 hour limit, without skipping the acceptance of any pending accepted proposals, and take their turn actions immediately.)
