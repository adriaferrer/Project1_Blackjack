Project1_Blackjack
## Blakcjack rules (from www.bicyclecards.com):

### OBJECT OF THE GAME
Each participant attempts to beat the dealer by getting a count as close to 21 as possible, without going over 21.

### CARD VALUES/SCORING
It is up to each individual player if an ace is worth 1 or 11. Face cards are 10 and any other card is its pip value.

### BETTING
Before the deal begins, each player places a bet, in chips, in front of him in the designated area. Minimum and maximum limits are established on the betting, and the general limits are from 2 to 500.

### THE SHUFFLE AND CUT
The dealer thoroughly shuffles portions of the pack until all the cards have been mixed and combined. He designates one of the players to cut, and the plastic insert card is placed so that the last 60 to 75 cards or so will not be used. (Not dealing to the bottom of all the cards makes it more difficult for professional card counters to operate effectively.)

### THE DEAL
When all the players have placed their bets, the dealer gives one card face up to each player in rotation clockwise, and then one card face up to himself. Another round of cards is then dealt face up to each player, but the dealer takes his second card face down. Thus, each player except the dealer receives two cards face up, and the dealer receives one card face up and one card face down. (In some games, played with only one deck, the players' cards are dealt face down and they get to hold them. Today, however, virtually all Blackjack games feature the players' cards dealt face up on the condition that no player may touch any cards.)

### THE PLAY
The player to the left goes first and must decide whether to "stand" (not ask for another card) or "hit" (ask for another card in an attempt to get closer to a count of 21, or even hit 21 exactly). Thus, a player may stand on the two cards originally dealt him, or he may ask the dealer for additional cards, one at a time, until he either decides to stand on the total (if it is 21 or under), or goes "bust" (if it is over 21). In the latter case, the player loses and the dealer collects the bet wagered. The dealer then turns to the next player to his left and serves him in the same manner.

The combination of an ace with a card other than a ten-card is known as a "soft hand," because the player can count the ace as a 1 or 11, and either draw cards or not. For example with a "soft 17" (an ace and a 6), the total is 7 or 17. While a count of 17 is a good hand, the player may wish to draw for a higher total. If the draw creates a bust hand by counting the ace as an 11, the player simply counts the ace as a 1 and continues playing by standing or "hitting" (asking the dealer for additional cards, one at a time).

### THE DEALER'S PLAY
When the dealer has served every player, his face-down card is turned up. If the total is 17 or more, he must stand. If the total is 16 or under, he must take a card. He must continue to take cards until the total is 17 or more, at which point the dealer must stand. If the dealer has an ace, and counting it as 11 would bring his total to 17 or more (but not over 21), he must count the ace as 11 and stand. The dealer's decisions, then, are automatic on all plays, whereas the player always has the option of taking one or more cards.

### SETTLEMENT
A bet once paid and collected is never returned. Thus, one key advantage to the dealer is that the player goes first. If the player goes bust, he has already lost his wager, even if the dealer goes bust as well. If the dealer goes over 21, he pays each player who has stood the amount of that player's bet. If the dealer stands at 21 or less, he pays the bet of any player having a higher total (not exceeding 21) and collects the bet of any player having a lower total. If there is a stand-off (a player having the same total as the dealer), no chips are paid out or collected.

### RESHUFFLING
When each player's bet is settled, the dealer gathers in that player's cards and places them face up at the side against a clear plastic L-shaped shield. The dealer continues to deal from the shoe until he comes to the plastic insert card, which indicates that it is time to reshuffle. Once that round of play is over, the dealer shuffles all the cards, prepares them for the cut, places the cards in the shoe, and the game continues.

## Bonus 1
### SPLITTING PAIRS
If a player's first two cards are of the same denomination, such as two jacks or two sixes, he may choose to treat them as two separate hands when his turn comes around. The amount of his original bet then goes on one of the cards, and an equal amount must be placed as a bet on the other card. The player first plays the hand to his left by standing or hitting one or more times; only then is the hand to the right played. The two hands are thus treated separately, and the dealer settles with each on its own merits. With a pair of aces, the player is given one card for each ace and may not draw again. Also, if a ten-card is dealt to one of these aces, the payoff is equal to the bet (not one and one-half to one, as with a blackjack at any other time).

## Bonus 2
### DOUBLING DOWN
Another option open to the player is doubling his bet when the original two cards dealt total 9, 10, or 11. When the player's turn comes, he places a bet equal to the original bet, and the dealer gives him just one card, which is placed face down and is not turned up until the bets are settled at the end of the hand. With two fives, the player may split a pair, double down, or just play the hand in the regular way. Note that the dealer does not have the option of splitting or doubling down.

## Bonus 3
### INSURANCE
When the dealer's face-up card is an ace, any of the players may make a side bet of up to half the original bet that the dealer's face-down card is a ten-card, and thus a blackjack for the house. Once all such side bets are placed, the dealer looks at his hole card. If it is a ten-card, it is turned up, and those players who have made the insurance bet win and are paid double the amount of their half-bet - a 2 to 1 payoff. When a blackjack occurs for the dealer, of course, the hand is over, and the players' main bets are collected - unless a player also has blackjack, in which case it is a stand-off. Insurance is invariably not a good proposition for the player, unless he is quite sure that there are an unusually high number of ten-cards still left undealt.

# Approach
1 player and 1 dealer
only 1 deck of cards (not like in casinos)
The shuffle will be considered as a random pick (i.e. no cut).
The player has a certain amount of money, that is used to bet, from 5 to 200.
Actions of each play:

0) Player decides how much money is he providing to the table (initialize pot)

1) Player places a bet (minimum 5, max 200)

2) The dealer deals to the player and and to himself but 1 card face-up and 1 face down. We assume that both cards of the player are face up and 1 of the dealer's is not visible for the player.

3) The player can "stand" or "hit" --> Action from the player is required here.

4) In case the action is "hit" another card is dealt to the palyer

5) Repeat step 3) until the player stands or is busted. Busted = the sum of his hand is greater than 21. In case the player has an "A", it can count as 11 but if this is causing the player to be busted, the "A" will count 1. The total count can be provided to the player for guidance (but is not required)

6) In the case the player is busted, the dealer is automatically the winner.

7) In case the player is not busted, the dealer uncovers his second card checks if the sum of his hand is equal or greater than 17. If it is not the case he has to deal himself until his hand (the sum) is 17 or higher. The dealer can also get "busted" if the sum of his hand is greater than 21.

8) In the case that neither the player nor the dealer are busted, the two sums are compared and the higher wins. In the case that any of the hands is A + ten-value-card, this beats a regular sum of 21.

9) If the player wins, he doubles his bet (so his pot = pot + bet). In case the dealer wins, the player loses his bet (pot = pot - bet). In case of tie, pot = pot.

10) The deck is reshuffled and we start again at step 1) until the player wants to quit or his pot is empty

# Approach to Bonus 1
Using the same flow as before, in the step 3), in case the player has two equal cards, he can decide to split, therefore having 2 hands instead of 1. He also needs to provide the same bet as the original one for the second hand. Each hands will be settled separately against the dealer's hand. 

# Approach to Bonus 2
Again, reusing the whole code but now, the first time we come into step 3. In case the sum of the hand is 9, 10 or 11, the player can double the bet and receive just 1 card until settlement. 

# Approach to Bonus 3
In case the dealer's hand is an Ace, the player can place a side_bet =< bet/2. In case the dealer gets a blackjack in the settlement, the player pot is pot = pot + side_bet.