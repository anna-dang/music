# Exploring & visualizing a playlist using Spotify and Genius APIs

Check out my [blog](https://annadangela.medium.com/playlist-analysis-using-genius-api-d7dedaaf4b9?sk=e39b6f903590d799852a8f2f7cdf4a8f) based on this analysis.

In this repo, I explore how to use the Spotify API to retrive playlist data. I analyzed the playlist via specific music feature scores that Spotify tracks per song. To visualize the overall playlist, I have plotted the composite scores as a radar graph.

<img alt="radar plot of playlist music features" src="./images/radar.png" width="600"/>

To produce a sentiment rating for the playlist, I analyzed the lyrics of the songs. I gathered the lyrics using the Genius API and scored the sentiment using VADER.

<img alt="bar chart comparing vader scores per song" src="./images/vader_scores.png" width="600"/>

To rank the overall sentiment of the playlist, I chose to examine both an average of the compound scores : 0.227; and the sum of positive/negative scores : 3.451 vs 3.044, respectively. This playlist is pretty balanced but skews slightly positive. For a real analysis, other rule based metrics should be explored to standardize ranking, but for a toy project I am satisfied with this visual.
