# Spotify-Analysis-Azerbaijani-Retro-Hits
**Data Collection with an API &amp; Getting Insights**

To gather data from the Spotify API, you must first understand what data is available and the format in which it is provided. You can find all the details from [https://developer.spotify.com/documentation/web-api].

Follow the steps below to sign up for API access and start collecting data:

Register for a Spotify Developer account on [https://developer.spotify.com/].
Navigate to "Create an App" to obtain your Client ID and Client Secret.

The access token you obtain is essential for authenticating and authorizing future requests to the Spotify API. Without it, your application won’t be able to interact with Spotify’s data and services using the Client Credentials flow. This flow is designed for server-to-server interactions without requiring user authorization, making it ideal for accessing publicly available information like music data and playlists.  

Next, install Spotify’s official Python API, Spotipy. You can do this in your Python environment by running the following command in your terminal or command prompt:  

**pip install spotipy**

Then  I have written a Python function to extract detailed information about each track in Azerbaijani Retro hits playlist.
To obtain the playlist ID of any Spotify playlist, simply copy its link. Below is a guide on how to extract the playlist ID from the playlist URL:

[https://open.spotify.com/playlist/1YQzSpN1WqojjGtVgZK41E]  -->  inside URL characters after "playlist/" are
playlist ID : **1YQzSpN1WqojjGtVgZK41E**

Towards the end of the code, several data transformations are applied. The 'Duration (ms)' column is converted into 'Duration (minutes)' for better readability. The release year is extracted from the 'Release Date' column to facilitate analysis. Tracks are then categorized into different length groups, such as 'Short,' 'Medium,' 'Long,' and 'Very Long,' based on their duration. Similarly, energy levels are classified into 'Low,' 'Medium,' and 'High' using predefined thresholds. These steps help structure the data for further analysis.

At the end I have used to_csv() method to save dataset to create dashboard  on PowerBI. Feel free to look into my daashboard following the link below.
[https://app.powerbi.com/view?r=eyJrIjoiNjM1YzFlNWQtOTJiOC00NGQwLWFjZmEtYmE3ZWFiYTcyZjNiIiwidCI6ImE0MzEyNWQxLTBmODktNGZhNC05OWFiLTU0NzRjODlmZGQ0MiIsImMiOjl9]


I have uploaded my ipynb file , you can check it for  all details.

