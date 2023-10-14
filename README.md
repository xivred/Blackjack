# Blackjack Plugin

Add the following repo to your Dalamud Settings: `https://raw.githubusercontent.com/xivred/Blackjack/main/repo.json`

# How to use Red's Blackjack Plugin

**Before you start:**
This plugin requires a valid License Key, which can be obtained by following the instructions on http://www.patreon.com/redxiv, without a valid key, you won't be able to use it.

1. Install `Macro Chain` plugin, which is available on Dalamud by Default. This will allow you to trigger macros through chat, the plugin will copy some of the macros to your clipboard so you just need to paste it on chat.
2. Add all the macros I have sent you to **SHARED MACROS**, paying special attention to the number some of those macros require:
**#50** = Player Bust.
**#51** = Player got a natural blackjack.
**#61** = Dealer Wins (table sweep).
**#62** = Dealer Bust.

3. You can use party chat to play as well as CWL7 to practice, you will need to update the macros that use `/dice party 13` to `/dice cwl7 13` to do so. I have a Blackjack CWLS for this purpose, let me know if you want to join it, make sure to change it's number to #7.


**Commands:**
- Type `/rbjc` to open the plugin configuration window.
- Type `/rbj` to open the game window.

**To add a player to the table:**
1. Target the player
2. Type `/e bets <amount>` for example `/e bets 500k` or `/e bets 1m` when adding 1.5m and any amount like that, please use `/e bets 1500k` as the dot will split the amount into 2 strings and will only add the player with 1m

**To change a player's bet:**
1. Target the player
2. Type `/e change bet <amount>`

**To remove a player from the table:**
1. Make sure the game has ended (you have stood).
2. Target the player.
3. Type `/e delete player`

--------------------

# How to use the plugin:
It works through keywords and targeting players, you must play one player at a time to have a smooth experience as the plugin copies strings to your clipboard, it's also friendly for new people coming into the games.

The game will not end until **the dealer Stands**. The table will automatically add up all the cards you draw, and will copy strings into your clipboard so you can just paste whatever the plugin copies.

Once the game ends, a "Play again?" button will appear, if you click this the table will restart and the bets will be returned to the initial bets (if there was a DD it will go back to the regular bet, if there's a split it will remove any additional hands).

**First:**
1. The dealer collects bets and adds players to the table, this is where you can modify the bet amounts if they change their bet.
2. Once you have collected bets, you can run your "dealer hit" macro, you will get the card added to your hand, and a message will be copied to your clipboard, all you need to do is PASTE on chat. "Dealer's first card is X".

**Second:**
1. Use your party list to target players, makes your life easier and gives you the order of the game. So target the player and HIT the player with 2 cards, one of the macros should be able to draw 2 `/dice 13`.
2. A message will be copied to your clipboard depending on the result, if it's a Natural Blackjack you will have to wait 2 seconds after the card draw to give the Macro plugin time to end the previous macro. This applies every time a `/runmacro` command is copied to your clipboard. An echo message will let you know what is being copied.

**Third:**
If you're doing a double down or split, collect the bet first, then run the corresponding macro.

**If it's a split:**
1. Collect the bet before, or run a pre-split macro (without mentioning the string that splits it, check below for more info).
2. Run the split macro to split the hand into 2 separate ones.
3. Hit the player TWICE (there's macros for Hand 1 and Hand 2, but regular hit works)
4. Once done, paste the result.
5. You will automatically be hitting hand 1 after this, and will pass onto hand 2 if you stand the player or if the player bust on hand 1.
6. Make sure to paste the result the plugin gives you, but READ it first, as it's not 100% bug free.

**If it's a double down:**
1. Collect the bet before, or run a pre-DD macro (without mentioning the string that duplicates the bet, check below for more info).
2. Run the DD macro to duplicate the bet.
3. Hit the player once.
4. The player will be stood automatically after you draw their card.
5. Paste the result.

**Fourth:**
Every time you end someone's turn, STAND THEM. It is needed for the plugin to know they're not still playing the game, if you don't see RED (bust) or YELLOW [STAND] (it actually says STAND on the plugin), then you need to go back and stand them.

**Fifth:**
Once you have given everyone their cards, run your "dealer hits" macro, until you hit HARD 17+. If you're on a soft 17+ (17/7) the plugin will allow you to continue hitting on the HARD number. It's up to you to stand or not when you're on or over Soft 17. If you keep on hitting and you have a Soft 18 for example, and get a "1" (Ace), your result is 9, not 19, you must NOT use the Soft result to win the game if you have chosen to hit on soft 17+ numbers.

The game ends once you BUST or STAND.

**When the game ends:**
Once the game is over you can paste your result into chat. AFTER YOU DO THAT, PASTE AGAIN to paste the win/lose/push result, the plugin does not let you know this has been copied after you send your result information, just paste again and it will be there.

The plugin will enable a "PLAY AGAIN?" button, this will reset the table bets and cards WITHOUT DELETING PLAYERS (only extra hands from splits and resets DD's amounts).

**Before you start the next round:**
Make sure to pay attention to who has pushed, and collect bets from people.
