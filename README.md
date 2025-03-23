# Shopify-App-Analysis-Success-Drivers-in-the-App-Marketplace-Power-BI-
📊 Part 1: App Landscape Overview

Using the apps table, I developed key visualizations to understand the Shopify App Store ecosystem:

KPI Card: Displayed the total number of unique apps in the marketplace.

Trend Analysis: A line chart showing the volume of reviews over time, based on the lastmod field, to reveal engagement trends.

Performance Distribution: A scatterplot of review count vs. average rating, highlighting how volume of feedback correlates (or doesn’t) with perceived quality. Text annotations were added to interpret trends and outliers.

📝 Part 2: Review Metrics & Developer Engagement

With a focus on review sentiment and developer responsiveness:

Created a new DAX column, helpful_reviews = rating * (1 + helpful_count), to weight ratings by their perceived helpfulness. A KPI card was used to display the average helpful review score.

Introduced a binary DAX column, developer_answered, to flag reviews with a developer response.

Built a scatterplot comparing average ratings based on whether a developer replied, providing insight into how responsiveness may influence user satisfaction.

🔍 Part 3: Developer-Level Review Insights

By establishing a many-to-one relationship between reviews and apps via app_id, I was able to perform deeper analysis at the developer level:

Total Ratings by Developer: A bar chart showed the total rating volume per developer, though this metric alone proved to be misleading due to rating distribution.

Weighted Satisfaction: A more accurate bar chart used average helpful_reviews to better assess developer performance in context.

Responsiveness Analysis: Visualized the percentage of developer responses using the developer_answered field, filtered to only include developers with 500+ reviews, identifying top performers in customer engagement.

💡 Key Skills Demonstrated

Data modeling (relationships, DAX calculations)

Insightful visual storytelling with Power BI

Root cause analysis using weighted metrics

UX-focused dashboard design for executive audiences

This project highlights my ability to work with multi-table datasets, build effective data models, and surface meaningful insights through clean, interactive visuals.
