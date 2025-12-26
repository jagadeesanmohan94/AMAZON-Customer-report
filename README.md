# AMAZON-Customer-Python Report

Dashboard Link: 

Amazon_Customer_Analysis.ipynb.

🧩 Overall Summary for Portfolio
🎯 What this analysis tells us


Review Activity is Highly Uneven

A small percentage of reviewers account for the majority of reviews (power–user pattern).

![2](https://github.com/user-attachments/assets/e9f6b8c4-cc52-4840-aa4e-93189a828808)


Ratings are Strongly Skewed Positive

5-star ratings dominate across both small and large datasets.
Suggests satisfaction but also hints at possible bias.



Top Reviewers Have Significant Influence

These users can shape product perception.
Useful to monitor for authenticity.



Product Performance Varies by Rating Mix

Some products perform exceptionally well.
Others show mixed ratings — indicating quality or expectation issues.



Business Value

Identify top-performing products
Detect potential review manipulation
Improve customer experience
Prioritize products for marketing or improvement




🔍 1. Reviewer Frequency Analysis
📌 Visuals: Boxplots of Frequent vs Non‑Frequent Reviewers
These two boxplots compare the number of reviews made by:

Frequent reviewers (users who post reviews often)
Non‑frequent reviewers (occasionally active users)

![Image](https://github.com/user-attachments/assets/304b8730-906a-4cba-b933-8ff2f28958c1)

🔎 Key Observations:

Frequent reviewers show a much higher median review count, indicating they contribute heavily to the dataset.
There are many outliers above 300+ reviews, showing a small subset of users posting reviews at scale.
Non-frequent reviewers show a small median and tighter spread — most users submit only a few reviews.

🧠 Interpretation:
This pattern reflects a Power Law (80/20 rule) where:

A small group of power users generates a large portion of all reviews.
This is common in online platforms — a few users are highly active while the majority are passive.

This insight is useful for:

Reviewer fraud detection
Identifying brand enthusiasts
Loyalty program targeting

![Image](https://github.com/user-attachments/assets/16406422-be0f-491b-b203-bf8125eb0452)

⭐ 2. Rating Distribution by Score (Small Sample)
📌 Visual: Bar chart showing counts of scores 1–5
🔎 Key Observations:

5-star reviews dominate (highest bar with ~5765 reviews)
Ratings decline progressively from 4 → 1
Very few negative reviews (1- and 2-star)

🧠 Interpretation:
This is typical of online review systems, where:

Satisfied customers are more likely to leave ratings
High average ratings often reflect product popularity or confirmation bias

Good for:

Customer sentiment snapshot
Understanding sampling bias


👥 3. Top Reviewers by Review Count
📌 Visual: Bar chart of top 10 reviewers
🔎 Key Observations:

![Image](https://github.com/user-attachments/assets/d0a408a5-005f-4202-a45c-fb245cb1e16a)

The top reviewer (AY12DBB0U420B) has over 325 reviews
Other reviewers also show high counts (200–300+)

🧠 Interpretation:

Strong presence of high-frequency reviewers
The review ecosystem is user-concentrated — most reviews come from a minority
Useful for influencer tracking, spam detection, or user segmentation


⭐ 4. Rating Distribution on Full Dataset (Large Sample)
📌 Visual: Large bar chart with scores 1–5 showing very high counts
🔎 Key Observations:

![Image](https://github.com/user-attachments/assets/97b240c4-a851-4314-bba9-d88764e729e3)

Again, 5-star reviews overwhelmingly dominate (~250,000 reviews)
4-star and 3-star follow next
Similar pattern as the smaller sample, but on a much larger scale

🧠 Interpretation:

Confirms the same positive skew in ratings
Could indicate:

High product quality
Reviewer positivity bias
Possible incentivized reviews (in some marketplaces)


![Image](https://github.com/user-attachments/assets/e747d620-5754-48de-aba4-b98b6bb52e68)

📦 5. Product-wise Rating Distribution
📌 Visual: Horizontal bar chart by Product ID × Score
🔎 Key Observations:

Some products (e.g., B002QWPB9S, B000UBD88A) receive very high volumes of 5-star reviews
Others have more balanced or even lower-score distributions
Score 5 dominates across most products, but variations exist between products

🧠 Interpretation:

Helps identify best-performing products
Shows which products generate polarized vs consistent reviews
Useful for:

Product quality assessment
Category managers
Customer experience teams
