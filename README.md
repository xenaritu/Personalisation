#Information about dataset

This dataset (ml-latest-small) describes 5-star rating and free-text tagging activity from MovieLens,
a movie recommendation service. It contains 100004 ratings and 1296 tag applications across 9125 movies. 
These data were created by 671 users between January 09, 1995 and October 16, 2016. 
This dataset was generated on October 17, 2016.

#Sampling
Users were selected at random for inclusion. All selected users had rated at least 20 movies.

#Further Information About GroupLens

GroupLens is a research group in the Department of Computer Science and Engineering at the University of Minnesota. 
Since its inception in 1992, GroupLens's research projects have explored a variety of fields including:

recommender systems
online communities
mobile and ubiquitious technologies
digital libraries
local geographic information systems
GroupLens Research operates a movie recommender based on collaborative filtering, MovieLens, which is the source of these data. We encourage you to visit http://movielens.org to try it out! If you have exciting ideas for experimental work to conduct on MovieLens, send us an email at grouplens-info@cs.umn.edu - we are always interested in working with external collaborators.

#Content and Use of Files

#Formatting and Encoding

The dataset files are written as comma-separated values files with a single header row.
Columns that contain commas (,) are escaped using double-quotes ("). These files are encoded as UTF-8. 
If accented characters in movie titles or tag values (e.g. MisÃ©rables, Les (1995)) display incorrectly, 
make sure that any program reading the data, such as a text editor, terminal, or script, is configured for UTF-8.

#User Ids

MovieLens users were selected at random for inclusion.Their ids have been anonymized. 
User ids are consistent between ratings.csv and tags.csv (i.e., the same id refers to the same user across the two files).

#Movie Ids

Only movies with at least one rating or tag are included in the dataset. 
These movie ids are consistent with those used on the MovieLens web site
(e.g., id 1 corresponds to the URL https://movielens.org/movies/1). 
Movie ids are consistent between ratings.csv, tags.csv, movies.csv, and 
links.csv (i.e., the same id refers to the same movie across these four data files).

#Ratings Data File Structure (ratings.csv)

All ratings are contained in the file ratings.csv.
Each line of this file after the header row represents one rating of one movie by one user, and has the following format:

userId,movieId,rating,timestamp
The lines within this file are ordered first by userId, then, within user, by movieId.

Ratings are made on a 5-star scale, with half-star increments (0.5 stars - 5.0 stars).

Timestamps represent seconds since midnight Coordinated Universal Time (UTC) of January 1, 1970.

Tags Data File Structure (tags.csv)

All tags are contained in the file tags.csv. Each line of this file after the header row represents one tag applied to one movie by one user, and has the following format:

userId,movieId,tag,timestamp
The lines within this file are ordered first by userId, then, within user, by movieId.

Tags are user-generated metadata about movies. Each tag is typically a single word or short phrase. The meaning, value, and purpose of a particular tag is determined by each user.

Timestamps represent seconds since midnight Coordinated Universal Time (UTC) of January 1, 1970.

Movies Data File Structure (movies.csv)

Movie information is contained in the file movies.csv. Each line of this file after the header row represents one movie, and has the following format:

movieId,title,genres
Movie titles are entered manually or imported from https://www.themoviedb.org/, and include the year of release in parentheses. Errors and inconsistencies may exist in these titles.

Genres are a pipe-separated list, and are selected from the following:

Action
Adventure
Animation
Children's
Comedy
Crime
Documentary
Drama
Fantasy
Film-Noir
Horror
Musical
Mystery
Romance
Sci-Fi
Thriller
War
Western
(no genres listed)
Links Data File Structure (links.csv)

Identifiers that can be used to link to other sources of movie data are contained in the file links.csv. Each line of this file after the header row represents one movie, and has the following format:

movieId,imdbId,tmdbId
movieId is an identifier for movies used by https://movielens.org. E.g., the movie Toy Story has the link https://movielens.org/movies/1.

imdbId is an identifier for movies used by http://www.imdb.com. E.g., the movie Toy Story has the link http://www.imdb.com/title/tt0114709/.

tmdbId is an identifier for movies used by https://www.themoviedb.org. E.g., the movie Toy Story has the link https://www.themoviedb.org/movie/862.

Use of the resources listed above is subject to the terms of each provider.



