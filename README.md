# Piki Music Dataset

We collect explicit ratings while incentivizing users to provide feedback in a way that is aligned with their individual tastes. The columns of the dataset are as following:

- timestamp: a datetime variable
- user_id: an anonymized user id
- song_id: an anonymized song id
- liked: this is the trinary indicator, 0 if the song is disliked, 1 if the song is liked, or 2 if the song is superliked. 
- personalized: this is 1 if the song was recommended based on their previous choices or 0 if the song was selected randomly. 
- spotify_popularity: this is the song's artist's popularity, a value between 0 and 100, with 100 being the most popular. It is published by Spotify for each artist, through their publicly-available API(https://developer.spotify.com/documentation/web-api/reference/#category-artists). 
