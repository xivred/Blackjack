# Macros for Blackjack Plugin

Please make sure to copy and paste the macros to your game's Shared Macros tab.

# **Player Bust**  
Used when a player cards reach over 21. 

> [!IMPORTANT]
> This macro is required on shared macro slot `#51`, you can change it on the plugin settings.

> [!NOTE]
> You can change `/broom` for other emote if you like.
```
                             ≫≫    ≪≪
 Woops! <t>, that's a bust. <se.11><br />
/broom
```

# **Player Natural Blackjack**  
Used when a player hits Natural Blackjack (first hand) with 10/11/12/13 + 1 (Ace). Does not apply to Split hands.

> [!IMPORTANT]
> This macro is required on shared macro slot `#52`, you can change it on the plugin settings.

```
                          ≫≫  .    ≪≪
 Congratulations!  <t>, that's a Natural Blackjack. <se.12><wait.1>
/congratulate
```

# **Dealer Wins**  
Used when there are no winners.

> [!IMPORTANT]
> This macro is required on shared macro slot `#61`, you can change it on the plugin settings.

```
                             ≫≫    ≪≪
 GG everyone, Dealer wins. ♥ <se.3>
/bow
```

# **Dealer Bust**  
Used when the dealer cards reach over 21.

> [!IMPORTANT]
> This macro is required on shared macro slot `#62`, you can change it on the plugin settings.

> [!NOTE]
> You can modify this macro as long as you have the keyword `dealer bust`, so the Plugin identifies the end of the game.
```
                             ≫≫    ≪≪
 Woops! That's a Dealer Bust. <se.11>
/stagger
```

# **Collecting Bets**  
Used when the bet collection begins.

```
      ≫≫     ≪≪
           Please wait for me to trade you.
/bstance
```

# **Bets Placed**  
Allows the players know the bet collection process has ended and the game is about to begin.

```
        ≫≫     ≪≪
                           All bets placed.
/bstance
```


# **Dealer Hit**  
Draws 1 card for the dealer.

> [!NOTE]
> You can change `/dice party 13` to `/dice cwl7 13` when you are practicing. You need to have a Cross World Linkshell on #7 for this to work.  
> You can modify this macro as long as you have the keyword `dealer hits`, so the Plugin identifies the next card will be added to the Dealer.
```
/vpose
           ≫≫     ≪≪
                           Dealer hits...<wait.2>
/dice party 13
```


# **Player First Hand**  
Draws 2 cards for the targetted player, used during first hand only.

> [!NOTE]
> You can change `/dice party 13` to `/dice cwl7 13` when you are practicing. You need to have a Cross World Linkshell on #7 for this to work.
```
/bstance
                 ≫≫        ≪≪
 Drawing  for  <t> <se.8><wait.2>
/dice party 13
/dice party 13
```

# **Player Hit**  
Draws 1 card for the targetted player.

> [!NOTE]
> You can change `/dice party 13` to `/dice cwl7 13` when you are practicing. You need to have a Cross World Linkshell on #7 for this to work.
```
/bstance
                             ≫≫     ≪≪
 Hitting  <t> with... <se.8><wait.2>
/dice party 13
```


# **Player Double Down Announcement**  
Used to modify the player's bet to x2 the value and enter Double Down processes.

> [!Warning]
> Use this macro **after** collecting the Double Down bet (equal to the initial bet).

> [!NOTE] 
> You can modify this macro as long as you have the keyword `chooses double down`, this will increase the targetted player's bet to x2 the value, after the next card draw the player will be forced to stand.
>  
> Optional: You can also add a macro previous to this, so the player knows they have to pay the bet first, and then make your own macro with the `chooses double down` keyword to trigger it.
```
              ≫≫       ≪≪
 Here we go!  <t> chooses double down. Your bet will be collected, a card will be drawn and you will be forced to stand.
```


