# MSCS_634_Lab_6
## Association Rule Mining Lab – Netflix Titles Dataset
# Purpose of the Lab

This lab explores association rule mining techniques using the Apriori and FP-Growth algorithms to uncover hidden relationships within the Netflix Titles dataset. Although the dataset does not contain traditional transactional purchase records, the listed_in field—which includes genres assigned to each movie or TV show—was transformed into transaction-style data. This allowed the application of frequent itemset mining and association rule analysis. The goal of the lab was to understand how data preprocessing, frequent itemset mining, and rule extraction can reveal meaningful co-occurrences and patterns that support decision-making in recommendation systems and content analysis.

# Key Insights From the Analysis

The analysis produced several interesting insights into the distribution and relationships of Netflix genres. Genres such as Documentaries, International TV Shows, TV Dramas, and Crime TV Shows appeared frequently, reflecting content trends within the platform. Both Apriori and FP-Growth generated 19 frequent itemsets at a minimum support threshold of 5%, confirming similar stability in results. Association rules identified strong relationships, such as Independent Movies → Dramas, with high confidence and lift values, illustrating how certain genres consistently co-occur. Additionally, TV Dramas → International TV Shows demonstrated strong lift, highlighting how certain themes are globally consistent.

# Challenges and Decisions

A primary challenge was adapting the dataset into a transactional format suitable for association rule mining. Since the dataset is not naturally transactional, the listed_in field was cleaned, split, and transformed into genre lists to represent “items” per transaction. Another challenge was determining appropriate support thresholds, as overly strict values reduced results while overly lenient thresholds produced excessive noise. The decision to use visualization tools such as Seaborn improved interpretability and helped highlight genre frequency and rule strength. FP-Growth proved more efficient, though both algorithms produced comparable insights.
