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
Draws 1 card for the dealer player.

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
> Use this macro **after** collecting the Double Down bet.

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
Used to modify the player's bet to x2 the value.

> [!NOTE] 
> You can change `/dice party 13` to `/dice cwl7 13` when you are practicing. You need to have a Cross World Linkshell on #7 for this to work.
```
                         ≫≫    ≪≪
 <t> stands.
```