# **Player Double Down Draw Card**  
Provides the player with their Double Down card, you can use [Player Hit](#player-hit) if you like instead.

> [!NOTE] 
> You can change `/dice party 13` to `/dice cwl7 13` when you are practicing. You need to have a Cross World Linkshell on #7 for this to work.
```
              ≫≫       ≪≪
 Here's your card   <t>... <se.8> <wait.3>
/dice party 13
```



# **Player Stands**  
Used to set a player on the stand status.

> [!NOTE] 
> You can modify this macro as long as you have the keyword `stands`, so the Plugin identifies that the targetted player is standing.
```
                         ≫≫    ≪≪
 <t> stands.
```


# **Player Split Announcement**  
Used to split the targetted player hand into 2 separate hands.

> [!Warning]
> Use this macro **after** collecting the Splitting bet (equal to the initial bet). 

> [!NOTE] 
> You can modify this macro as long as you have the keyword `chooses to split`.
>  
> Optional: You can also add a macro previous to this, so the player knows they have to pay the bet first, and then make your own macro with the `chooses to split` keyword to trigger it.
```
                         ≫≫    ≪≪
 Here we go!  <t> chooses to split the hand.
Your bet will be collected and each card will be treated as a separate hand. I will hit both hands once, then continue with each one individually. <se.8>
```


# **Player Split Hit Hand 1**  
Draws 1 card for the targetted player, mentioning it's for Hand 1 of the split.

> [!NOTE]
> You can change `/dice party 13` to `/dice cwl7 13` when you are practicing. You need to have a Cross World Linkshell on #7 for this to work.
>
> Optional: You can use regular [Player Hit](#player-hit) instead to save on some macro space.
```
                 ≫≫        ≪≪
 Hitting  <t> with... <se.8><wait.2>
/dice party 13
```

# **Player Split Hit Hand 2**  
Draws 1 card for the targetted player, mentioning it's for Hand 2 of the split.

> [!NOTE]
> You can change `/dice party 13` to `/dice cwl7 13` when you are practicing. You need to have a Cross World Linkshell on #7 for this to work.
>
> Optional: You can use regular [Player Hit](#player-hit) instead to save on some macro space.
```
                 ≫≫        ≪≪
 Hitting  <t> with... <se.8><wait.2>
/dice party 13
```



# **Dealer Stands**  
Used to end the game when the Dealer hits Hard 17 or higher.

> [!Warning]
> This will end the current game, make sure everyone on the table is on standing position before you trigger it, else the game will think they can still do their move.
>
> The Plugin will copy to your clipboard different messages depending on the Dealer's cards, if it's on Hard 17 or higher, the plugin will automatically include this trigger on the copied message. You can use this macro when for example, you're on Soft 19 and you chose to stand.

> [!NOTE] 
> You can modify this macro as long as you have the keyword `dealer stands`.

```
                         ≫≫    ≪≪
 Dealer stands.
```



# **Rules**  
A macro that shows the rules of the game.

> [!NOTE] 
> This macro is optional, you can modify it to your liking, some of these rules follow the Plugin's configuration.
>
> You can modify the x2.5 Natural Blackjack multiplier in the Plugin Settings using `/rbjc`

```
_______________________________________________
                             ≫≫   ≪≪
.
 The dealer will be forced to hit on 16 or less, and stand on Hard 17 or higher, if the dealer is on a Soft 17+ (17/7), the dealer is free to hit on 7 but not on 17.
 Same numbers can be split into 2 hands (during first hand), same bet is required for 2nd hand. This applies only if you get for example 12+12 not on 12+13 cards.
 You can Double Down once your hand has been drawn (first hand).
 Natural Blackjack (1 + 10) wins x2.5 only on first hand, does not apply on Splits.
 Natural Blackjack (1 + 10) vs Dealer Natural Blackjack (1 + 10) will push the Player's Bet.
 1 or "ACE" has a value of 1 or 11, 10-13 have a value of 10.
 Pushing will move your bet to the next round unless you want to leave the table.
 When you Double Down and your hand is pushed, your Double Down is lost, only the initial bet will be pushed.
```

