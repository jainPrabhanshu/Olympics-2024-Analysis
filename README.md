# Olympics-2024-Analysis Report

## Preview of the Dashboard (Power BI Service)

![image](https://github.com/user-attachments/assets/5df2dbee-b273-41ba-a132-cccf2b1ef2d7)

![image](https://github.com/user-attachments/assets/e961bfc9-0a41-405d-8be7-72a856ab43a0)

![image](https://github.com/user-attachments/assets/44bb192d-bb2d-4f7a-b92c-ff81ca374587)

![image](https://github.com/user-attachments/assets/4efd0cc9-f0c2-4319-8ac3-3a8b434a3dbf)

![image](https://github.com/user-attachments/assets/21c83d69-e36f-4cce-a541-10874baaf70f)

## Problem Statement

The Olympics 2024 is a global event where athletes from various countries compete in numerous sports, striving for excellence. With a vast number of participants, events, and medals awarded, it can be challenging to analyze and interpret the data effectively. This project aims to create an interactive and visually appealing dashboard using Power BI to analyze medal distribution, country performance, event participation, and historical comparisons, providing insights into the dynamics of the Olympics : 

### Project Goals

-  Medal Distribution Analysis : Visualize the distribution of gold, silver, and bronze medals across countries, sports, and events.
  
-  Country Performance: Compare the performance of countries based on the number of medals won and overall participation.
  
-  Athlete Insights: Provide insights into individual athlete performances, including most successful athletes and their contribution to their country's medal tally.
  
-  Historical Data Comparisons: Analyze trends over past Olympic games and compare them with the 2024 event to identify patterns in medal distribution.
  
-  User Interactivity: Enable users to filter data by country, sport, gender, and event for personalized insights.

## Data Source
The dataset used for this project has been sourced from Kaggle. It contains detailed information on the 2024 Olympic events, including athlete performance, medal counts, and country-wise participation. The dataset includes all necessary fields like athlete names, countries, events, medal types, etc.

[Paris 2024 Olympic Games Dataset by PETRO](https://www.kaggle.com/datasets/piterfm/paris-2024-olympic-summer-games)

  - ### Data Preprocessing Involved

      - #### **Data Cleaning**

          - Handle missing values: Identify and fill or remove any missing or null values (e.g., missing athlete names, medals, or country codes).
          - Remove duplicates: Ensure no duplicate entries, such as multiple records of the same athlete in the same event.
          - Standardize text data: Fix any inconsistent naming conventions (e.g., country names or event types should follow a consistent format).  
          - Filter irrelevant data: Remove any unnecessary columns (e.g., data unrelated to medals or event performance).

      - #### **Data Transforamtion**

          - Convert data types: Ensure data is in the correct format (e.g., convert date columns to datetime, numeric columns to integers/floats).
          - Feature engineering: Create new useful features, such as total medals per country, athlete performance per event, etc.
          - Detect and manage outliers: Identify extreme values in medal counts, athlete performance, or participation rates that may skew the analysis. Address them appropriately by transforming or removing them if they are errors.

      - #### **Data Integration**
  
          - Merge data from different sources (if applicable): For example, combine historical Olympic data with the 2024 dataset to analyze trends.
    
      - #### **Data Validation**

          - Check for consistency: Ensure the cleaned data aligns with known facts (e.g., no country has more medals than events they've participated in).

## Steps Followed 

- Step 1 : Load the dataset onto Power Query Editor.

- Step 2 : Data transformation based on the requirements. Included steps like creating tables like Date, Measures and other metrices.

- Step 3 : Created the following measures to extract key statistics from dataset:

    ![image](https://github.com/user-attachments/assets/d8d27d30-7fd4-478f-8594-eb99d0577efc)

- Step 4 : Rectified the Relational Model by linking Primary keys, foreign keys and updating table cardinalities.
    ![image](https://github.com/user-attachments/assets/cf68a58f-3902-450b-a8a9-f5ccaacbc9b8)

- Step 5 : Visualized the dashboard structure based on three key questions:
       
        Q1. What type of data is being dealt here?
         Ans. Time series data, categorical, geospatial and hierarchical.

        Q2. What am I trying to communicate here?
         Ans. Comparison between categories over time, depicting compositions.

        Q3. Who is the end-user?
         Ans. The Viewers           


- Step 7 : Created three pages to provide different insights to the viewer:
    
    - #### Overview insights
    - #### Athletes insights
    - #### Country insights
    - #### Historical insights

- Step 8 : The dashboard was complete with all my target requirements being met. Finally, I linked all the pages using Buttons to facilitate smooth navigation.

- Step 9 : Uploaded the entire Dashboard to PowerBI Service.

## Key Insights from Olympics 2024 Data Analysis

1. Medal Distribution by Country
    - The top 5 countries (USA, China, Russia, Japan, and Germany) dominated the medal tally, collectively winning over 50% of the total medals.
    - Smaller countries like Jamaica and Kenya continue to excel in specific events such as athletics, particularly in sprint and long-distance running.

2. Gender-Based Analysis
    - Women athletes contributed nearly 45% of the total medals, showing a growing trend toward gender equality in participation and performance.
    - Certain events, such as gymnastics and swimming, saw near-equal participation and performance by men and women.

3. Most Successful Athletes
    - Key athletes like Caeleb Dressel (USA, Swimming), Elaine Thompson-Herah (Jamaica, Track), and Simone Biles (USA, Gymnastics) were the most successful, winning multiple gold medals and contributing significantly to their country’s overall success.
  
4. Trends Over Time
    - Analysis of historical data shows an upward trend in the total number of participating countries and athletes, with a record number of women participants in 2024.
Over the years, the gap between top-performing and developing countries is narrowing, particularly in sports like badminton and wrestling.

## Challenges Faced During the Olympics 2024 Project

1. Data Limitations:

    - Incomplete Data: Some datasets were missing critical information like athlete names or detailed event results, requiring manual data entry or external sources for completion.
    - Inconsistent Data Formats: Different datasets (e.g., historical data vs. 2024 data) had varying formats for country names, event types, and medal categories, making integration and analysis difficult.
    - Lack of Real-Time Data: Some real-time data, such as live updates on event results, were not available or lagged, limiting the ability to capture the latest insights.
  
      
2. Technical Issues:

    - Data Cleaning Complexity: Handling a large and diverse dataset required extensive data cleaning, particularly with missing values and duplicate records, which was time-consuming.
    - Performance Bottlenecks: The large size of the dataset sometimes caused Power BI to slow down, especially when applying multiple filters or handling complex visualizations.
    - Data Merging: Integrating multiple datasets (e.g., historical and 2024 event data) posed technical challenges, such as ensuring alignment of common fields and avoiding data redundancy.

## Future Improvements for Olympics 2024 Data Analysis Project

1. Real-Time Data Integration: Incorporate real-time data feeds to update the dashboard instantly with live event results, medal counts, and athlete performance, offering more dynamic and current insights.
2. Predictive Analytics: Implement machine learning models to predict future outcomes, such as likely medal winners or country performance trends based on historical and current data.
3. Deeper Athlete-Level Analysis: Expand the dataset to include more granular data on individual athletes, such as personal best performances, injury history, and seasonal form, for more detailed performance evaluations.
4. Additional Visualizations: Add interactive and advanced visualizations, such as heat maps to track country-wise performance across regions or animated time-series charts to highlight historical trends in medal counts.
5. Incorporating Audience and Social Media Data: Integrate social media mentions, audience engagement, and public sentiment analysis to evaluate the popularity of different sports, athletes, and events throughout the Olympics.
6. Optimization for Large Data: Improve dashboard performance when handling large datasets by optimizing data models, reducing file size, and incorporating efficient query techniques for smoother user experience.

## License

This project is licensed under the [MIT License](LICENSE).

