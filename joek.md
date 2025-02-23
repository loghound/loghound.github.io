# Joe-K-Annuity

Joe Kuhn did [a video](https://www.youtube.com/watch?v=1bjMv3AQqnc&ab_channel=JoeKuhn) recently where he talked about being 'careful' with annuities because 6% payout is different than 6% CAGR.  **He is completely right on this point**.

what is missed, I think, is annuities can be useful as a replacement for bonds in a portfolio.

It's sort of easy to show this using the fantastic https://ficalc.app  You can run pretty easily run scenarios and see how it would have done historically.

Assuming the retiree has:
* $1M in total assets
* $40k/yr withdraw rate (Inflation adjusted)
* Annuities pay 6% (Joe's Rate)
* 30 year expected retirement
* Nominally 60/40 portfolio (i do a 80/20 also) 
* SPIA (single premium immediate annuity) -- this is the most simple product where you give the insurance company money and then they invest it and give it back to you for life.  

As I said it's easy to compare how a retiree would do with and with an annuity 

Link | Success Rate | $ in Stocks |  $ in Bonds | Stock/Bond % | Annuity Invesment | Annuity annual payout (no inflation adjustment) |  Median portfolio end value | Mean Portfolio End Value
-- | -- |---       |---       |--- | -- | -- |-- | --
[Without Annuity](https://ficalc.app?additionalIncome=%5B%5D&additionalWithdrawals=%5B%5D&annualWithdrawal=40000&bondsFees=0.05&bondsFinalRatio=15&bondsInitialRatio=40&cashFees=0&cashFinalRatio=5&cashGrowth=1.5&cashInitialRatio=0&changeAllocationsOverTime=false&equitiesFees=0.04&equitiesFinalRatio=80&equitiesInitialRatio=60&inflationAdjustedFirstYearWithdrawal=true&initialPortfolioValue=1000000&maxWithdrawalLimit=60000&maxWithdrawalLimitEnabled=false&minWithdrawalLimit=20000&minWithdrawalLimitEnabled=true&numberOfYears=30&portfolioRebalanceEquation=linear&rebalance=true&rebalanceFrequency=1&retirementStartingAge=60&withdrawalStrategyName=constantDollar) | 96.7% | $600k | $400k | 60/40 | $0 | $0 | $1,324,181 | $1,882,896| 
[With Annuity](https://ficalc.app?additionalIncome=%5B%7B%22name%22%3A%22Annuity%22%2C%22value%22%3A12000%2C%22inflationAdjusted%22%3Afalse%2C%22delayInflation%22%3Afalse%2C%22lastsForever%22%3Atrue%2C%22duration%22%3A1%2C%22startYearNumber%22%3A0%2C%22disabled%22%3Afalse%7D%5D&additionalWithdrawals=%5B%5D&annualWithdrawal=40000&bondsFees=0.05&bondsFinalRatio=15&bondsInitialRatio=25&cashFees=0&cashFinalRatio=5&cashGrowth=1.5&cashInitialRatio=0&changeAllocationsOverTime=false&equitiesFees=0.04&equitiesFinalRatio=80&equitiesInitialRatio=75&inflationAdjustedFirstYearWithdrawal=true&initialPortfolioValue=800000&maxWithdrawalLimit=60000&maxWithdrawalLimitEnabled=false&minWithdrawalLimit=20000&minWithdrawalLimitEnabled=true&numberOfYears=30&portfolioRebalanceEquation=linear&rebalance=true&rebalanceFrequency=1&retirementStartingAge=60&withdrawalStrategyName=constantDollar) | 96.7% | $600k | $200k | 75/25 | $200k | $12k | $1,775,329 | $2,086,130 |


So we had less risk (even in the few scenarios where we 'ran out of money' the annuity continued to pay out) and we ended up with more money in the median and mean cases.

You may think that I've gamed this to show the annuity to it's advantage but feel free to try different numbers.  Here is an example with a retiree who likes a 80/20 portfolio

Link | Success Rate | $ in Stocks |  $ in Bonds | Stock/Bond % | Annuity Invesment | Annuity annual payout (no inflation adjustment) |  Median portfolio end value | Mean Portfolio End Value
-- | -- |---       |---       |--- | -- | -- |-- | --
[Without Annuity](https://ficalc.app?additionalIncome=%5B%5D&additionalWithdrawals=%5B%5D&annualWithdrawal=40000&bondsFees=0.05&bondsFinalRatio=15&bondsInitialRatio=20&cashFees=0&cashFinalRatio=5&cashGrowth=1.5&cashInitialRatio=0&changeAllocationsOverTime=false&equitiesFees=0.04&equitiesFinalRatio=80&equitiesInitialRatio=80&inflationAdjustedFirstYearWithdrawal=true&initialPortfolioValue=1000000&maxWithdrawalLimit=60000&maxWithdrawalLimitEnabled=false&minWithdrawalLimit=20000&minWithdrawalLimitEnabled=true&numberOfYears=30&portfolioRebalanceEquation=linear&rebalance=true&rebalanceFrequency=1&retirementStartingAge=60&withdrawalStrategyName=constantDollar) | 97.6% | $800k | $200k | 80/20 | $0 | $0 | $2,232,897 | $2,601,041| 
[With Annuity](https://ficalc.app?additionalIncome=%5B%7B%22name%22%3A%22Annuity%22%2C%22value%22%3A12000%2C%22inflationAdjusted%22%3Afalse%2C%22delayInflation%22%3Afalse%2C%22lastsForever%22%3Atrue%2C%22duration%22%3A1%2C%22startYearNumber%22%3A0%2C%22disabled%22%3Afalse%7D%5D&additionalWithdrawals=%5B%5D&annualWithdrawal=40000&bondsFees=0.05&bondsFinalRatio=15&bondsInitialRatio=0&cashFees=0&cashFinalRatio=5&cashGrowth=1.5&cashInitialRatio=0&changeAllocationsOverTime=false&equitiesFees=0.04&equitiesFinalRatio=80&equitiesInitialRatio=100&inflationAdjustedFirstYearWithdrawal=true&initialPortfolioValue=800000&maxWithdrawalLimit=60000&maxWithdrawalLimitEnabled=false&minWithdrawalLimit=20000&minWithdrawalLimitEnabled=true&numberOfYears=30&portfolioRebalanceEquation=linear&rebalance=true&rebalanceFrequency=1&retirementStartingAge=60&withdrawalStrategyName=constantDollar) | 95.9% | $800k | $0k | 100/0 | $200k | $12k | $2,620,290 | $2,932,394 |

In this case we had a slighly worse success rate (but we never really fail with the annuity as we always get **some** money) but we once again ended up with a higher mean & median portfolio balance

Everyone situation is different so you really need to assess for youself (including things like Social Security) but every time I play with this I end up with results like above.  Annuities provide lower risk and greater (long term) returns as long as you are willing to use them as a bond replacement and you think you'll live "long enough"

Ultimately you have to decide what you are comfortable with and not everyone is comfortable with this idea (honestly I retire in 3 weeks at the age of 59 and I'm still sort of on the fence even though when I run the numbers it looks attractive) but my main point is it's worth at least a serious look before you wave your hands and say 'annuities bad'


## What can go wrong?

* this analysis doesn't include any tax implications.  There might be reasons (like roth conversations) where a lump sum starts making more sense (this is highly dependent on your individual situation)
* Insurance companies can go out of business (so either get multiple annuities to spread risk and buy from highly rated companies)
* You may die early -- this doesn't matter to you so much at that point but your heirs might end up with 'less' money then they otherwise would have. (nb the breakeven on this strategy in terms of legacy seems to be 15-20 years)
* Ficalc.app may be have a problem with it's math -- I've checked it a bunch of times against other tools and it works really well in my experience but perhaps?
* The future may be significantly different than the past (duh?) - ficalc useses historical data so all it can tell you how you **would** have done. Not have you **will* do. This is a hard thing to plan for however since, you know, "who knows" what the future holds. 
* Probably other things that I can't think of right now -- like any financial decision it has risks (but also doing nothing has risk, so.....)

