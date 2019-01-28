Movie Mustache

The Situation:
Watching a movie with friends, the twist being that there are is a non-zero number of mustaches on the TV screen and every time a mustache lines up with a character, you drink.

The Process:
1) Find software (a package) that draws bounding boxes on faces
2) Make a 3D histogram of bounding-box-centroids using x,y bins and counts for each x,y coordinate pair
3) Make a GIF of the movie with mustaches right below the top coordinate pairs

The Solution:
1) MTCNN, found in https://towardsdatascience.com/mtcnn-face-detection-cdcb20448ce0, finds nose, mouth-left, and mouth-right locations, the centroid is the mustache location
2) Seaborn distplot
3) GIPHY
