<!DOCTYPE html>
<html lang="en">
<head>
</head>
<body>
    <div class="container">
    <h1>UK Accident Data Analysis</h1>

<h2>Overview</h2>
<p>This project involves analyzing UK accident data to understand the patterns and factors influencing road accidents. The dataset includes detailed records of accidents, including the severity, number of casualties, and various environmental and situational conditions. The analysis focuses on identifying trends and correlations to draw insights into accident occurrences.</p>

<h2>Steps Involved</h2>
<ol>
    <li><strong>Data Import:</strong> Load the dataset from a CSV file and examine its structure.</li>
    <li><strong>Data Preprocessing:</strong> Handle missing values by filling them with logical defaults and preprocess the data for analysis.</li>
    <li><strong>Data Analysis:</strong> Perform exploratory data analysis to identify patterns and trends, such as the number of casualties on different days of the week.</li>
    <li><strong>Data Visualization:</strong> Create visualizations to represent the data, such as bar plots showing the number of accidents per day and the maximum and minimum speed limits where accidents occurred.</li>
    <li><strong>Statistical Analysis:</strong> Use SQL queries with pandas to extract insights about speed limits and casualties across different days of the week.</li>
    <li><strong>Summary:</strong> Interpret the findings to draw conclusions and suggest improvements for future accident prevention.</li>
</ol>

<h2>Summary</h2>
<p><strong>Intuitive Findings:</strong> Intuitively, it is expected that accidents would be more frequent under poor lighting and weather conditions. For example, accidents may be higher at night when street lights are absent, and during severe weather conditions like heavy rain or snow.</p>

<p><strong>Data-Driven Insights:</strong> The correlation matrix reveals that light and weather conditions have a minimal impact on accident severity. However, the presence of street lighting appears to have a more significant effect compared to weather conditions. This suggests that accidents and their severity are higher when street lights are present compared to daytime conditions.</p>

<p><strong>Recommendations:</strong> To enhance prediction models for accident severity, it is essential to identify and remove unnecessary columns from the dataset. This helps in focusing on the most impactful features for more accurate predictions.</p>

  <h2>Insights</h2>
  <p>
      <strong>Casualty Trends:</strong> The analysis reveals trends in the number of casualties across different days of the week, highlighting the days with the highest and lowest accident rates.
  </p>
  <p>
      <strong>Speed Limit Analysis:</strong> By comparing speed limits with casualty counts, the project identifies how varying speed limits may influence the severity of accidents.
  </p>


<h2>Contributing</h2>
<p>Contributions are welcome! Please open an issue or submit a pull request for any improvements or bug fixes.</p>
</div>
</body>
</html>
