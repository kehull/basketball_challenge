# basketball_challenge
 
View coding for data analysis [here](https://github.com/kehull/basketball_challenge/blob/main/Untitled.ipynb)

As a milennial born in the suburbs of the great city of Chicago, some of my earliest memories involve sitting in the living room with my family while my father and brother yelled at the 90's Bulls games on TV. More memorably- for me, anyway- was the release of the generation-defining film, Space Jam, smack-dab in the middle of my childhood. I didn't then and I don't know know anything about basketball, but I did know one thing to be true- Michael Jordan, the man in the #23 jersey, was and would forevermore be the king of basketball. Could I tell you how or why? Absolutely not. Some things are simply true whether you understand them or not.

Absolute truth, however, is not included in the dataset for this challenge. At least, not the absolute truth passed down to me by my father. The truth in this challenge is the pure numbers accumulated over the careers of Michael Jordan, Kobe Bryan, and Lebron James. Would it be possible for me, an admittedly highly-biased observer, to fairly analyze the data and determine which of these men is the greatest player of all time?

Before we can answer this question, we must ask ourselves- what makes a player great, anyway? As a sports outsider, this led to a series of other questions for me- question such as "Why is there a 'Field Goal' category here? Aren't field goals a soccer thing?' As you can see in my code, my first step was to furiously Google all of the abbreviations in the dataset and rename the columns to something I could understand. Sort of. At least they're in English now.

Under normal circumstances, I'd dive into research on what all the stats mean exactly, but between work and school I've had exactly three hours of free time over the last month to complete this challenge, so I made the decision to limit my research to topics I already understand- things like points and salaries.

This led me to my thesis- the NBA is a corporation. Corporations need to earn money, and they need to save on costs. Therefore, it stands to reason that the player with the highest bang-to-buck ratio could very well be considered the greatest player by the NBA.

Note: my take on this study was partly inspired by [this study on tbe best-value actors in hollywood](https://www.statista.com/statistics/649757/best-value-actors-in-hollywood/#:~:text=The%20statistic%20presents%20a%20ranking,one%20dollar%20of%20his%20pay.)

First, I used the salary, points per game, and minutes played per game calculations to determine the average cost per minute and cost per point per player over the course of their career.

![](https://github.com/kehull/basketball_challenge/blob/main/images/cost_per_minute.png?raw=true)

![](https://github.com/kehull/basketball_challenge/blob/main/images/raw_plot.jpg?raw=true)

While the numbers are indeed fascinating, I was struck by the great disparity between the clear winner (Michael Jordan, earning less than 50% per point and per minute of gameplay than either James or Bryant) and his competition. While charting the data in matplotlib, the realization hit me- the three careers in question span from 1988 to 2017 within the dataset. Inflation exists. Could it be that Michael Jordan was not the clear winner?

I did some more Googling, and with a bit of an assist from [SmartAsset.com's inflation calculator](https://smartasset.com/investing/inflation-calculator) (admittedly, not a perfect metric, but it would have to do), I was able to write a for-loop that adjusted each player's salary to 2017 dollars.

![](https://github.com/kehull/basketball_challenge/blob/main/images/adj_cost_per_minute.png?raw=true)

![](https://github.com/kehull/basketball_challenge/blob/main/images/adj_plot.png?raw=true)

Even with salaries adjusted for inflation, based on my initial thesis of cost effectiveness, Michael Jordan still reigns supreme.

![Jordan gif](https://media4.giphy.com/media/l46CqLVMWzaJUFPLW/giphy.gif)

Thank you for your time.
