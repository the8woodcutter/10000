## Dice Game of 10,000 played with 6 dice
### XMPP (slixmpp / python) Bot for MUC chats
#### Author: The8Woodcutter // Licence: GPL

### This game is yet to begin being coded.
- The author of this is amidst a very long time, periodical, study and learning of python and has not begun this small project yet.
  - SliXMPP is the python library we use for this bot
  - Game of 10,000:
    - Need to get a complete x6 d6 dice to get on the board (x so many points to get onto the board)
    - A list is kept for score
    - Various poker hands, in the representation of dice (like Yahtzee), are granted set points for all
    - Turn after turn until a high enough score of points is reached
    - Game is considerably more entertaining if once in a while use a couple or 3 extra dice and make the scores larger to obtain

**Please Note**: I may not currently remember this game entirely correctly

### Order of flow for bot:
- Bot requires a flow:
    - A command with an invite like `mrBot 10,000 challenge kou`
      - `mrBot` is nickname for bot
      - `10,000` is obviously name of game
      - `challenge` is even more obvious
      - `kou` is another MUC participant
    - Challenger is already initiated, so recipient of challenge (`kou` in this case):
      - has `x time` to call the challenge, or cancel
    - Upon accepted challenge:
      - Challenger rolls first
      - Bot calls nicknames of who's turn it is while rendering the ASCII character dice
      - For each hand to keep a dice the human player selects from a common list index: `[0,1,2,3,4,5]`
        - calling it like `2,3,5,6`
    - Game score sheet is printed everytime points are put on it
    - Bot computes the best collection of dice for a 'hand' or a 'roll' and automatically decides once your hand is complete
      - _**please send an issue about it if you have a better idea, thanks**_

#### That's all I'm writing, oh look a squirrel!!
