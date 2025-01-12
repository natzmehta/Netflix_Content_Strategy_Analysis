# Netflix Content Strategy Analysis

**Background & Overview**

The Netflix Content Analysis is a comprehensive evaluation of Netflix's streaming catalog, analyzing content performance, audience preferences, and strategic distribution patterns across their global platform.

This analysis leverages Netflix's extensive content database, which includes detailed information about movies and TV shows, their performance metrics (IMDb scores, TMDb popularity), content characteristics (genres, runtime, age certifications), and geographical distribution. The data, previously underutilized, provides valuable insights into content strategy optimization and audience engagement patterns.

The project utilizes a multi-tool approach:
* Power Query and Pivot Tables for initial data cleaning and structuring
* MySQL database for complex data exploration and analysis
* Tableau for advanced visualization and insight generation

Insights and recommendations are provided on the following key areas:
1. Content Strategy Analysis: Comprehensive evaluation of Netflix's content performance across three key dimensions:
    * Viewer engagement metrics (IMDb scores 1-10 and TMDb popularity) by genre and content type
    * Content duration patterns and their correlation with audience ratings
    * Age certification distribution and its impact on content success

2. Geographic Distribution Analysis: Evaluation of production countries' contribution to Netflix's catalog, focusing on regional content performance and market penetration patterns

3. Quality Metrics Assessment: Deep dive into the relationship between IMDb scores (1-10) and TMDb popularity metrics, identifying success factors across different content categories

The analysis is based on Netflix's content catalog data of releases from 1945 - 2022, examining movies and TV shows across multiple decades, with particular focus on viewer ratings, engagement metrics, and content characteristics.

Before beginning the analysis, several quality control measures were implemented, details can be found in the Titles.xlsx file  The SQL queries used to prepare the data for the dashboard as well as the targeted SQL queries regarding various business questions can be found [here](https://github.com/natzmehta/Netflix_Content_Strategy_Analysis/blob/main/SQL_Netflix_Data_Analysis.sql)


<br><br>

**Data Structure Overview**

The Netflix content database consists of the following tables with a total row count consisting of 5851 unique titles including movies and tv shows - 

![image](https://github.com/user-attachments/assets/0397ddc8-0494-4931-9db1-1235ba120ca6) 

<br><br>

**Executive Summary**

Overview of Findings:

After peaking in the later half of the 1900s, with content from the 1960s-1970s achieving some of the highest average ratings -  peaks reaching above 8.0, the IMDB score has since seen a notable downward trend visible from the 1990s to 2021. Recent content (2010-2021) consistently averages below 7 and the variance in scores has decreased over time, suggesting more standardized content quality. 

Some key considerations behind this trend could be:
* Survivorship bias: Older content that survived tends to be of higher quality
* Rating dynamics: Recent content often experiences rating fluctuations as more diverse audiences provide reviews
* Volume effect: The significant increase in content production in recent decades has led to more variation in quality

 This trend analysis provides a strong foundation for examining Netflix's content strategy and quality metrics across different eras. The declining trend raises important questions about content diversification and quality maintenance in the streaming era.

Below is the overview page from the Tableau dashboard with a deeper analysis included in the report.

![image](https://github.com/user-attachments/assets/eaef25f6-14b6-4f20-afe4-81a74036c398)

<br><br>

Insights Deep Dive:


Content Strategy - 

- Netflix's content catalog shows a clear split: 65% movies versus 35% TV shows. This distribution largely stems from historical production patterns, where movies dominated the entertainment industry (Movies have 35% more IMDB votes compared to TV shows) for decades before TV shows gained comparable production volume in the early 2000s
- While Netflix's larger movie catalog offers broader genre coverage and diverse viewing options, TV shows tend to drive longer viewer engagement due to their multi-episode format. This is reflected in their higher average IMDb score of 6.9, compared to 6.6 for movies
- Documentaries boast the highest average IMDb score of 6.9, while Rom-Coms have the lowest at 5.9. Although Comedy has the highest number of titles, it maintains a relatively lower score. Meanwhile, Drama-Comedy achieves a strong average score of 6.95 but with only 109 titles, offering valuable insights into where production resources could be strategically allocated
- Both movies and TV shows exhibit a positive correlation between runtime and IMDb scores. Although TV shows generally outperform movies in average IMDb ratings, movies remain the more popular choice, garnering a total of 91 million IMDb votes



![image](https://github.com/user-attachments/assets/6ed0a0cf-46cf-436a-9351-12bfb6b085a5) 

<br><br>

Geographical Analysis - 

- U.S. produces the majority of Netflix's movies, accounting for 36%, followed by India at 10%. However, countries like Japan (JP), South Korea (KR), and Spain (ES), while not among the top contributors, are highly favored by audiences based on their popularity

![Primary Country](https://github.com/user-attachments/assets/a44b70d9-19a0-4cd4-a912-cc54f22e8d40) 

<br><br>

Quality metrics - 
- While movies have traditionally been the dominant form of entertainment, TV shows have surpassed them in performance and preference; they tend to achieve higher TMDb popularity scores compared to movies at equivalent IMDb ratings
- Higher IMDb scores (7.5-10.0) demonstrate a strong correlation with increased TMDb popularity, indicating that quality content significantly drives viewer engagement.
- The majority of content clusters between IMDb scores of 5.0-8.0, with significantly fewer titles at the extreme high or low ends of the rating spectrum

![image](https://github.com/user-attachments/assets/40ea7af2-0256-4101-8363-20a54cfa21e5)


<br><br>

Recommendations:

* Increase TV show production given their higher engagement and IMDb scores; focus on multi-season series development, particularly in high-performing genres
* Expand Drama-Comedy content given its high average score (6.95) and current limited catalog while reducing investment in Comedy & Rom-Coms unless significant quality improvements can be achieved
* Maintain strong U.S. production base while diversifying into emerging markets - increase content production in high-performing markets like Japan, South Korea, and Spain
* Shift 15-20% of movie production budget to TV show development and consider mini-series formats that blend movie production quality with TV show engagement while building stronger partnerships with tv show creators



