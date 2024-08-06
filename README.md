# World-Bank-Data-Analysis-in-Python

This report analyzes the World Bank Project Performance Ratings dataset, emphasizing project success and performance trends. It aims to identify opportunities for enhancing project efficiency and quality.

Purpose 
As a global financial institution aiding low and middle-income countries, the World Bank aims to alleviate poverty and promote development. Evaluating project success is crucial given the significant resources invested.

Objectives 
This analysis examines project success across regions, the impact of global practices, the correlation between bank performance and monitoring quality, trends in project sustainability over completion years, and insights from different country lending groups.

Tools
Google Colab was our primary platform for executing Python code. Google Docs and Google Presentations facilitated the creation and presentation of the report. We also used Python libraries, including Pandas for data manipulation and analysis, NumPy for numerical operations, matplotlib and seaborn for data visualization, GeoPandas for handling geospatial data, SciPy for statistical analysis, and Tabulate to format tabular data. Google Colab's AI prompting feature and ChatGPT also helped us  in optimizing and refining our code throughout the project.

ANALYSIS

Project Success Rate
To evaluate the success rates across different regions and their respective countries, we analyzed the 'Outcome' column from the dataset. Most of the performance results were converted from the rankings (Highly Satisfactory to Highly Unsatisfactory) to numerical values (6 to 1). Successes were considered as scores from 6 to 4, and failures from 3 to 1.
We calculated the success rate for each region as the percentage of total completed projects and visualized this in Figure 1.1 while Table 1.2 displays relevant summary statistics. Notably, regions like 'East Asia and Pacific' and 'Europe and Central Asia' had higher success rates, while African regions had lower success rates. Despite this, African regions accounted for nearly 40% of the total projects, as shown in Figure 1.3.
This high project count in Africa, despite lower success rates, suggests a need for more focused and region-specific interventions. A recommendation for the World Bank is to target regional projects within Africa rather than continental projects, as the latter have the lowest success rates.

Global Practice Impact
Our analysis examined how different 'Global Practice' areas impact project success across various regions. By grouping data by 'Global Practice' and 'Region' and visualizing it through bar plots and heatmaps, we identified significant trends. Practices such as 'Infrastructure, PPPs & Guarantees' and 'Finance, Competitiveness and Innovation' showed higher success rates, particularly in 'East Asia and Pacific' and 'Europe and Central Asia'. In contrast, 'Agriculture and Food' and 'Education' had lower success rates, especially in African regions.
Figure 2.1 illustrates these trends amongst the different global practices, separating what proportions each region takes up for each practice. Figure 2.2 takes it a step further and graphs the regions by their respective continents, their average outcome displayed in Table 2.3. 
The continent Africa has the lowest average numeric outcome (3.74862), whereas Oceania (4.22403) and Europe (4.19624) have higher averages. These findings suggest that some practices are more effective in certain regions, indicating the need for tailored strategies and additional support for less successful practices, particularly in Africa.

M&E Quality and Bank Performance
We explored the relationship between 'M&E Quality' and 'Bank Performance' to determine the impact of monitoring and evaluation quality on bank performance. By converting the performance ratings to numeric values, we created a box plot, Figure 3.1, to visualize this relationship. Additionally, we calculated the correlation coefficient, which yielded 0.57, indicating a moderately positive correlation as shown in Table 3.2.
Projects with 'High' M&E Quality consistently had the highest median and mean bank performance, while those with 'Negligible' M&E Quality had the lowest. This analysis emphasizes the importance of investing in high-quality monitoring and evaluation practices to achieve better project outcomes.

Final Closing Fiscal Year 
We analyzed the relationship between the 'Final Closing Fiscal Year' and project success and sustainability. The data was cleaned, and categorical ratings were converted to numeric values. Success flags were created from numeric outcome values, and the data was aggregated by 'Final Closing FY' to calculate mean values for 'Outcome Numeric', 'M&E Quality Numeric', and 'Success'.
The resulting line plot, Figure 4.1, shows trends in these metrics over time. Initially, both M&E quality and success rates were high in 2000 but declined until 2002, then improved until 2003, followed by another decline until 2005, and a subsequent increase in 2006. These trends highlight the need for ongoing efforts to stabilize and enhance project performance, with rigorous monitoring and evaluation practices playing a crucial role.

Country Lending Groups
Our study examined the trends in project performance across different 'Country Lending Groups'. We converted 'Outcome' strings to numerical values, grouped the data by 'Country Lending Group', and calculated mean 'Outcome' scores.
Table 5.1 displays these summary statistics for each group ‘Blend’, ‘IBRD’, ‘IDA’, and ‘Other’. Statistical analysis involved computing the Pearson correlation coefficient and visualizing performance distributions using box and violin plots, Figure 5.2 and Figure 5.3 respectively.
Findings indicate that the 'IDA' group shows consistent performance with lower standard deviation and higher median performance scores, while the 'IBRD' group displays higher variability. Recommendations include prioritizing the 'IDA' group for future engagements, investigating factors causing variability in the 'IBRD' group, and implementing enhanced monitoring practices to optimize project performance and strategic planning.

Recommendations 
To enhance World Bank project outcomes, focus on regional over continental projects in Africa and tailor strategies for specific 'Global Practice' areas. Invest in high-quality Monitoring and Evaluation (M&E) practices throughout the project lifecycle. Prioritize the 'IDA' lending group for its consistent performance and investigate variability in the 'IBRD' group to optimize project performance and strategic planning.

References 
Sullivan, D. (2015). NoSQL for Mere Mortals. Addison-Wesley Professional.
The World Bank. (n.d.). https://www.worldbank.org/en/about/what-we-do.prin
The World Bank. (2023, October 5). Africa Overview. https://www.worldbank.org/en/region/afr/overview
Pandas Development Team. (2008). pandas: Python Data Analysis Library. https://pandas.pydata.org/
Oliphant, T. (2006). NumPy. https://numpy.org/
Hunter, J. D. (2003). Pyplot API. https://matplotlib.org/3.5.3/api/_as_gen/matplotlib.pyplot.html
Waskom, M. (2014). Seaborn. https://seaborn.pydata.org/
GeoPandas Development Team. (2013). GeoPandas. https://geopandas.org/en/stable/
SciPy Community. (2001). SciPy Stats. https://docs.scipy.org/doc/scipy/reference/stats.html
Lopuhin, K. (2010). Tabulate. https://pypi.org/project/tabulate/
Pandas Development Team. (2008). DataFrame.replace. https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.replace.html
Hunter, J. D. (2003). Named colors. https://matplotlib.org/stable/gallery/color/named_colors.html
Practical Python for Data Science Team. (n.d.). Seaborn Palette. https://www.practicalpythonfordatascience.com/ap_seaborn_palette
Stack Overflow Community. (2011, August 16). How to set the label's size on a pie chart. https://stackoverflow.com/questions/7082345/how-to-set-the-labels-size-on-a-pie-chart
