# Charting in Python: Graphics Lies, Misleading Visuals
This study is an assignment of "Applied Data Science with Python" by University of Michigan. This assignment of the course draws heavily on Alberto Cairo’s book, The Truthful Art, where five qualities of great visualizations (truthful, functional, beautiful, insightful, and enlightening ) are explained. Assignment instruction specified that "locate an example of a misleading visual that uses one or more of the mechanisms for misleading that Cairo outlines in his book". So the study was taken shape from the instructions.

While making a small search in online newspapers, I saw a chart in today's print (13.09.2019) of "Sabah",which is one of the bestseller newspaper in Turkey. The chart is related to the decision of the Republic of Turkey's Central Bank's (TCMB) 'Policy Interest Rates'. We learned from the news that TCMB decreased the interest rates from 19.65% to 16.50%. But __the chart doesn't show this news exactly.__

The intended audience of the newspaper is the general public. But generally, some news, especially related to the economy, are announced more softly. Also sometimes, details or some parts of the news are hidden (and/or not explained clearly) deliberately. __I think this chart one of the example of this "Misleading Visuals".__

To understand the news correctly, firstly I visited the TCMB web sites and scraped the 'Policy Interest Rates' data which include from 2010 to today by BeautifulSoup.

After visualizing the data, differences between the chart of the news and chart of the real-data is seen clearly.
- In x-axis of the chart does not compatible with the real-time. The time period of 24%-19.75% is more than 3 times longer than the time period of 17.75%-24%. But the reality of the "living with high-interest rates" is hidden in the chart.
- Also because of the manipulating in the x-axis, as if understood that the peak of the interest rate (24%) continues a small time period. But in real-time, "living with high-interest rates" continued nearly a year and this period should be shown in chart clearly.
- In chart, it is shown that there is a point (value) exist between the time period of 17.75%-24%. But in real data, there isn't any value exists between this period. With the chart, as if understood that reached the peak of the interest rates (24%) slowly. The reality of sharp increase is hidden with unreal data in the chart.
- Lastly, while looking at the chart it is understood that with the TCMB' decrease decision the interest rates come back the normal level. Because the chart contains the last 2 years period. If looking at the timeline more widely, it is understood that the interest rates are still high.

Visualization tells us much more information quickly than text in addition to permanent. It is an easy way to explain the long texts, numbers, correlations. But like this example, sometimes it can be used for misleading the public.

## Used Libraries
- The data was scraped (collected) from tcmb.gov.tr with Python _BeautifulSoup_ library.
- Visualizing the result by Python _Matplotlib_ library.
