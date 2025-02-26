# [EDA]-Exploratory Data Analysis: Marathon Trends with Pandas [Python] 

## Project Overview
This project examines marathon trends by looking into **Exploratory Data Analysis (EDA)** to reveal insights from historical race data. The main objective is to examine **participation growth, performance trends, demographic patterns, and external factors like weather and course difficulty**.

## Key Insights
- **Participation Growth:** Marathon popularity has grown, particularly among amateur and women runners.
- **Performance Trends:** Winning times have become better thanks to **advances in training and technology**.
- **External Factors:** Weather conditions and course elevation play a major role in affecting finish times.

## Business Relevance 
- **Race Organizers:** Maximize event logistics and scheduling according to past participation trends.
- **Sponsors & Marketers:** Target audiences based on demographic shifts and engagement trends.

## Example Code Snippets
### Load and Inspect Data
```python
import pandas as pd
df = pd.read_csv("marathon_data.csv")
print(df.head())
```

### Analyze Performance Trends
```python
performance_trends = df.groupby("Year")["Winning Time"].mean()
print(performance_trends.tail(10))
```

### Impact of Weather on Finish Times
```python
import matplotlib.pyplot as plt
df.plot.scatter(x="Temperature", y="Winning Time", title="Temperature vs Winning Time")
plt.xlabel("Temperature (°F)")
plt.ylabel("Winning Time (minutes)")
plt.show()
```

## To conclude 
This EDA looks into key trends **marathon trends and performance-affecting factors** to offer practical guidance for **race organizers, runners, and sponsors**. 
The main takeaway of this project is that there is a seasonality to these average finish times, with summer marathons averaging the slowest (6.87 hours) and fall marathons averaginq the fastest (7.40 hours) during this period. This indicates that seasonal and weather conditions significantly influence runner performance and informs race planning and training schemes for best results.

