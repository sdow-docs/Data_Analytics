<b>Project Analysis</b>
Dataset selected: (https://www.kaggle.com/datasets/mahdimashayekhi/social-media-vs-productivity)

<b>Purpose</b>
I selected this dataset because I was curious to know if all the hype about social media affecting productivity was true. I know that my sister is very concerned about screen time and finds ways to limit their social media usage, including blocking some features.

<b>Cleaning</b>
This was a large dataset to work with. In the initial look into it, there were 30,000 rows of data and over 2,000 were missing at least on value in a column.
The first thing I did was to drop all the rows that were missing data.
I then checked for duplicates but I figured there wouldn't be as this dataset did not have a single column with unique values in it. The df.duplicated().sum() came back with a 0 confirming my thoughts.

<b>Manipulation</b>
Once the cleaning was done, I was still left with a large dataset. I decided to only use a p






