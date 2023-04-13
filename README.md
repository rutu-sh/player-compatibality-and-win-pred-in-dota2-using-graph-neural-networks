# player-compatibality-in-dota2-using-graph-neural-networks
## Dota2

Dota 2 is a multiplayer online battle arena (MOBA) game developed and published by Valve Corporation. It is the sequel to Defense of the Ancients (DotA), which was a community-created mod for Blizzard Entertainment's Warcraft III: Reign of Chaos.

In Dota 2, two teams of five players compete against each other with the goal of destroying the enemy team's ancient, a heavily guarded structure at the center of each team's base. Each player controls a single hero, chosen from a pool of over 120 unique characters, each with their own abilities and playstyles.

The game is played on a symmetrical map divided into three lanes, with neutral territory and forests separating them. The teams start at opposite corners of the map, with their bases and ancients located at the opposite ends of the central lane.

Players earn gold and experience by killing enemy units, including heroes, creeps, and towers. Gold can be used to purchase items, which enhance a hero's abilities and attributes, while experience is used to level up a hero and unlock new abilities.

Communication and teamwork are essential in Dota 2, as each player must work with their team to coordinate their strategies and make the most of their hero's unique abilities. The game is known for its complex gameplay mechanics and steep learning curve, as well as its thriving esports scene, with millions of dollars in prize money awarded each year at international tournaments.

## e-sports

Dota 2 has a vibrant esports scene, with numerous tournaments held throughout the year featuring some of the best professional players from around the world.

The pinnacle of Dota 2 esports is The International, an annual tournament organized by Valve Corporation that brings together the best teams from around the world to compete for a multi-million dollar prize pool. The International has become one of the most prestigious esports events in the world, with fans and players alike eagerly anticipating its arrival each year.

In addition to The International, there are numerous other Dota 2 tournaments held throughout the year, both online and offline, with varying prize pools and levels of competition. Major tournaments include the Dota Pro Circuit (DPC) events, which are sponsored by Valve and offer qualification points for The International.

Dota 2 tournaments typically follow a standard format, with teams competing in a round-robin or double-elimination bracket to determine a winner. Matches are typically played in a best-of-three or best-of-five format, with the winning team advancing to the next round.

Dota 2 tournaments are often broadcast live on streaming platforms like Twitch and YouTube, with millions of fans tuning in to watch the action unfold. Commentators and analysts provide live commentary and analysis of the matches, helping viewers understand the complex strategies and gameplay mechanics involved.

Overall, Dota 2 esports tournaments are a thrilling spectacle, showcasing the highest levels of skill and teamwork in one of the most popular and competitive esports games in the world.

## Related Works

Being a highly competitive e-sport, players need a good coordination with each other. Each team can pick and ban heros from selection, and hence the team's composition matters, the players should be able to play with heros of varying skills so that the team can make a balanced selection of heros that can counter the opposition. 

Work has been done on analysing the hero composition in teams. Conley et al., 2013 <sup>[1]</sup> had created a recommendation engine for picking heros in Dota2 that will perform well against the opposing team of heros. Atish et al., 2014<sup>[1]</sup> had found a correlation between the hero selection and the chances of winning, by modelling the interactions between heros by performing logistic regression. Wang et al, 2016<sup>[3]</sup> introduced neural networks along with duration of the match as one of the features. Chen, Zhengxing et al, 2018<sup>[4]</sup> generated embeddings for hero avatars and used synergy and opposition between them to predict the probability of win. Wong et al., 2022<sup>[5]</sup> surveyed several methods for predicting the match outcome and first-blood in Dota2, based solely on pre-match team character selections. 

There is an underlying assumption to the approaches mentioned. They only model the interaction between heros, ignoring the interaction between players, assuming that each player is equally skilled. Cheng, Ziqiang et al., 2019<sup>[6]</sup> have done an analysis on the effects of team composition in MOBA games like "Honor of Kings" and found the effect of the individual players on the team composition and how it affects winning, surrendering, and abusive language in the game. Ahmad, Sabbir et al., 2019<sup>[7]</sup> have proposed a method to model individual and team behavior by labeling tactical and strategical decisions and visualize them. In a separate approach, Yang, Pu et al., 2014 <sup>[8]</sup> have used graphs to represent combat as a sequence of graphs and used the features from extracted from those graph to train a decision tree and generate graphs denoting patterns in compat that can lead to a win. These studies have shown that the interaction between players is also an important feature while modeling a system for MOBA games. 

In the space of representing entities and the relationship between them, a lot of developments have been made in the domain of Graph Neural Networks. 



## References


[1] Conley, Kevin and Daniel Perry. [“How Does He Saw Me ? A Recommendation Engine for Picking Heroes in Dota 2.” (2013)](https://www.semanticscholar.org/paper/How-Does-He-Saw-Me-A-Recommendation-Engine-for-in-2-Conley-Perry/7b890df91c53b7c1a489dd5a1f30b608f5cb3546)

[2] Agarwala, Atish [“Learning Dota 2 Team Compositions.” (2014)](https://cs229.stanford.edu/proj2014/Atish%20Agarwala,%20Michael%20Pearce,%20Learning%20Dota%202%20Team%20Compositions.pdf)

[3] Wang, Weiqi. [“Predicting Multiplayer Online Battle Arena (MOBA) Game Outcome Based on Hero Draft Data.” (2016)](https://www.semanticscholar.org/paper/Predicting-Multiplayer-Online-Battle-Arena-(MOBA)-Wang/5fdc77ba44903fbfe229aa256d0919f4fbb04511)

[4] Chen, Zhengxing et al. [“Modeling Game Avatar Synergy and Opposition through Embedding in Multiplayer Online Battle Arena Games.” _ArXiv_ abs/1803.10402 (2018): n. pag.](https://www.semanticscholar.org/paper/Modeling-Game-Avatar-Synergy-and-Opposition-through-Chen-Xu/67050ffbe46164b48bdf64a91364883a8c2884ce)

[5] Wong, Nicholas Heng Loong et al. [“Predictive Analytics of First Blood and Match Outcome in Dota 2.” _TENCON 2022 - 2022 IEEE Region 10 Conference (TENCON)_ (2022): 1-6.](https://www.semanticscholar.org/paper/Predictive-Analytics-of-First-Blood-and-Match-in-2-Wong-Kwok/5b63766687e6fa7ce58859ddaea679fa2f5e3f27#references)

[6] Cheng, Ziqiang et al. [“What Makes a Good Team? A Large-scale Study on the Effect of Team Composition in Honor of Kings.” _The World Wide Web Conference_ (2019): n. pag.](https://www.semanticscholar.org/paper/What-Makes-a-Good-Team-A-Large-scale-Study-on-the-Cheng-Yang/37a1db2f1e064b7579c07721ee3fd77b6b583958)

[7] Ahmad, Sabbir et al. [“Modeling Individual and Team Behavior through Spatio-temporal Analysis.” _Proceedings of the Annual Symposium on Computer-Human Interaction in Play_ (2019): n. pag.](https://www.semanticscholar.org/paper/Modeling-Individual-and-Team-Behavior-through-Ahmad-Bryant/2266597c947d0b2407dbca5bfbf2cfa9e05b22bd)

[8] Yang, Pu et al. [“Identifying patterns in combat that are predictive of success in MOBA games.” _International Conference on Foundations of Digital Games_ (2014).](https://www.semanticscholar.org/paper/Identifying-patterns-in-combat-that-are-predictive-Yang-Harrison/9bc1cfc95bcaeb08ce460b797e6718fe522aff95)

