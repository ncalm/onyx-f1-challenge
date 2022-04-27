# onyx-f1-challenge

The files in this repository were created and used to submit an entry to the Onyx Data #dataDNA challenge in April 2022.

My personal goals were:

1. Refamiliarize myself with DAX and recent features of Power BI Desktop
2. Gain more experience with M and Power Query

## The challenge

The challenge link:
https://onyxdata.co.uk/dataset_challenge/april-2022/

The brief was:
"Can you identify the dominating drivers and constructors of Formula 1 (F1)"

## Notes on my analysis and approach:

Since the point systems changed frequently and regulations regarding constructor participation evolved over the decades, I created a scenario modelling tool to see what the total points would have been had the point systems been fixed.

I limited most of my analysis to 1980 onward, since this is when constructors were both required to have 2 drivers per event and to register for each event in a season.

Analysis of driver performance is limited to the first 50 races post-1980 for drivers with at least 50 races after that year.

I found it interesting to measure constructors by mean points per event, to remove "total events entered" as a factor when considering dominance of constructors.

## Additional comments

I think it's important to always try to answer the question "what measurement will answer this question accurately?"

In this case, one way to judge dominance of drivers and constructors was using the points allocated (there are others such as races won, laps completed etc).

There were several issues with the points as well as the scoring system changing:

1. Constructors did not participate consistently in early decades Saying a well-funded constructor scored more points simply because they had the money to enter more races is not the same as saying they were produced the best vehicles.

2. Team sizes were not fixed until later years (so total number of chances to score points varied by year, constructor and driver)

3. Drivers have careers of differing lengths and depending on the time of calculation relative to the start or end of their career, the number of events they are measured by can change. This is why it was important to do something like "first 50 races". 50 is arbtirary of course, it could be 100, or 80 and I included a parameter in the model to adjust this (though it isn't shown)
