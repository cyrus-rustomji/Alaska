# Interview Questions


### 1. 	What is the conversion rate for an individual flight search result?

First, I would take note of all the filters that would be in this formula. It would include either a round-trip, one-way, or multi-city stop, you use miles, the places you are leaving and going to, adults, children, dates, and/or you have a discount code or not. We would need all these factors to better determine if individuals are more or less likely to click these factors when looking up a flight search result.

The formula I would create for conversion rate would be (Non-Null Result) / (opening up alaskaair.com). A non-Null Result is a search for a destination that Alaska Airlines serves during the date the customer searches. A Null Result is a search for a destination that Alaska Airlines does not serve during that specific date or airport.
We would track an individual opening up alaskaair.com by looking at their IP address or potentially every unique webpage that opens up alaskaair.com; this method would be dependent on whichever method is compliant with GDPR laws.
I would pull this data from SQL and transform the data in Python, then display it in PowerBI. In PowerBI, I’d display a bar graph that shows which filters each individuals click or not. Thus comparing, which filters or a combination of filters bring out a higher conversion rate and highlight those filters.


### 2. How does the cost in miles affect the guests’ willingness to purchase?

When I think cost in miles, my immediate though or bias is that individuals who think in miles usually either have an Alaska account, are thinking about getting an Alaska account, or have a gift card or voucher that are in miles.

Therefore, I would create 3 different formulas each for guests' willingness to purchase and for guests' that purchase in dollars and in miles. I would add purchase in dollars to see individuals what the data would look like for individuals who do not have account or gift card. These 3 formula would be one for individuals who didn’t log in, one for individuals that did, and one for both. The formula would be (Result) / (Purchase). This would pull data from the previous question, and I would create a column in SQL for purchases as well.

I would also compare 2 bars for each of the 3 formulas, one for guests' that saw cost in miles and the other for guests' that saw the cost in dollars. This visual would be in PowerBI.

Lastly, I would do an A/B test in Optimizely comparing the two formulas, one comparing cost in miles and the other comparing cost in dollars to see if one is more statistically significant than the other. I'd use p-value and lift metrics to find my results.

### 3. How many times does a guest attempt to search for a destination that we do not serve for the given airport or date?

Initially, I would create a list of airports that we currently do not serve. Then, I would join that list on attempted searches to see when and how often individuals searched for those destinations. I would store this data in SQL and create a PowerBI pipeline to display the results, so it refreshes daily and we can see which airports we should prioritize to service soon.

I'd present these findings in two bar graphs displaying which are our top 10 airports that are chosing to fly depart from (first graph) and are chosing to arrive to (second graph). I would only limit it to 10 or less in the bar graph, so it's easier to digest for the executive team.

After finding the top airports, I would filter the top 5-10 dates to see which dates individuals most likely want to fly into each location, so we can provide the frequency of how often we should service in these locations and at what time periods in the year as well.