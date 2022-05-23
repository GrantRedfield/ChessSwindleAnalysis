# A Closer Look Of Swindles In Chess
For those less familiar with the term "swindle", this is winning a chess game that 


Recently [books](https://www.amazon.com/Complete-Chess-Swindler-Points-Positions/dp/9056919113/ref=sr_1_4?crid=3W3KRYLEVGMRW&keywords=swindling+chess&qid=1652719878&sprefix=swindling+chess%2Caps%2C88&sr=8-4) have come out around the art of swindling in chess. Its an unavoidable phenomenon that haunts us all, or gives us something to play for. I couldnt seem to find the question **"What are my chances of swindling my opponent in a lost game?"** I tried to quantify this backed up by some statistics.

Using [This](https://web.chessdigits.com/data) dataset of 200k lichess games (Blitz + Rapid + Classical), I was able to extract out how many games were in the following categories.
1. **SteamRoll** :One-sided game played well by one opponent with no big opportunities
![SteamRoll](https://github.com/GrantRedfield/ChessSwindleAnalysis/blob/main/SteamRoll.JPG)


2. **Chaotic Game** : This game full of chances from either side from the beginning. Not a game I would consider a  traditional "swindle"
![](https://github.com/GrantRedfield/ChessSwindleAnalysis/blob/main/Chaotic_Game.JPG)


3. **Swindle** :  A game where one side is in control the majority of the game, up until an opportunity for the opponent at a later stage
![](https://github.com/GrantRedfield/ChessSwindleAnalysis/blob/main/Swindle.JPG)



**How Many Opportunities Do You Have To Swindle Based On Your Rating?**

Out of 10 losing games, these are the amount of games You will have an opportunity to turn things around.
![](https://github.com/GrantRedfield/ChessSwindleAnalysis/blob/main/Number%20of%20Opportunities%20To%20Swindle%20Out%20of%2010%20Losing%20Games.jpg))

Rating 0-1000: There is a probability of 81% that 4 or more games contain swindle chances

Rating 1001-1500:  There is a probability of 64% that 4 or more games contain swindle chances

Rating 1501-2000: : There is a probability of 69% that 3 or more games contain swindle chances

Rating  2000+:  There is a probability of 74% that 2 or more games contain swindle chances

**Are There Points In A Game Where Swindle Opportunities Are More Prevalent?**

For this question I focused on two factors;  The Opponents % Time Left and The Move Number When a Swindle Opportunity Occurs

First I looked solely at the opponents time left, and came up with interesting results.
![](https://github.com/GrantRedfield/ChessSwindleAnalysis/blob/main/Percent_Time_Left_Swindle_Occurs.jpg)

There are two opportunities when your opponent slips up; When they play too fast and when they play too slow. Its intuitive, but It's fascinating that the majority happen around the 75th percentile. This is likely due to a relatively complex middle game combined with reckless fast moves. The time pressure is explainable as its harder to be accurate.

When charting percent time left against the move number, we get a pretty neat graph showing clusters of swindle opportunities

![](https://github.com/GrantRedfield/ChessSwindleAnalysis/blob/main/Move_vs_Opponent_Time_Left.jpg)


**Conclusion:**

1. I think its possible to incorporate this knowledge into your own games. The move number + the knowledge of your opponents time left can give you some clues into and ideal scenario where your opponent will blunder their advantage away.
2. Psychologically its important to not give up. There will be opportunities throughout the game to turn things around in your losing games.


