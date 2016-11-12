# Nash Equilibrium

## 2.1 - Strategic Games
- Every player simultaniously choses their sole plan of action.
- N = players; i = player; A_i = set of actions with preferences (action, preference);  
- Players have to have actions (can't have random unneeded players)
- The preference function of each action **is dependent on the other player's actions**
  - ie. if I choose rock, I will have 1 preference defined for if you choose paper vs if you choose scissor.
  - Different from a "decision problem" because you care about what the other players choose.

 This model is most useful when we define a set of consequences that are accociated with action profiles
 [are action profiles the same as strategies?]
 We can add random chance
 - Ω = a set of probabilities applied to consequences
 - A × Ω → C (aka the preference of your action = the chance that it will happen * it's awesomeness)
   - In other words, if you have an action which gives you a 10% chance to win a million dollars, it's 10x worse than having an action that gives you a 100% chance to win a million dollars. You multiply the optimality of the outcome by the chance it will happen.

     
<img width="165" alt="screen shot 2016-11-12 at 2 37 19 pm" src="https://cloud.githubusercontent.com/assets/706123/20240412/911bbc70-a8e5-11e6-9e50-65fc5a6131ee.png">

- in this picture, w_1, w_2 are the payoffs of players 1 and 2 respectively when the players pick those outcomes
- Players are often assumed to act rationally
- Players only have the model to work off of when picking their actions
- In this book players are assumed to have played the game in the past
- The actions of previous games cannot effect the actions of the current game   

## 2.2 - Nash Equilibrium
- Steady state of of a strategic game
- The set of actions in which each player is choosing their optimal strategy

[Wikipedia's](https://en.wikipedia.org/wiki/Nash_equilibrium) definition:
> ...the Nash equilibrium is a solution concept of a non-cooperative game involving two or more players in which each player is assumed to know the equilibrium strategies of the other players, and no player has anything to gain by changing only his or her own strategy. If each player has chosen a strategy and no player can benefit by changing strategies while the other players keep theirs unchanged, then the current set of strategy choices and the corresponding payoffs constitutes a Nash equilibrium. ...

> Stated simply, Amy and Phil are in Nash equilibrium if Amy is making the best decision she can, taking into account Phil's decision while Phil's decision remains unchanged, and Phil is making the best decision he can, taking into account Amy's decision while Amy's decision remains unchanged. Likewise, a group of players are in Nash equilibrium if each one is making the best decision possible, taking into account the decisions of the others in the game as long as the other party's decision remains unchanged.

## 2.3 - Examples

### Example 15.3 - Bach or Stravinsky? (BoS) (aka “Battle of the Sexes”--not PC)
<img width="281" alt="screen shot 2016-11-12 at 3 07 51 pm" src="https://cloud.githubusercontent.com/assets/706123/20240577/d3945ac2-a8e9-11e6-910d-5cbd27199574.png">
- 2 people want to want to go out together, but each prefer different activities (aka Bach concert or Stravinsky)
- Two Nash Equalibrium, (Bach, Bach) or (Stravinsky, Stravinsky)

### Example 16.1 - A coordination game
<img width="216" alt="screen shot 2016-11-12 at 3 09 31 pm" src="https://cloud.githubusercontent.com/assets/706123/20240584/0bbdc4ec-a8ea-11e6-8847-0724dec1cdcc.png">
- Two people want to go out together, but both find one activity better than the other
- Another example (I think) is 2 cars arriving at an intersection with the choice to either stop or go
- There are **two** Nash Equlibrium here! Woah
  - That's because once both players have chosen the less optimal action (ie Mahler), there is no incentive to individually change their choice. That's because if they did they would recieve a zero payoff
  - Once you hit a nash equlibrium, you are stuck there even if it is sub-optimal (a local maxima) -- scary!

### Example 16.2 - The Prisoner’s Dilemma
<img width="362" alt="screen shot 2016-11-12 at 3 19 37 pm" src="https://cloud.githubusercontent.com/assets/706123/20240642/7611fa42-a8eb-11e6-81ae-c87708141513.png">
- (1,1) is actually the Nash Equlibrium. To understand this, follow these steps
  - Assume player B chooses "Don't Confess", what would your optimal choice be? Don't confess would give you **3** and confess would give you **4**, so you should confess.
  - Assume player B chooses "Confess", what would your optimal choice be? Don't confess would give you **0** and confess would give you **1**, so you should confess.

### Example 16.3 - Hawk-Dove
<img width="188" alt="screen shot 2016-11-12 at 3 30 25 pm" src="https://cloud.githubusercontent.com/assets/706123/20240697/f46ead4e-a8ec-11e6-9437-ebd1cdc53dac.png">
- Two nash equilibrium, (Dove, Hawk) & (Hawk, Dove)

### Example 17.1 - Matching Pennies
<img width="198" alt="screen shot 2016-11-12 at 3 34 14 pm" src="https://cloud.githubusercontent.com/assets/706123/20240722/7fe218f2-a8ed-11e6-8af8-5844f4b06de2.png">
- There is no nash equlibrium!
- You can see this because if player1 chooses H then player2 will choose T, but if player2 chooses T then player1 would instead choose T which begins this cycle of changing choices.
- This is called “strictly competitive”

---
#### So far those are simple games, next are some complex ones:

### Example 18.1 - an auction
- An action where everyone simultaneously submit their bids

### Exercise 18.2
**First price auction:** If there is a tie in the bid, the player with the lowest index wins

- Prove: In a first price auction, in nash equlibrium player with the lowest index always wins.
- Explanation: https://www.youtube.com/watch?v=MROR272191E
- #thatishard

### Exercise 18.3
**Second price auction:** The payment made is the bid that the 2nd highest bidder placed

- Prove: in a second price auction the bid v_i of any player i is a weakly dominant action: player i’s payoff when he bids v_i is at least as high as his payoff when he submits any other bid, regardless of the actions of the other players. Show that nevertheless there are (“inefficient”) equilibria in which the winner is not player 1.
- Explanation: https://www.youtube.com/watch?v=5YzVBaNEIz0
- #lesshard video but the solution is a bit difficult

### Example 18.4 - War of Attrition
Two players have a dispute over an object. The war is over who will give up the object (admit defeat) first. If it happens at the same time, they split the winnings. As time goes on the payout is reduced.

- Explaination: https://www.youtube.com/watch?v=hSYXkDnCpHM

### Example 18.6 - a location game

- Explaination: https://youtu.be/pglQ_E0g8PY?t=14m34s

### Exercise 19.1

