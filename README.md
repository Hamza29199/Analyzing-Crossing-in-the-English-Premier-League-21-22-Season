# Analyzing-Crossing-in-the-English-Premier-League-21-22-Season

Crossing is one of the oldest and most intuitive attacking movements in football, but is it as effective as it is popular? Is it the best way to create
attacking opportunities, or is it just a wasteful exercise at the end of the day? Personally, I think teams are better off investing their precious seconds
into retaining as much possession of the ball as possible and progressing it forward smartly....but I wanted to get the relevant data and see for myself
if my instinct about crossing was correct. 

As a fan of Premier League football - big up Manchester City! - I headed over to Kaggle to fetch data for this past season of English top flight football i.e. 21/22.
As any fan can attest, it happened to be one of the most dramatic seasons to date, with City quite literally clinching the title with a few minutes to go. 
However, what did it look like in terms of good ol' crossing? 

# Quick Overview of Data

The data, entitled "English Premier League Data 2021/22", was fetched from Kaggle and comprised a bunch of CSV files containing information on everything from
attempts on goal made by teams across the season to referee stats. However, the one I was interested in the most was "attacking.csv", since it had fields on corners 
cross attempts and cross accuracy and more. The link to the dataset: https://www.kaggle.com/datasets/charlesadedotun/epl-data-2021-22

# Connecting to Tableau

I connected the data to Tableau and quickly ensured that there are no null values. It's a pretty straightforward file really, with just 20 rows corresponding to the
20 premier league teams and five fields - Matches, Total Corners, Average Corners, Crosses Attempted, and Crossing Accuracy. But the analysis I was going to perform
and visualize would answer some burning questions I had about the utility of crossing.

# Calculations

Again, about the only calculated fields I included are Goals Per Match and Crosses Per Match, as I wanted to break it down on a "per-game" level and eventually see if
there has been any correlation at all between crosses and goals per match in the 21/22 season.

# First and Second Visualizations

So the first two visualizations are bar charts looking at the top five teams most reliant on crosses per match and the top five teams least reliant on crosses,
respectively. A few important insights here:
* Liverpool, with 5.82 crosses per match, has relied the most on crossing as an offensive strategy this past season. And it makes sense, given the strength they
have in full-backs Trent Alexander-Arnold and Andrew Robertson. Trent, specifically, is lethal with his right foot and has consistently ranked among the top
assisters in the league for the past few seasons (finished at second spot this season with 12 assists!) and you best believe that the majority of them were 
crosses
* Man City, averaging 4.39 crosses per match, is once again understandable given their strength in full-backs, especially Joao Cancelo who is up there with
Trent in terms of most offensive-minded full-backs in the league
* Surprisingly, we also see Brighton, Everton, and Burnley in this top 5. Two of these three teams have spent extended periods of time in the relegation zone 
(Burnley in fact did get relegated), so what's the deal here? Well, as I mentioned at the start, crossing is one of the most intuitive moves at your disposal.
If you are the kind of team that goes behind a lot (and safe to say, relegation threatened teams do find themselve trailing in games A LOT), you are more likely
to desperately whip in crosses, hoping for one of your tall strikers to head it in or an opposition defender to fumble it or for any manner of scoring opportunity
really.
* Brighton is a more interesting one because it finished 9th this season (an impressive finish given the resources and players they have at their disposal) and
it has attempted the second-most crosses on average this season. The answer lies in its formation - 3-5-1-1 - with wingbacks like Cucurella and Lamptey and wingers
like Trossard more than happy to progress forward and whip a cross or two in for the likes of Danny Welbeck. Cucurella, in fact, has been one of the stand-out
offensive full-backs this season alongside the likes of Trent and Cancelo so once again, a case of a team relying on its strengths here.
* In the second viz, I will only talk about Leicester because it has averaged the least crosses per match this season with just 2.58, while the others have all
averaged between 3 and 4. This can be explained my manager Brendan Rodger's newer strategy of relying on his two strikers up front - Vardy and Iheanacho - to
impact attacks with midfielder James Maddison sitting right behind them as a no.10 in a 3-4-1-2 formation. With an average of 2.29 points per game using this
system, it's little wonder that the Foxes have been more than happy to ignore a wing-heavy cross-happy system.

# Third Visualization

This one is a treemap depicting cross accuracy for teams across the season. Cross accuracy, by the way, is simply the percentage of crosses that meet their intended
target. It doesn't necessarily mean a cross that results in a goal, but a cross that is delivered accurately speaks volumes about the team's fortunes. After all,
the more you meet you target, the more you increase your chances of having a shot on target and hopefully a goal.

Here, our leaders are the likes of Brighton, Everton, and Newcastle, each of whom have essentially had one out of every four crosses meet a man. We've already
talked about Brighton's strengths, so let's take a look at the other two. If I had to take a guess, I'd point to the quality of the wingers and wing-backs both
teams have. While they have had their fair share of struggles in various departments - the centre-backs for Everton, the lack of midfield quality for Newcastle -
they have been blessed with a few brilliant players. The young winger Demarai Gray for Everton, for instance, had a pass accuracy of 81% across all comps, and 
created over 40 chances on his own. Similarly, for Newcastle, the likes of Allan Saint-Maximin (76% pass acc with almost 50 chances created across all comps)
and left-back Emil Krafth who impressed fans so much with his performances that he was called the "Swedish Cafu". That tells you everything, really.

# Final Visualization
