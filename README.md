# Recommender-System
To explore various recommender algorithms available and to develop the new customizable model using LSTM.

There are varieties of recommendation systems available and below are the two primary types:
1. Collaborative Filtering, and
2. Content Based Filtering

Here, we will be leveraging RecBole libraries to explore various models and to develop more customizable one.

Ref: https://recbole.io/

1. Last.fm, Description: Sequential music listening data.


user_id    item_id       timestamp
1          song_1001     2021-01-01 08:00:00
1          song_1002     2021-01-01 08:15:00
2          song_1050     2021-01-02 09:45:00
2          song_1060     2021-01-02 10:00:00

3. Spotify Million Playlist Dataset
Description: Playlist-based data where each user creates a sequence of tracks.
plaintext
Copy code
user_id    playlist_id   item_id     timestamp
1          playlist_1    track_201   2021-03-01 12:30:00
1          playlist_1    track_202   2021-03-01 12:35:00
2          playlist_5    track_210   2021-03-02 15:00:00
2          playlist_5    track_211   2021-03-02 15:05:00
   
5. Foursquare Check-in Dataset
Description: Location check-ins with sequential timestamps.
plaintext
Copy code
user_id    location_id   timestamp
1          loc_3001      2021-02-01 14:00:00
1          loc_3002      2021-02-01 15:20:00
2          loc_3010      2021-02-03 10:15:00
3          loc_3025      2021-02-04 18:30:00

