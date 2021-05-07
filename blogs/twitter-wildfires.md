---
layout: page
title: Twitter Spatial Analysis Techniques
---

In their analysis of Twitter activity related to wildfires in California, Wang et al. use four broad analysis techniques: text mining, kernel density analysis, content analysis, and network analysis. They use text mining to gather and clean Tweets, and present summary statistics describing their input data in tables and a map showing the location and frequency of wildfire-related tweets in their study area. Their kernel density analysis consists of analyzing the spatial distribution of wildfire tweets by comparing kernel density of wildfire-related tweets to population kernel density, and is presented in a heat map. They use further cleaning and filtering by keywords to prepare the data for content and network analysis by removing stop words and consolidating duplicate words, and from this calculate the frequency of key terms and group terms into clusters, presenting the results in a histogram and table. For their network analysis, the authors construct a graph where each node represents a user and directed edges represent information flow through retweets. They calculate the cumulative distribution of the indegree and outdegree of this graph, and represent these results in charts.

This study contains many aspects of reproducible research, but has several key shortcomings that might hinder reproduction. The spatial and temporal context of the analysis is well defined, as are the keywords and parameters used to select and filter the raw data. However, the authors do not define well how they clean and consolidate the content of the tweets, they do not give detailed information about how kernel density or content clusters are calculated, and the domain of the input data (i.e. which subset of the raw data) used to create some of the final charts is ambiguous. If these issues with reproduction were resolved, I believe this paper would lend itself to replication in other regions or time periods, since most of the results that the authors report are fairly general and could be easily compared across space and time. Most of the findings are defined in terms of the relative spatial, temporal, and social distributions of the data rather than place-specific attributes (i.e. "there is more tweet activity close to wildfires" or "local news and government organizations are hubs of information networks in disaster situations"), attributes that are relatively easy to compare in different places and times. 

References:
Wang, Z., Ye, X. & Tsou, MH. Spatial, temporal, and content analysis of Twitter for wildfire hazards. Nat Hazards 83, 523–540 (2016). https://doi.org/10.1007/s11069-016-2329-6