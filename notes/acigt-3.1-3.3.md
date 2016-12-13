### 3.1
Instead of going through the book which for this section at least seems super complex, I'm using https://www.youtube.com/watch?v=FU6ax5K9HIA

- Strategy: strategy s_i is for player i, any probability distribution over actions A_i
- Pure strategy: Only one action is chosen with positive probability
- Mixed strategy: Players introduce an element of randomness to their strategy, they can choose multiple actions and give them postiive probability
- Support of mixed strategy: set of actions which are played with *postive* probability
- Set of all strategies for i be S_i
- Set of all **strategy profiles** be S = S_1 x ... x S_n

- Because we changed the definition of strategies to include an infinite set of probability distributions, we have to change our utility functions
to instead represent *expected utility* as opposed to the percice utility.
- New utility definition:

<img width="257" alt="screen shot 2016-12-13 at 5 16 21 pm" src="https://cloud.githubusercontent.com/assets/706123/21161762/f8898024-c157-11e6-80e1-9f238b4e47e7.png">

- **ENGLISH EXPLANATION:** This new utility represents the sum of all of action profiles, considering each action profiles' utility multiplied
by the probability that that action profile will be reached given a particular mixed strategy profile. The 2nd equation defines
the probability of a particular action profile given a strategy profile as the product of each player playing that action profile.
- We can now reevaluate our definition of best response and nash equilibrium:

<img width="641" alt="screen shot 2016-12-13 at 5 24 33 pm" src="https://cloud.githubusercontent.com/assets/706123/21161996/1cfeacee-c159-11e6-94e8-3b42b4bdb060.png">

- Best response in English: `s*_i` is a member of the set of best responses if and only if: for all `s_i` contained in `S_i`, the utility
of playing `s*_i` while everyone else plays `s_-i` is at least as good as the utility of playing `s_i` while everyone else plays `s_-i`
- Nash Equlibrium in English: Strategy `s` is a Nash equilibrium if and only if for all players (agents), everyone is playing a best response.
- Awesome Thereum: **Every mixed strategy finite game has a Nash equilibrium using**
