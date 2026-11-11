<h1>Project Analysis</h1>
Dataset selected: (https://www.kaggle.com/datasets/mahdimashayekhi/social-media-vs-productivity)

<h2>Purpose</h2>  
I selected this dataset because I was curious to know if all the hype about social media affecting productivity was true. I know that my sister is very concerned about screen time and finds ways to limit their social media usage, including blocking some features.

<h2>Cleaning</h2>  
This was a large dataset to work with. In the initial look into it, there were 30,000 rows of data and over 2,000 were missing at least on value in a column.
The first thing I did was to drop all the rows that were missing data.<br>
<br>
<br>
I then checked for duplicates but I figured there wouldn't be as this dataset did not have a single column with unique values in it. The df.duplicated().sum() came back with a 0 confirming my thoughts.
<br>
<h2>Manipulation</h2>  
Once the cleaning was done, I was still left with a large dataset. I decided to only use a 5% sampling of the dataset. I also created a new age_group column for the different ages.

<h2>Data Visualization</h2>  
To make my visualizations my own, I defined a color pallet for gender for use in my scatterplot, specified the "crest" color pallet for my bar chart, and specified the "BuPu" cmap pallet for the heatmap.<br>
<br>
The first visualization I selected is a scatterplot comparing screen time before bed and the number of hours slept. I chose to highlight by gender.<br>
<br>
<img width="680" height="455" alt="image" src="https://github.com/user-attachments/assets/c301c49c-bd69-4ba7-aa37-87bff8072470" /><br>
<br>
<br>
The second visualization I selected is a bar chart comparing the perceived productivity and the actual productivity for the different age groups.  <br>
<br>
<img width="824" height="455" alt="image" src="https://github.com/user-attachments/assets/d372190b-8ff7-4589-a934-2a1247aeab97" /><br>
<br>
<br>
The last visualization I selected is a heatmap looking for correlations between coffee consumption per day, stress level, daily social media time, and number of days feeling burned out in a month.<br>
<br>
<img width="643" height="591" alt="image" src="https://github.com/user-attachments/assets/4e4f2b5d-9328-464c-bd5b-b3aa449dd393" /><br>
<br>
<br>
<h2>Statistical Analysis</h2>
I ran "df.info()" several times to learn more about this dataset (null values, size, etc.). <br>
<br>
I also generated descriptive statistics. From the descriptive statistics I was able to see the min and max age in the dataset and I used those values when creating my age groups.<br>
<br>
age	daily_social_media_time	number_of_notifications	work_hours_per_day	perceived_productivity_score	actual_productivity_score	stress_level	sleep_hours	screen_time_before_sleep	breaks_during_work	coffee_consumption_per_day	days_feeling_burnout_per_month	weekly_offline_hours	job_satisfaction_score
count	854.000000	854.000000	854.000000	854.000000	854.000000	854.000000	854.000000	854.000000	854.000000	854.000000	854.000000	854.000000	854.000000	854.000000
mean	41.776347	3.214347	60.442623	6.989194	5.517646	4.933323	5.469555	6.498326	1.017053	5.052693	1.948478	15.930913	10.474655	4.927475
std	13.821093	2.203382	7.770800	1.986666	2.039795	1.914641	2.848810	1.460126	0.650146	3.226616	1.410783	9.199809	7.218914	2.130617
min	18.000000	0.000000	39.000000	0.000000	2.001756	0.713488	1.000000	3.000000	0.000000	0.000000	0.000000	0.000000	0.000000	0.000000
25%	30.000000	1.808446	56.000000	5.680571	3.661517	3.313862	3.000000	5.462022	0.532369	2.000000	1.000000	8.000000	4.671126	3.265969
50%	42.000000	3.078964	60.000000	6.956217	5.558436	4.911378	5.000000	6.491128	0.982382	5.000000	2.000000	16.000000	9.987798	5.044289
75%	53.000000	4.346789	65.000000	8.330446	7.311469	6.601171	8.000000	7.550985	1.455804	8.000000	3.000000	24.000000	15.424462	6.534930
max	65.000000	17.817948	89.000000	12.000000	8.998854	8.800745	10.000000	10.000000	3.000000	10.000000	6.000000	31.000000	36.359084	10.000000
<br>
<h3>Chart Analysis</h3>
I was surprised by the findings from my visualizations.<br>
<br>
<b>Scatterplot</b> <br>
The trendline for the scatterplot is almost level. This would indicate that there is not a correlation between the screen time and amount of sleep. As only 5% of the database was sampled, this is not a definitive answer. I had rerun this with a 1.5% sampling and the trendline indicated a positive correlation. I think the dataset needed to be modified a bit more. For example to limit the sample to only one age range for the scatterplot.<br>
<br>
<b>Bar Chart</b><br>
This cart is very interesting. It appears that all age groups perceived they were more productive then they really were. This can hint that social media usage is taking more of their productivity time.<br>
<br>
<b>Heatmap</b><br>
This last chart also supprised me as daily social media seems to have no significant correlation to feeling burned out. It also has no linear correlation at all to stress level.
