# Marketing Optimization: MTA & MMM for Cross-Company Insights

## Overview

This project analyzes marketing strategies for five companies (Alpha Innovations, DataTech Solutions, Innovate Industries, NexGen Systems, TechCorp) using a dataset of 200,000 campaign records. It employs Mixed Marketing Modeling (MMM) and Multi-Touch Attribution (MTA) to quantify the impact of channels (Email, Facebook, Google Ads, Instagram, Website, YouTube) and campaign types (Email, Influencer, Search, Social Media) on ROI and conversions. Additional analyses include temporal trends (Jan–May 2021), cost efficiency (Cost_Per_Conversion), and campaign type performance, culminating in actionable recommendations to optimize budget allocation and marketing strategies.

## Features





* MMM: Quantifies channel and campaign type impacts on ROI using linear regression (lightweight) and proposed XGBoost, Neural Networks, and Bayesian MMM (advanced).



* MTA: Attributes conversions to channels using linear attribution (lightweight) and proposed Markov Chains, LSTMs, and SHAP (advanced).



* Temporal Analysis: Examines ROI and Conversion_Rate trends (stable at ~5.0 and ~0.08, Jan–May 2021), with proposed Prophet and LSTM forecasting.



* Cost Efficiency: Calculates Cost_Per_Conversion by company and channel.



* Campaign Type Analysis: Evaluates ROI and Conversion_Rate by campaign type.



* Recommendations: Company-specific strategies (e.g., prioritize Email for NexGen Systems, Google Ads for TechCorp) and cross-company insights.

## Dataset





* Size: 200,000 campaign records



* Columns: Campaign_ID, Company, Channel_Used, Campaign_Type, Conversion_Rate, ROI, Acquisition_Cost, Date, Clicks, Impressions, Engagement_Score, etc.



* Companies: Alpha Innovations, DataTech Solutions, Innovate Industries, NexGen Systems, TechCorp



* Channels: Email, Facebook, Google Ads, Instagram, Website, YouTube



* Campaign Types: Email, Influencer, Search, Social Media, etc.

Usage





Data Preparation:





Clean Acquisition_Cost (remove '$', convert to numeric, handle missing values).



Calculate Conversions = Conversion_Rate * Clicks.



Run Analyses:





MMM: Run mmm_refined.py for lightweight results or advanced_algorithms/xgboost_mmm.py for advanced modeling.



MTA: Run mta_visualization.py for linear attribution or markov_mta_debug.py for Markov Chains.



Temporal: Run temporal_refined.py for trends or advanced_algorithms/prophet_forecast.py for forecasting.



Cost Efficiency: Run cost_efficiency.py to analyze Cost_Per_Conversion.



Campaign Type: Run campaign_type_analysis.py for campaign type performance.



Visualizations:





Stacked bar charts for MTA (channel contributions per company).



Bar charts for MMM feature importance and cost efficiency.



Line plots for temporal trends (ROI, Conversion_Rate).



Recommendations:





See recommendations.md for detailed company-specific strategies based on MMM, MTA, temporal, and cost efficiency analyses.

Key Findings





Alpha Innovations: Scale YouTube and Influencer campaigns; reduce Google Ads and Instagram.



DataTech Solutions: Optimize Website and Facebook; reassess campaign types (e.g., test Brand).



Innovate Industries: Reinforce Email and YouTube; explore Brand campaigns.



NexGen Systems: Balance Email (high conversions) and Search (high ROI); scale Facebook and Google Ads.



TechCorp: Prioritize Facebook, Instagram, and Google Ads; focus on Influencer and Search campaigns.

