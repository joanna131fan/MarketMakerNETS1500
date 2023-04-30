# MarketMakerNETS1500
NETS 1500 Project - Market Maker Simulation
HOW TO RUN: 
To run the simulation, simply open the Colab and click on ‘Run All’ under the ‘Runtime’ tab. Then, the simulation will give you your secret number and prompt you to input your name. After doing so, you will begin the rounds. For each round, input your quote as buy price and sell price in the format ‘buy@sell’ where buy is an integer and sell is an integer. Ideally, buy is less than sell since it doesn’t make sense to want to buy something for more than you want to sell it for, but the code lets you play around with the numbers however you want. At the end of the simulation, you will be given your opponent’s numbers and their strategies and your own PNL. 
You are free to change the constants in cell 2 as well as the strategy ranges of the computers in the strategy class section.

GAME BREAKDOWN:
(Screenshots of game in folder)

From the perspective of the market maker, the objective is to provide liquidity to the market by continuously offering quotes to buy and sell the asset at prices that are close to the fair value. In this game, the market maker is asked to make a market on a number that is equal to their secret number plus the sum of all five opponents' secret numbers.

In the first round, the market maker sets a quote of 66@70, which means they are willing to buy the asset at 66 and sell it at 70. Players 2, 4, and 5 hit the bid at 66, which means they are willing to sell the asset to the market maker at that price. The market maker acquires three stocks at a cost of 66 each and incurs a cash outflow of 198. At the end of the first round, the market maker's position is 3 stocks.

In the second round, the market maker sets a quote of 62@73, which means they are willing to buy the asset at 62 and sell it at 73. Player 2 and 5 hit the bid at 62, which means they are willing to sell the asset to the market maker at that price. The market maker acquires two additional stocks at a cost of 62 each and incurs a cash outflow of 124. At the end of the second round, the market maker's position is 5 stocks.

In the third round, the market maker sets a quote of 61@63, which means they are willing to buy the asset at 61 and sell it at 63. Player 1 lifts the offer at 63, which means they are willing to buy the asset from the market maker at that price. The market maker sells one stock at a price of 63 and incurs a cash inflow of 63. At the end of the third round, the market maker's position is 4 stocks.

In the fourth round, the market maker sets a quote of 60@64, which means they are willing to buy the asset at 60 and sell it at 64. No player takes any action, and the market maker's position remains the same at the end of the fourth round.

In the fifth and final round, the market maker sets a quote of 61@65, which means they are willing to buy the asset at 61 and sell it at 65. Player 2 and 5 hit the bid at 61, which means they are willing to sell the asset to the market maker at that price. The market maker acquires two additional stocks at a cost of 61 each and incurs a cash outflow of 122. At the end of the fifth round, the market maker's position is 6 stocks.

At the end of the game, the market maker reveals the secret numbers and player ranges, which allows them to calculate the fair value of the asset, which is determined to be 76. The market maker then computes their total PNL, which is the difference between the cash inflows and outflows they incurred throughout the game and the value of their remaining stocks exchanged at the fair value. In this case, the market maker's total PNL is 98, which means they earned a profit of 98 dollars from making a market in this game.

