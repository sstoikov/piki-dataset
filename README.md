# Piki Music Dataset

We collect explicit ratings while incentivizing users to provide feedback in a way that is aligned with their individual tastes. The columns of the dataset are as following:

- timestamp: a datetime variable
- user_id: an anonymized user id
- song_id: an anonymized song id
- liked: this is the trinary indicator, 0 if the song is disliked, 1 if the song is liked, or 2 if the song is superliked. 
- personalized: this is 1 if the song was recommended based on their previous choices or 0 if the song was selected randomly. 
- spotify_popularity: this is the song's artist's popularity, a value between 0 and 100, with 100 being the most popular. It is published by Spotify for each artist, through their publicly-available API(https://developer.spotify.com/documentation/web-api/reference/#category-artists). 
- treatment_group: the amount of time needed to unlock the like button. 1 if the timer is 3 seconds, 2 if the timer is 6 seconds, 3 if the timer is 9 seconds.

In an effort to mitigate ratings inflation and incentivize ratings in line with a user's true opinions, Piki implemented a set of timers on each of the ratings options on February 21, 2021. 
Since then, users have not been able to \textit{immediately} rate a song after it begins playing. 
Instead, each of the ``dislike,'' ``like'' and ``super-like'' buttons appear sequentially in that order, several seconds after the song begins playing or the previous button appears. 

During the period of August 19, 2022 to December 5, 2022, a randomized controlled trial was performed, where the amount of time needed to unlock the like button was changed. Treatment groups had timers of 3, 6, and 9 seconds.
