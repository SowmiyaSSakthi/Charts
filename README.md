Sprint Data Visualization with Matplotlib and Pandas

A beginner-friendly Jupyter notebook that explores 12 chart types in Python, using a small dataset of sprint metrics for three development teams. The same data is plotted in different ways to show how the choice of chart changes the story.

Dataset

A small hand-made dataset built with a Pandas DataFrame (3 rows, 6 columns):

Sprint	Task_completed	Bugs_reported	Hours_worked	Developers	Code_coverage
S1	       25	              1	            230	        Team A	     40
S2	       45	              2	            122	        Team B	     70
S3	       78	              6	            320	        Team C       90


Charts Covered

#	Chart	                           Function	                               What it shows

1	Bar chart	                       plt.bar()	                      Tasks completed per sprint
2	Line plot	                       plt.plot()	                      Task progress across sprints
3	Pie chart	                       plt.pie()	                      Share of tasks completed by each team
4	Histogram	                       plt.hist()	                      Distribution of hours worked
5	Scatter plot	                   plt.scatter()                   	Hours worked vs. tasks completed
6	Box plot	                       plt.boxplot()	                  Spread of bugs reported
7	Horizontal bar chart	           plt.barh()                     	Code coverage by team
8	Fill between	                   plt.fill_between()	              Sprint progress as a filled area
9	Stack plot                       plt.stackplot()                  Tasks vs. bugs, stacked
10	Heatmap                        plt.imshow()	                  All project metrics side by side



Requirements

Python 3.8+
pandas
matplotlib
Jupyter Notebook, JupyterLab, or Google Colab


Key Takeaways

Bar charts make it easy to compare values across categories.
Line plots show trends over time.
Scatter plots reveal whether two variables are related, such as hours worked and output.
Heatmaps give a compact overview of many metrics at once, though metrics with very different scales (hours vs. bugs) can dominate the color range.
With only three data points, some charts (histogram, box plot) are for practice rather than real insight.


Tools Used

Python
Pandas
Matplotlib
Google Colab



		
