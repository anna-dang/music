# Exploring & visualizing a playlist using Spotify and Genius APIs.

Check out my [blog](https://annadangela.medium.com/playlist-analysis-using-genius-api-d7dedaaf4b9?sk=e39b6f903590d799852a8f2f7cdf4a8f) based on this analysis.

In this repo, we will explore how to use the Spotify API to gather playlist data. Then we will analyze the songs in the playlist for music feature scores and plot as a radar graph.
<img alt="radar plot of playlist music features" src="./images/radar.png" width="600"/>

We will then use the Genius API to gather lyric data for the each song and run a quick sentiment analysis of the playlist using VADER.
<img alt="bar chart comparing vader scores per song" src="./images/vader_scores.png" width="600"/>

To rank the overall sentiment of the playlist, I chose to examine both an average of the compound scores : 0.227; and the sum of positive/negative scores : 3.451 vs 3.044, respectively. This playlist is pretty balanced but skews slightly positive. For a real analysis, other rule based metrics should be explored to standardize ranking, but for a toy project I am satisfied with this visual.