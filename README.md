# Client in FX Market
> Tags: [Market Research], [Data Analytics], [BI]
>
> Technical Skills: [PowerBI], [Excel]
>
> Theoretical Frameworks: [SWOT Analysis], [Financial Analysis], [Industry Analysis]

> [!Note]
This lite version of the study includes only the chapters that incorporate open-source information.

**Client in FX Market** is a cut-down version of a project in my former workplace that was not released due to a sudden shut-down. The prompt of the study was to create a better understanding of the new client, and also investigate where else we can further support their business. 

**Subject**: Client operates in the Foreign Exchange market and offers a bespoke travel card, which targets UK audience, that trades in low rates against the high-street banks.




![image](https://github.com/user-attachments/assets/5b9c3e14-ad0d-4b26-b2c3-57ce97f289bf)


## Original Framework

The following chapters consists of the original framework of the study: 
1. Executive Summary,
2. Industry Overview,
3. Competitor Identification,
4. Competitor Profiles,
5. Competitive Landscape,
6. Product/Service Comparison,
7. Marketing and Sales Strategies,
8. Customer Analysis,
9. Technology and Innovation,
10. Strategic Recommendations,
11. Appendices.

## Current Version
This lite version of the report breaks down the first four chapters. In more detail:
1. Executive Summary
	- Objective: State the purpose of the analysis.
	- Scope: Define the scope of the analysis, including markets and competitors covered.
2. Industry Overview
	- Market Size and Growth: Provide data on the current size and growth rate of the industry.
	- Trends and Drivers: Highlight key trends, drivers, and challenges shaping the industry.
	- Regulatory Environment: Mention any relevant regulations impacting the industry.
3. Competitor Identification
	- Direct Competitors: List and describe direct competitors in the market.
	- Indirect Competitors: Identify and describe indirect competitors or substitutes.
	- Potential Entrants: Note any potential new entrants that could impact the market.
4. Competitor Profiles
	- Company A:
		- Overview: Brief description of the company.
		- Market Position: Current market share and position.
		- Products/Services: Key products or services offered.
		- Strengths: Competitive advantages and strengths.
		- Weaknesses: Areas where the company is lacking.
		- Financial Performance: Recent financial data and performance metrics.
		- Strategies: Key strategies employed (e.g., pricing, marketing, partnerships).
		- SWOT Analysis: Detailed SWOT analysis.
	- Company B, and so on.


## Market Analysis


![image](https://github.com/user-attachments/assets/24225573-8cb6-4495-aa5f-7270a069c6d4)
> [Outbount Travel Industry Dashboard.pdf](https://github.com/user-attachments/files/16713539/Client.in.FX.Market.pdf)
>
> Power BI Dashboard made out of the IPS (International Passengers Survey) dataset: [Travel Pac, 2023](https://www.ons.gov.uk/peoplepopulationandcommunity/leisureandtourism/datasets/travelpac) of ONS (Office of National Statistics.)

The first goal was to identify the exact industry/market which our client operates in, and understand what market share are they competing for. 
This helps to create a benchmark and evaluate what *current efforts* bring back home.

Logically speaking, for UK focused only audience, it was pretty straight forward to what I'm looking for to denote as "Market Share." I am looking for UK populace that goes abroad, regardless of reason. A.k.a the Outbound Travel Industry.

I was thrilled when I had found 2023 data for the International Passergers Survey, that essentially ask for questions such as age, duration, expenditure, destination, e.t.c.

Right away, from the static Power BI dashboard picture provided above, we can observe a couple of interesting findings in the exploratory part of the analysis. 
1. The UK populace has three predominantly preferred destinations, based on number of visits:
	- France (9.44%)
	- Spain (5.61%)
	- Netherlands (4.72%)
2. Interestingly enough, the expenditure of the destinations procure a second list with Spain being the holiday destination where people prefer to spend more, over France over Netherlands:
	- Spain (17.41%)
	- France (8.67%)
	- Netherlands (1.83%)
This insight already labels and defines "premium locations."
3. The most travelled age groups are:
	- 35-44 (14.23%),
	- 25-34 (14.03%),
	- 45-54 (12.30%).
4. Usually, the UK populace would prefer their getaway, business, or visiting family and friends (VFR) to be done in a span of 4-13 nights, over 14-27 nights, over 1-3 nights:
   	- 4-13 nights (43.31%),
   	- 14-27 nights (22.52%),
   	- 1-3 nights (21.71%). 
4. For this one, I had to create "Expenditure Bands" in order to segment the consumer's habits. After going through the expenditure values, I decided that the information would be analysed and displayed better if I broke down the segment into 10 bands.
	- Band 1: >1m, anyone that has spent more than a million,
	- Band 2: >=500k - <1m, -//- anywhere between 500k to 1m (-1),
	- Band 3: >=250K - <500K, -//- 250k to 500k (-1),
	- Band 4: >=100k - <250K, -//- 100k to 250k (-1),
	- Band 5: >=50k - <100k, -//- 50k to 100k (-1),
	- Band 6: >=25k - <50k, -//- 25k to 50k (-1),
	- Band 7: >=15k - <25k, -//- 15k to 25k (-1),
	- Band 8: >=10k - <15k, -//- 10k to 15k (-1),
	- Band 9: >=5k - <10k, -//- 5k to 10k (-1),
	- Band 10: <249, anyone that has spent less than 250 pounds.

Up until this point, I was happily exploring this dataset, feeling so *hyped* that I have found an immediate solution to my problems, and there was a source I can rely on, as ONS generally is known for validity. But the moment I had segmented expenditure in 10 whole bands, I realised something was off.

Let me explain. In the past, whenever I had to segment a feature, the more bands I made meant that there are data entries stuck behind a percentile in the distribution of the dataset. Based on what it is that you are trying to breakdown, a number of data entries under a certain percentile, make no sense.

Let me ask you if you noticed anything wrong with the data presented on the dashboard. Want to go back and have a quick look?

**How** is it possible that 62.94% of the people that have travelled for *any* reason, spent more than 1 million GBP on their travels? Unless travelling nowadays is a millionaire-only thing, then some of the passengers answering those surveys might have not been 100% *honest*.

Moreover, 2.17% or 366 people managed to make do with their travels with budget of under 249 pounds. Now, that's impressive. I now knew that the market share that I had denoted early on the research of Outbound Travel Industry being valued somewhere between £71.5bn - £75bn in 2024 with a stated CAGR of 8.6% over 2024 - 2034, is a metric with inconsistent data evidence.

> Enter <Micheal Scott screaming "NO" when he found out Toby from HR had in fact returned> gif here.

## The Real Problem
If I found that dataset, and I made that mistake, it is almost certain that other analysts have done it as well. And indeed, analysts from big market research companies have used that same dataset, and made a whole prediction for 10 years in the future. **Ah, the wonders of analytics!** 

Funnily enough, it all goes back to the fundamental question which my mother used to ask me all the time when I did something under the premise of "It wasn't just me, the other kids did it as well, mom!", which is "If *the other kids* ran and jumped off a cliff, would you do it as well?" <sub> ..well, how big is the fall.. </sub>

Some of you could argue: "But Fanis, if the market has the same false information and big research companies use that same false information to create a chassis of how the market is going to be, and every business is using that very false chassis to benchmark and compare themselves, isn't this becoming a new reality and the nash equilibrium is to use the same false information and chassis and benchmark your client and their strategies to the false standards?"

**You are chaotic neutral and I like you.** but no.

Jokes aside, even with such a setback, the competitive research yielded far greater results even with the uncertainty of the Market Share. In the end, I did create an artificial share for the client's industry in order to simulate appropriate strategies. Conveniently enough, this great effort does not appear in the lite-version of the report that can be found in this repo, but as Jack Black once said:

>This is not the greatest song in the world, no
>
>This is just a tribute

## Lessons Learnt

This case study, has reinforced some of my beliefs. 

1) Always have your own internal voice and thoughts: if it does not look or feel right, you do not force the numbers in your study.
2) The earlier you accept the setback, the better. Think of this as a sunk cost; It is more harmful to keep building your analysis around unreliable data and unsustainable in the long-term.
3) Be open-minded with problem-solving. In Academia, problem-solving demands are straightforward: use framework X to solve problem Y. In the day-to-day problems, you need the understanding of multiple frameworks and concepts, in order to solve a problem.
4) When creating insights from raw data, draw a distinct relationship about what can be and what can't be supported in your hypotheses. It will make those meetings with the clients and managers/directors way easier.
5) Do not underestimate the knowledge earned from rejecting a hypothesis. It contributes to your understanding of the market and its modus operandi. That helps a lot, particularly in the past when I was working for the Marketing Industry. 

The lite-version of the report can be found [here.](https://github.com/FanisGl/Client-in-FX-market/blob/main/Report/Competitive%20Analysis%20-%20FX%20market.pdf)
