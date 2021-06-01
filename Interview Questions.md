# Interview Questions


### 1. 	What is the conversion rate for an individual flight search result?

The formula I would create for conversion rate would be (Non-Null Result) / (opening up alaskaair.com). A non-Null Result is a search for a destination that Alaska Airlines serves during the date the customer searches. A Null Result is a search for a destination that Alaska Airlines does not serve during that specific date or airport.
We would track an individual opening up alaskaair.com by looking at their IP address or potentially every unique webpage that opens up alaskaair.com; this method would be dependent on whichever method is compliant with GDPR laws.
I would pull this data from SQL and transform the data in Python, then display it in PowerBI. In PowerBI, I’d display a bar graph that shows which filters each individuals click or not.


### 2. How does the cost in miles affect the guests’ willingness to purchase?

I would create 3 different formulas for guests' willingness to purchase and for guests' that purchase in dollars. One for individuals who didn’t log in, one for individuals that did, and one for both. The formula would be (Result) / (Purchase). This would pull data from the previous question, and I would create a column in SQL for purchases as well.

I would compare 2 bars for each of the 3 formulas, one for guests' that saw cost in miles and the other for guests' that saw the cost in dollars. This visual would be in PowerBI.

Lastly, I would do an A/B test comparing the two formulas, one comparing cost in miles and the other comparing cost in dollars to see if one is more statistically significant than the other. I'd use p-value and lift metrics to find my results.

### 3. How many times does a guest attempt to search for a destination that we do not serve for the given airport or date?

I would create the track the number of times and location a guest attempts to search for a destination that we do not serve for the given airport or date.

Additionally, I would present the findings in two bar graphs displaying which are our top 10 airports that are chosing to fly depart from (first graph) and are chosing to arrive to (second graph). This would give our team an idea of which potential airports we should target to service at.

After finding the top airports, I would filter the airports each top airports top 5-10 dates to see which dates individuals most likely want to fly into each location, so we can provide the frequency of how often we should service in these locations and at what time periods in the year.